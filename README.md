# Kopperfield

Kopperfield builds design and permitting software for electrical contractors, electricians, inspectors
and instructors. Founded in 2022 as an EV charger installation booking service, it has since become a
broader contractor platform covering NEC-compliant residential and commercial load calculations,
drag-and-drop single line diagrams, panel schedules with circuit directories, AI panel-photo analysis,
and a National Electrical Code chatbot trained on the 2017, 2020 and 2023 code editions. Web plus iOS
and Android apps.

- Website: https://www.kopperfield.com/
- Status: https://status.kopperfield.com/
- GitHub: https://github.com/kopperfieldco
- Backed by: General Catalyst, MCJ Collective, Lachy Groom, Designer Fund

## API posture

**Kopperfield does not currently operate a public developer program.** As of 2026-07-19 there is no
published API reference, OpenAPI/AsyncAPI definition, developer portal, SDK, CLI or public Postman
collection. `api.kopperfield.com` is a live host but serves no public documentation, and
`robots.txt` disallows `/api/` for every crawler. No OpenAPI-dependent artifacts (mcp, overlays,
errors, conventions, data-model, skills, scopes, authentication, arazzo) could be produced without
fabricating them, so they are intentionally absent.

## Artifacts

| Artifact | File | Method |
|---|---|---|
| llms.txt | `llms/kopperfield-llms.txt` | searched (verbatim from `/llms.txt`) |
| Well-Known | `well-known/kopperfield-well-known.yml` | probed — no real document found (site returns a 200 SPA shell for every unknown path) |
| Lifecycle | `lifecycle/kopperfield-lifecycle.yml` | searched — public status page; no versioning/deprecation/SLA policy published |
| Domain security | `security/kopperfield-domain-security.yml` | probed (TLS 1.3, HSTS 2y, SPF + DMARC `p=none`, no DNSSEC, no CAA) |
