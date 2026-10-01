# Proposed data handling for the ChartFox feature

Updated 30 September 2026. **Design proposal, not a verified description of implemented software or a final privacy policy.**

The ChartFox integration has not been represented as implemented. Its final data flows depend on the approved authentication and API design.

## Intended handling

- Request only the permissions necessary for the user-selected chart workflow.
- Keep provider sign-in within the provider-approved authorization flow; do not collect provider passwords in AERION.
- Send only the information necessary for approved authorization, airport selection and chart retrieval.
- Keep access credentials out of the public repository, exported flight reports, diagnostic logs and OBS views.
- Do not distribute confidential client secrets in desktop code or browser assets.
- Store tokens using an appropriate protected mechanism once the supported client model is confirmed.
- Offer disconnect and local credential removal; follow provider guidance for revocation.
- Avoid chart caching until its permitted scope and retention have been confirmed.

## Before release

Document the actual data collected, storage locations, retention, third-party recipients, deletion process and a working privacy contact. Verify the implementation against that notice before publishing it as a privacy policy. This proposal must not be submitted as a final privacy policy if ChartFox requires one.

Public questions may be raised through repository issues. Do not include personal account information or tokens in public issues.
