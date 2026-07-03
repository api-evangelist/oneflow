# Oneflow (oneflow)

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
