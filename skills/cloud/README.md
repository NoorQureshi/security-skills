# Cloud & containers — `cloud` skills

AWS/GCP/Azure and Kubernetes/containers: metadata/IMDS abuse, object-storage misconfig, IAM escalation, exposed control planes.

## Skills in this domain

- [`cloud-azure`](cloud-azure/SKILL.md) — Attack Azure / Entra ID — managed-identity token theft, Entra (Azure AD) role abuse, and app/storage misconfig.
- [`cloud-container-escape`](cloud-container-escape/SKILL.md) — Break out of a container to the host.
- [`cloud-docker-api-abuse`](cloud-docker-api-abuse/SKILL.md) — Turn an exposed container daemon or an over-privileged container into host compromise — a Docker API on 2375/2376, a mounted docker.sock, or a privileged container.
- [`cloud-docker-registry`](cloud-docker-registry/SKILL.md) — Find and loot exposed container registries — image pull/push, secrets baked in layers, and registry misconfig.
- [`cloud-gcp`](cloud-gcp/SKILL.md) — Attack Google Cloud Platform — metadata/SA token theft, IAM privilege escalation, and storage/function misconfig.
- [`cloud-iam-privesc`](cloud-iam-privesc/SKILL.md) — Escalate privileges in cloud IAM (AWS/GCP/Azure) from a low-priv set of credentials.
- [`cloud-imds-ssrf`](cloud-imds-ssrf/SKILL.md) — Escalate SSRF to cloud credential theft via the instance metadata service (IMDS).
- [`cloud-kubernetes`](cloud-kubernetes/SKILL.md) — Attack exposed Kubernetes: API server, kubelet, etcd, dashboards, and RBAC.
- [`cloud-s3-exposure`](cloud-s3-exposure/SKILL.md) — Find and prove misconfigured cloud object storage (S3/GCS/Azure Blob).

Add a skill here:
```bash
cp -r skills/_templates/technique.md skills/cloud/<slug>/SKILL.md
# edit frontmatter (domain: cloud) + body, then:
python3 tools/catalog.py
```

Naming: domain-prefixed kebab-case, e.g. `cloud-<thing>`. See the full table in [`CATALOG.md`](../../docs/CATALOG.md).
