# Skirmshop Serial Numbers K8s

GitOps overlay for the `pocharlies-sn-replicas` Shopify app.

- Public path: `https://skirmshop.e-dani.com/sn`
- Source repo: `pocharlies-org/skirmshop-serial-numbers`
- Runtime DB: shared PostgreSQL `serial_numbers`
  (`postgres-shared-rw.databases.svc.cluster.local:5432/serial_numbers`)
- Legacy backup: PVC `serial-data` still contains the pre-Postgres SQLite copy for rollback.
- Secret: `serial-secrets` in namespace `skirmshop` (created from the legacy `.env`, not committed)
