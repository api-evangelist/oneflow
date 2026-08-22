# Oneflow (oneflow)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Oneflow is a contract lifecycle management (CLM) and e-signature platform that turns static documents into smart, data-rich digital contracts - covering creation from templates, negotiation, e-signing, and post-sign lifecycle management. The Oneflow Public API is a REST API at `https://api.oneflow.com/v1`, authenticated with an account API token (`x-oneflow-api-token`) plus an acting-user email header (`x-oneflow-user-email`) for permission-scoped authorization. It lets teams programmatically create contracts from templates, add parties and participants, fill data fields and products, publish contracts for signing, download signed files, manage users and workspaces, and subscribe to contract lifecycle events via webhooks. API access and webhooks are available on the Business and Enterprise plans.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/oneflow/refs/heads/main/apis.yml)

## Tags

- Contract Management
- Contract Lifecycle Management
- E-Signature
- Digital Contracts
- Document Automation
- CLM

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### Oneflow Contracts API

Create contracts from templates, retrieve and list contracts, update top-level contract information, publish a draft contract for signing, copy and delete contracts, and download the resulting contract files. The core resource of the Oneflow platform.

- **Human URL:** [https://developer.oneflow.com/docs/create-a-basic-contract](https://developer.oneflow.com/docs/create-a-basic-contract)
- **Base URL:** `https://api.oneflow.com/v1`

#### Tags

- Contracts
- E-Signature
- Lifecycle

#### Properties

- [Documentation](https://developer.oneflow.com/docs/getting-started)
- [API Reference](https://developer.oneflow.com/docs/create-a-basic-contract)
- [OpenAPI](openapi/oneflow-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/oneflow.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/oneflow.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Oneflow Templates API

Retrieve the templates available to a user and inspect template types - the reusable, pre-configured contract definitions that new contracts are created from. Filterable by workspace, template type, and active state.

- **Human URL:** [https://developer.oneflow.com/reference/get-templates](https://developer.oneflow.com/reference/get-templates)
- **Base URL:** `https://api.oneflow.com/v1`

#### Tags

- Templates
- Template Types
- Contract Creation

#### Properties

- [API Reference](https://developer.oneflow.com/reference/get-templates)
- [OpenAPI](openapi/oneflow-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/oneflow.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/oneflow.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Oneflow Workspaces API

List the workspaces in an account - the organizational containers that scope templates, contracts, branding, and permissions. Workspace IDs are required when creating contracts and filtering templates.

- **Human URL:** [https://developer.oneflow.com/reference/get-workspaces](https://developer.oneflow.com/reference/get-workspaces)
- **Base URL:** `https://api.oneflow.com/v1`

#### Tags

- Workspaces
- Organization
- Accounts

#### Properties

- [API Reference](https://developer.oneflow.com/reference/get-workspaces)
- [OpenAPI](openapi/oneflow-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/oneflow.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/oneflow.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Oneflow Data Fields API

Read and update the data fields (custom / merge fields) on a contract and inspect the data fields defined on a template type. Data fields drive the dynamic, data-rich content Oneflow merges into a contract.

- **Human URL:** [https://developer.oneflow.com/docs/data-field.md](https://developer.oneflow.com/docs/data-field.md)
- **Base URL:** `https://api.oneflow.com/v1`

#### Tags

- Data Fields
- Custom Fields
- Merge Fields

#### Properties

- [Documentation](https://developer.oneflow.com/docs/data-field.md)
- [OpenAPI](openapi/oneflow-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/oneflow.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/oneflow.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Oneflow Participants API

Manage the parties (counterparty companies or individuals) and the participants (signatories and viewers) on a contract - add, update, and remove them, and control their signing method, permissions, and delivery channel before a contract is published.

- **Human URL:** [https://developer.oneflow.com/docs/participant.md](https://developer.oneflow.com/docs/participant.md)
- **Base URL:** `https://api.oneflow.com/v1`

#### Tags

- Participants
- Parties
- Signatories

#### Properties

- [Documentation](https://developer.oneflow.com/docs/participant.md)
- [Documentation](https://developer.oneflow.com/docs/party.md)
- [OpenAPI](openapi/oneflow-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/oneflow.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/oneflow.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Oneflow Webhooks API

Register, list, and delete webhook subscriptions that deliver contract lifecycle events (published, signed, declined, and others) to an HTTP callback URL, optionally filtered by event type and workspace. Oneflow's outbound push mechanism - there is no public WebSocket API.

- **Human URL:** [https://developer.oneflow.com/docs/webhook.md](https://developer.oneflow.com/docs/webhook.md)
- **Base URL:** `https://api.oneflow.com/v1`

#### Tags

- Webhooks
- Events
- Callbacks

#### Properties

- [Documentation](https://developer.oneflow.com/docs/webhook.md)
- [OpenAPI](openapi/oneflow-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/oneflow.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/oneflow.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Oneflow Users API

List and retrieve the users in an account - the people whose email addresses back the `x-oneflow-user-email` authorization header and who own contracts, templates, and workspace permissions. Enterprise accounts also provision users and groups via a separate SCIM API.

- **Human URL:** [https://developer.oneflow.com/reference/get-users-in-an-account](https://developer.oneflow.com/reference/get-users-in-an-account)
- **Base URL:** `https://api.oneflow.com/v1`

#### Tags

- Users
- Accounts
- Identity

#### Properties

- [API Reference](https://developer.oneflow.com/reference/get-users-in-an-account)
- [Documentation](https://developer.oneflow.com/docs/user.md)
- [OpenAPI](openapi/oneflow-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/oneflow.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/oneflow.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Oneflow Comments API

Read the inline comments left on a contract during negotiation - the threaded collaboration messages exchanged between internal users and counterparties while a contract is being reviewed and agreed.

- **Human URL:** [https://developer.oneflow.com/docs/contract.md](https://developer.oneflow.com/docs/contract.md)
- **Base URL:** `https://api.oneflow.com/v1`

#### Tags

- Comments
- Collaboration
- Contracts

#### Properties

- [Documentation](https://developer.oneflow.com/docs/contract.md)
- [OpenAPI](openapi/oneflow-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/oneflow.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/oneflow.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/oneflowcom)
- [Website](https://oneflow.com)
- [Documentation](https://developer.oneflow.com)
- [Plans](plans/oneflow-plans-pricing.yml)
- [Rate Limits](rate-limits/oneflow-rate-limits.yml)
- [Fin Ops](finops/oneflow-finops.yml)

## Authentication

Every request to the Oneflow Public API (`https://api.oneflow.com/v1`) requires two HTTP headers:

- `x-oneflow-api-token` — the account API token, generated under **Marketplace → API tokens** in the Oneflow application.
- `x-oneflow-user-email` — the email of the acting Oneflow user, used for permission-scoped authorization (omitting it runs the request as an anonymous admin user).

Validate a token with `GET /v1/ping`, which returns `200` and an empty object on success.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
