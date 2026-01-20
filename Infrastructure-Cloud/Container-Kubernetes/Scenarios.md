# Container and Kubernetes Security — Scenarios

1. A pod runs as root. How do you fix? — Set runAsNonRoot and drop capabilities.
2. An image has critical CVEs. What do you do? — Rebuild with patched base.
3. A service account has cluster-admin. How do you fix? — Scope permissions.
4. A compromised pod scans the network. How do you stop it? — Apply network policies.
5. A secret is stored in plain YAML. What do you do? — Use external secrets or encryption.
6. A container needs access to hostPath. How do you reduce risk? — Read-only and restrict paths.
7. A new cluster is exposed publicly. What do you do? — Restrict API access and add auth.
8. The kubelet port is open. How do you fix? — Restrict access and enable auth.
9. A developer uses `latest` tag. How do you fix? — Enforce immutable tags.
10. A node is compromised. How do you respond? — Drain, cordon, and rotate creds.
11. A webhook admission controller fails open. What do you do? — Set failurePolicy to Fail.
12. A cluster uses default namespace. How do you improve? — Separate namespaces per team.
13. A service exposes metrics publicly. What do you do? — Add auth and network policies.
14. A cluster stores etcd unencrypted. How do you fix? — Enable encryption at rest.
15. A privileged DaemonSet is required. How do you reduce risk? — Scope and audit.
