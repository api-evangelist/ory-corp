# Ory (ory-corp)

Ory builds open-source identity and access infrastructure and runs it as the Ory Network managed cloud. The stack is composed of Ory Kratos (identities, sessions, and self-service login/registration/recovery/verification/settings flows), Ory Hydra (OAuth2 and OpenID Connect - clients, tokens, consent, and introspection), Ory Keto (Google Zanzibar-style permissions and relationship tuples), and Ory Oathkeeper (zero-trust access proxy). On the Ory Network, all services are exposed on a single project-scoped base URL (`https://{project-slug}.projects.oryapis.com`) with public and admin surfaces, while workspaces, projects, organizations (B2B SSO), event streams, and billing are managed through the Ory Network Console API (`https://api.console.ory.sh`). The Ory projects are Apache-2.0 licensed and self-hostable; the Ory Network is the managed cloud that runs the same engines.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/ory-corp/refs/heads/main/apis.yml)

## Tags

- Identity
- Authentication
- OAuth2
- OpenID Connect
- Authorization
- Permissions
- IAM
- Open Source

## Timestamps

- **Created:** 2026-07-02
- **Modified:** 2026-07-02

## APIs

### Ory Identity API (Kratos - Self-Service)

Public-facing Ory Kratos frontend API for browser and native apps - create and complete self-service login, registration, recovery, verification, settings, and logout flows, and read the current session via `/sessions/whoami` plus list and revoke the caller's own sessions.

