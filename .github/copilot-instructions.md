# Copilot instructions — brand-promoter-api

Stack: NestJS + Prisma + PostgreSQL. Product: Brand Promoter Management System.

**Functional source of truth:** sibling `../brand-promoter-docs/docs/` in the multi-root workspace. Read scope, matrix, HU spec, ADRs and DoD before implementation. If inaccessible, stop and request specific files.

Implement only endpoints in approved specs. JWT guards, roles and server-side store checks. Validated DTOs; Prisma transactions for receptions; API-generated OpenAPI. Do not expose passwordHash or secrets. PostgreSQL integration tests. No Docker/registry without ADR.

Work by HU and small PR. Inspect Git before editing. Propose a plan and await approval for broad changes. Do not assume tests were executed. Do not change contracts without documenting impact on other repositories.

## Naming and AI workflow
- Official name: Brand Promoter Management System. Technical repository prefix: `brand-promoter`.
- Use English for technical identifiers, filenames, API routes, DB objects, branches and commits; Use Spanish for business-facing specifications and UI copy. Follow the bilingual glossary and language policy in the documentation repository.
- Follow `../brand-promoter-docs/docs/process/naming-conventions.md`, `sdd-copilot.md`, `review-gates.md`, and `change-control.md`.
- Approved specs are the source of truth. Do not silently change them.
- For a completed or blocked HU, report real commands and test evidence using the implementation report template.
- Escalate cross-repository breaking contracts, schema/auth changes, new infrastructure and persistent defects.
