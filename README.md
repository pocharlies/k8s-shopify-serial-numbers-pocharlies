# Skirmshop Serial Numbers K8s

GitOps overlay for the `pocharlies-sn-replicas` Shopify app.

- Public path: `https://skirmshop.e-dani.com/sn`
- Source repo: `pocharlies-org/skirmshop-serial-numbers`
- Runtime DB: SQLite at `/data/dev.sqlite` on PVC `serial-data`
- Secret: `serial-secrets` in namespace `skirmshop` (created from the legacy `.env`, not committed)