- **Human URL:** [https://www.ory.com/docs/kratos/reference/api](https://www.ory.com/docs/kratos/reference/api)
- **Base URL:** `https://{project-slug}.projects.oryapis.com`

#### Tags

- Identity
- Sessions
- Self-Service

#### Properties

- [Documentation](https://www.ory.com/docs/kratos/self-service)
- [API Reference](https://www.ory.com/docs/kratos/reference/api)
- [OpenAPI](openapi/ory-corp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ory-corp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ory-corp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Ory Identity Admin API (Kratos)

Privileged Kratos admin API to list, create, get, update, patch, and delete identities, look up identities by external ID, manage identity credentials, administer sessions (list, get, disable, extend), and issue recovery codes and links on behalf of users.

- **Human URL:** [https://www.ory.com/docs/kratos/reference/api](https://www.ory.com/docs/kratos/reference/api)
- **Base URL:** `https://{project-slug}.projects.oryapis.com`

#### Tags

- Identity
- Admin
- User Management

#### Properties

- [Documentation](https://www.ory.com/docs/kratos/manage-identities/overview)
- [API Reference](https://www.ory.com/docs/kratos/reference/api)
- [OpenAPI](openapi/ory-corp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ory-corp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ory-corp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Ory OAuth2 and OpenID Connect API (Hydra)

Public OAuth2 / OIDC provider endpoints served by Ory Hydra - the authorization endpoint (`/oauth2/auth`), token endpoint (`/oauth2/token`), token revocation, the UserInfo endpoint, and the OpenID Connect discovery and JWKS well-known documents.

- **Human URL:** [https://www.ory.com/docs/hydra/reference/api](https://www.ory.com/docs/hydra/reference/api)
- **Base URL:** `https://{project-slug}.projects.oryapis.com`

#### Tags

- OAuth2
- OpenID Connect
- Tokens

#### Properties

- [Documentation](https://www.ory.com/docs/oauth2-openid-connect-do-you-need-use-cases-products)
- [API Reference](https://www.ory.com/docs/hydra/reference/api)
- [OpenAPI](openapi/ory-corp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ory-corp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ory-corp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Ory OAuth2 Admin API (Hydra)

Privileged Hydra admin API to manage OAuth2 clients (CRUD plus token lifespans), introspect and revoke tokens, drive the login / consent / logout request handshakes, manage JSON Web Key Sets, and administer JWT-bearer grant trust relationships.

- **Human URL:** [https://www.ory.com/docs/hydra/reference/api](https://www.ory.com/docs/hydra/reference/api)
- **Base URL:** `https://{project-slug}.projects.oryapis.com`

#### Tags

- OAuth2
- Clients
- Consent

#### Properties

- [Documentation](https://www.ory.com/docs/hydra/guides/oauth2-clients)
- [API Reference](https://www.ory.com/docs/hydra/reference/api)
- [OpenAPI](openapi/ory-corp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ory-corp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ory-corp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Ory Permissions API (Keto)

Google Zanzibar-style permission checks powered by Ory Keto - check a single permission, run batched checks, expand a subject set into its members, read relationship tuples, and list configured namespaces.

- **Human URL:** [https://www.ory.com/docs/keto/reference/rest-api](https://www.ory.com/docs/keto/reference/rest-api)
- **Base URL:** `https://{project-slug}.projects.oryapis.com`

#### Tags

- Authorization
- Permissions
- Zanzibar

#### Properties

- [Documentation](https://www.ory.com/docs/keto/concepts/api-overview)
- [API Reference](https://www.ory.com/docs/keto/reference/rest-api)
- [OpenAPI](openapi/ory-corp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ory-corp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ory-corp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Ory Relationships API (Keto Write)

Privileged Keto write API to create, update (patch), and delete relationship tuples that define who has what relation to which object, plus a syntax-check endpoint for the Ory Permission Language (OPL) namespace config.

- **Human URL:** [https://www.ory.com/docs/keto/reference/rest-api](https://www.ory.com/docs/keto/reference/rest-api)
- **Base URL:** `https://{project-slug}.projects.oryapis.com`

#### Tags

- Authorization
- Relationship Tuples
- Admin

#### Properties

- [Documentation](https://www.ory.com/docs/keto/reference/ory-permission-language)
- [API Reference](https://www.ory.com/docs/keto/reference/rest-api)
- [OpenAPI](openapi/ory-corp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ory-corp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ory-corp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Ory Courier Messages API

Admin API to list and inspect the courier messages (verification, recovery, and other transactional emails/SMS) that Ory has queued or dispatched, for auditing and delivery troubleshooting.

- **Human URL:** [https://www.ory.com/docs/kratos/reference/api](https://www.ory.com/docs/kratos/reference/api)
- **Base URL:** `https://{project-slug}.projects.oryapis.com`

#### Tags

- Messages
- Email
- Admin

#### Properties

- [Documentation](https://www.ory.com/docs/kratos/self-service/flows/verify-email-account-activation)
- [API Reference](https://www.ory.com/docs/kratos/reference/api)
- [OpenAPI](openapi/ory-corp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ory-corp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ory-corp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Ory Organizations API (B2B SSO)

Admin API to create, list, get, update, and delete organizations that scope B2B customers, each mapping members to their own OIDC/SAML SSO connections and login policies within a single Ory Network project.

- **Human URL:** [https://www.ory.com/docs/kratos/organizations](https://www.ory.com/docs/kratos/organizations)
- **Base URL:** `https://{project-slug}.projects.oryapis.com`

#### Tags

- Organizations
- B2B
- SSO

#### Properties

- [Documentation](https://www.ory.com/docs/kratos/organizations)
- [API Reference](https://www.ory.com/docs/reference/api)
- [OpenAPI](openapi/ory-corp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ory-corp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ory-corp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Ory Network Projects API (Console)

Ory Network Console API to manage the control plane - list workspace projects, and create, get, update (patch/put), and delete projects along with their identity, OAuth2, and permission configuration.

- **Human URL:** [https://www.ory.com/docs/guides/manage-project-via-api](https://www.ory.com/docs/guides/manage-project-via-api)
- **Base URL:** `https://api.console.ory.sh`

#### Tags

- Projects
- Workspaces
- Console

#### Properties

- [Documentation](https://www.ory.com/docs/guides/manage-project-via-api)
- [API Reference](https://www.ory.com/docs/reference/api)
- [OpenAPI](openapi/ory-corp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ory-corp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ory-corp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Ory Network Project API Tokens API

Console API to create, list, and delete the project API tokens (ory_pat_/ory_wak_ keys) that authenticate calls to a project's admin and Console endpoints.

- **Human URL:** [https://www.ory.com/docs/concepts/personal-access-token](https://www.ory.com/docs/concepts/personal-access-token)
- **Base URL:** `https://api.console.ory.sh`

#### Tags

- API Keys
- Tokens
- Console

#### Properties

- [Documentation](https://www.ory.com/docs/concepts/personal-access-token)
- [API Reference](https://www.ory.com/docs/guides/manage-project-via-api)
- [OpenAPI](openapi/ory-corp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ory-corp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ory-corp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Ory Network Event Streams API

Console API to configure event streams that forward Ory Network events (registrations, logins, session and token activity) to external sinks such as AWS SNS - create, list, update, and delete event stream destinations per project.

- **Human URL:** [https://www.ory.com/docs/guides/event-streams/aws-sns](https://www.ory.com/docs/guides/event-streams/aws-sns)
- **Base URL:** `https://api.console.ory.sh`

#### Tags

- Events
- Streaming
- Console

#### Properties

- [Documentation](https://www.ory.com/docs/guides/event-streams/aws-sns)
- [API Reference](https://www.ory.com/docs/reference/api)
- [OpenAPI](openapi/ory-corp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ory-corp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ory-corp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Ory Network Subscriptions and Billing API

Console API to read and manage a workspace or project subscription - inspect the active plan, create or change a subscription, and retrieve the Stripe customer/billing portal context for the Ory Network account.

- **Human URL:** [https://www.ory.com/docs/guides/manage-project-via-api](https://www.ory.com/docs/guides/manage-project-via-api)
- **Base URL:** `https://api.console.ory.sh`

#### Tags

- Billing
- Subscriptions
- FinOps

#### Properties

- [Documentation](https://www.ory.com/pricing)
- [API Reference](https://www.ory.com/docs/reference/api)
- [OpenAPI](openapi/ory-corp-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ory-corp.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ory-corp.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/ory)
- [LinkedIn](https://www.linkedin.com/company/ory)
- [Website](https://www.ory.com)
- [Documentation](https://www.ory.com/docs)
- [Plans](plans/ory-corp-plans-pricing.yml)
- [Rate Limits](rate-limits/ory-corp-rate-limits.yml)
- [Fin Ops](finops/ory-corp-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
