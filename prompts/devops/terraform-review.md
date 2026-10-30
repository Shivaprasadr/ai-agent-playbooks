# Terraform review

Review `<TERRAFORM_SCOPE>` for concrete configuration or operational risks.

Inspect the relevant modules, variables, providers, and references. Prefer static, non-mutating validation; do not run `apply`, change state, or access live infrastructure without explicit authorization. Report evidence-backed findings and distinguish code evidence from environment-dependent assumptions. Redact secrets and sensitive values.
