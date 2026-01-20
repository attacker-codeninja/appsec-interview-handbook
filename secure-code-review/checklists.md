# Secure Code Review Checklists

Language-specific items to look for during review.

## General Checklist

- Authentication and authorization checks on all sensitive actions
- Input validation and output encoding by context
- Use of safe APIs (parameterized queries, safe serializers)
- Secrets management and no hardcoded credentials
- Proper logging without sensitive data leakage
- Dependency and supply-chain risk controls
- Secure error handling and no debug info in prod

## Critical 5 (10-Minute Cram)

- **AuthZ everywhere**: Verify server-side **authorization** on every sensitive action.
- **Source to sink**: Trace untrusted input to dangerous `sinks`.
- **Safe APIs**: Prefer parameterized queries and vetted libraries.
- **Secrets control**: No hardcoded secrets; use managed secret stores.
- **Supply chain**: Pin dependencies and verify provenance.

## Red Flags

- **Bypassable authZ** via client-side checks
- **Untrusted deserialization** with `readObject`/`pickle`-style APIs
- **SSRF-capable** URL fetchers with no allowlist
- **Mutable** dependencies or base images (`latest`)
- **Missing** audit trails for admin actions

## Java

- Use of `PreparedStatement` for DB access
- Avoid Java native serialization on untrusted data
- Safe XML parsing (`XXE` protections)
- Proper validation for Spring controllers
- Use of `@PreAuthorize`/`@PostAuthorize` or centralized authZ
- TLS config and hostname verification

## Python

- Avoid `eval`, `exec`, and `pickle` on untrusted input
- Use parameterized SQL in DB libraries
- Safe subprocess usage (`subprocess` without shell)
- Proper URL validation to prevent SSRF
- Secure deserialization (JSON over pickle)
- Input validation via schemas (Pydantic, Marshmallow)

## C/C++

- Bounds checking on buffers and arrays
- Use safe string APIs and avoid `strcpy`/`sprintf`
- Memory lifecycle: avoid use-after-free/double free
- Use of modern C++ containers (`std::string`, `std::vector`)
- Integer overflows in size calculations
- Secure compilation flags (`-fstack-protector`, ASLR)

## JavaScript (Node.js)

- Avoid `eval` and unsafe dynamic requires
- Validate and sanitize request bodies and params
- Use `helmet` and proper security headers
- Prevent prototype pollution (`__proto__`, `constructor`)
- Safe file path handling (`path.join` + allowlists)
- Ensure async errors are handled and not ignored

## Go

- Use **context timeouts** for external calls
- Validate JSON input with struct tags (e.g., `json` tags)
- Use `database/sql` with **prepared statements**
- Check for **SSRF** on URL fetchers
- Avoid `os/exec` with untrusted inputs

## Rust

- Review **`unsafe` blocks** for memory safety assumptions and invariants
- Check **integer overflows** in arithmetic and conversions (e.g., `as`, `checked_add`)
- Validate **FFI boundaries** for untrusted inputs
- Ensure **panic safety** does not bypass authZ or input checks
- Audit dependencies with `cargo audit` and review `Cargo.lock`
- Prefer **safe crates** over custom crypto or parsers

## Mobile (Swift/Kotlin)

- Verify **biometric auth** uses OS-backed APIs (`LocalAuthentication`, `BiometricPrompt`)
- Store secrets in **Keychain/Keystore** (e.g., `Keychain`, `AndroidKeyStore`)
- Confirm **Secure Enclave/StrongBox** usage for high-value keys
- Enforce **certificate pinning** with rotation strategy
- Validate **deep links** and URL schemes (allowlist, authZ check)
- Ensure **sensitive data** is excluded from backups and logs

## TypeScript

- Treat **type safety** as compile-time only; validate at runtime
- Avoid `any` and `unknown` misuse; require explicit narrowing
- Use **schema validation** (e.g., `zod`, `valibot`) at boundaries
- Guard **JSON parsing** and external inputs with validators
- Ensure **strict** compiler settings (e.g., `noImplicitAny`)

## IaC (Terraform/CloudFormation)

- No public S3 buckets or open security groups
- Enforce **encryption** at rest and in transit
- Avoid wildcard IAM policies
- Enable **audit logging** and monitoring
- Use private subnets and minimal ingress

## GraphQL

- Enforce **depth limiting** to prevent expensive queries
- Apply **query complexity analysis** and cost budgets
- Implement **field-level authorization** and ownership checks
- Avoid **over-fetching** sensitive fields by default
- Validate **input types** and custom scalars

## Serverless (AWS Lambda/Azure Functions)

- Validate **event payloads** to prevent event injection
- Configure **timeouts** and memory limits per function
- Enforce **least privilege IAM** per function (no shared broad roles)
- Avoid **secret exposure** in env vars; use managed secret stores
- Restrict **egress** to prevent SSRF and data exfiltration

## AI/LLM Integration

- Mitigate **prompt injection** by separating system and user content
- Filter **PII** and secrets from prompts and outputs
- Validate **LLM output** before use (schema checks, allowlists)
- Prevent **tool/function abuse** with strict input validation
- Log **model interactions** with redaction and audit controls

## Cloud Native and Kubernetes (Senior Scenarios)

- **Privileged DaemonSet** required for observability; how do you reduce blast radius and enforce `PSA`?
- **Cluster-admin service account** is mounted in pods; how do you move to workload identity?
- **Unsigned images** are allowed; how do you enforce `cosign` verification via admission control?
- **Namespace isolation** breaks and cross-tenant access occurs; how do you fix `RBAC` and `NetworkPolicy`?
- **`hostPath` mounts** are used for logs; how do you prevent host escape?
- **`etcd` is unencrypted**; how do you remediate without downtime?
- **`latest` tags** deployed in prod; how do you enforce digest pinning?
- **Admission webhook** is fail-open; what risks and how to fix?
- **Secrets in etcd** are plaintext; how do you enable encryption and rotate?
- **Runtime policy alert** fires (crypto mining); how do you triage and contain?

## Essential Security Research Resources

| Resource | Why It Matters | Link |
| --- | --- | --- |
| OWASP ASVS | **Baseline** security requirements for applications | https://owasp.org/www-project-application-security-verification-standard/ |
| CWE | **Taxonomy** of software weaknesses | https://cwe.mitre.org/ |
| PayloadsAllTheThings | **Practical payloads** for testing and validation | https://github.com/swisskyrepo/PayloadsAllTheThings |
| Google KPR Framework | **Know, Prevent, Retain** strategy for security programs | https://security.googleblog.com/2019/08/know-prevent-retain.html |

## Visual Asset Descriptions

- **Untrusted Input Pipeline**: Diagram showing `source` -> **validation** -> **sanitization** -> `sink`, with trust boundaries highlighted.
- **GraphQL Query Risk Map**: Diagram of query depth and **field-level authZ** gates across a resolver tree.
- **Serverless Event Flow**: Diagram of event source -> **validation** -> function -> **IAM checks** -> downstream services, with failure paths.
