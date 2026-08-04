# ABC Trainerize (trainerize)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

ABC Trainerize is a personal-training and fitness-coaching software platform for trainers, studios, and gyms - online training, workout programming, nutrition and meal planning, habit and goal tracking, in-app messaging, and a custom-branded client app. Its partner API lets integrators add, modify, and retrieve client data - clients, programs and workouts, goals, habits, body stats, nutrition, appointments, tags, and groups - and register webhooks for business events.

> **Access model (read first).** The ABC Trainerize API is a **partner / private API, not open self-serve.** API access and webhook registration are available **only on the Studio and Enterprise plans**. Credentials (an **API key** and/or an **OAuth2** connection) are provisioned from the ABC Trainerize account settings. ABC Trainerize support explicitly does **not** help build API calls, and the full API reference lives behind the authenticated help center - there is **no openly published OpenAPI document**. Enterprise plans add dedicated integration support.

> **Parent company.** ABC Trainerize is a product of **ABC Fitness Solutions**, which acquired Trainerize in 2021. ABC Fitness also runs its own separate developer program at `developers.abcfitness.com`; that is a **different** API surface and is not conflated with the Trainerize API cataloged here.

> **Grounding & honesty note.** The API **host and version prefix** (`https://api.trainerize.com/v03`) were **confirmed live** by direct probing on 2026-07-12 (TLS 1.3, Microsoft-IIS 10 / ASP.NET Web API, behind Cloudflare + AWS ELB; the `/v03` prefix returns 200, and unknown sub-paths return ASP.NET "No HTTP resource was found" 404s). The **individual operation paths and request/response schemas** in the OpenAPI and collections are **MODELED** from ABC Trainerize's publicly documented capabilities (the help center API/webhooks article and the published Zapier / Latenode partner action catalog) - they are representative, not copied from a public reference. Treat exact paths, parameter names, and payloads as illustrative and verify against the gated docs before implementation.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/apis.yml)

## Tags

- Fitness
- Personal Training
- Coaching
- Fitness Software
- Client Management
- SaaS

## Timestamps

- **Created:** 2026-07-12
- **Modified:** 2026-07-12

## APIs

### ABC Trainerize Clients API

Create, update, find, deactivate, and reactivate clients; assign clients to trainers; and manage client tags and group membership. Used to onboard clients from a form or sync them with a CRM.

- **Human URL:** [Using API and Webhooks With ABC Trainerize](https://help.trainerize.com/hc/en-us/articles/37082084919060-Using-API-and-Webhooks-With-ABC-Trainerize)
- **Base URL:** `https://api.trainerize.com/v03`

#### Tags

- Clients
- Client Management
- CRM

#### Properties

- [Documentation](https://help.trainerize.com/hc/en-us/articles/37082084919060-Using-API-and-Webhooks-With-ABC-Trainerize)
- [OpenAPI](openapi/trainerize-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/trainerize.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/trainerize.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ABC Trainerize Training Programs API

Assign training to clients - copy a master program onto a client, subscribe a client to a main or add-on program, unsubscribe from programs, add the next training phase, and retrieve a client's workouts.

- **Human URL:** [Using API and Webhooks With ABC Trainerize](https://help.trainerize.com/hc/en-us/articles/37082084919060-Using-API-and-Webhooks-With-ABC-Trainerize)
- **Base URL:** `https://api.trainerize.com/v03`

#### Tags

- Workout Programming
- Programs
- Workouts

#### Properties

- [Documentation](https://help.trainerize.com/hc/en-us/articles/37082084919060-Using-API-and-Webhooks-With-ABC-Trainerize)
- [OpenAPI](openapi/trainerize-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/trainerize.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/trainerize.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ABC Trainerize Client Data API

Add, modify, and retrieve a client's goals, habits, body stats, nutrition, and appointments.

- **Human URL:** [Using API and Webhooks With ABC Trainerize](https://help.trainerize.com/hc/en-us/articles/37082084919060-Using-API-and-Webhooks-With-ABC-Trainerize)
- **Base URL:** `https://api.trainerize.com/v03`

#### Tags

- Goals
- Habits
- Nutrition

#### Properties

- [Documentation](https://help.trainerize.com/hc/en-us/articles/37082084919060-Using-API-and-Webhooks-With-ABC-Trainerize)
- [OpenAPI](openapi/trainerize-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/trainerize.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/trainerize.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ABC Trainerize Messaging API

Send in-app messages to clients and upload attachments such as meal-plan PDFs.

- **Human URL:** [Using API and Webhooks With ABC Trainerize](https://help.trainerize.com/hc/en-us/articles/37082084919060-Using-API-and-Webhooks-With-ABC-Trainerize)
- **Base URL:** `https://api.trainerize.com/v03`

#### Tags

- Messaging
- Attachments
- Communication

#### Properties

- [Documentation](https://help.trainerize.com/hc/en-us/articles/37082084919060-Using-API-and-Webhooks-With-ABC-Trainerize)
- [OpenAPI](openapi/trainerize-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/trainerize.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/trainerize.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ABC Trainerize Webhooks API

Register, list, and delete webhook subscriptions that notify an external system when a business event occurs - workout completed, cardio completed, habit completed, daily nutrition goal hit, weight goal hit, new client, new purchase, product start/end, auto-renew cancelled, and tag added/removed. Webhooks are one-way, server-to-endpoint HTTP POSTs.

- **Human URL:** [Using API and Webhooks With ABC Trainerize](https://help.trainerize.com/hc/en-us/articles/37082084919060-Using-API-and-Webhooks-With-ABC-Trainerize)
- **Base URL:** `https://api.trainerize.com/v03`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://help.trainerize.com/hc/en-us/articles/37082084919060-Using-API-and-Webhooks-With-ABC-Trainerize)
- [OpenAPI](openapi/trainerize-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/trainerize.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/trainerize.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Domain Security](security/trainerize-domain-security.yml)
- [Authentication](authentication/trainerize-authentication.yml)
- [LinkedIn](https://www.linkedin.com/company/trainerize)
- [Website](https://www.trainerize.com)
- [Documentation](https://help.trainerize.com/hc/en-us/articles/37082084919060-Using-API-and-Webhooks-With-ABC-Trainerize)
- [Plans](plans/trainerize-plans-pricing.yml)
- [Rate Limits](rate-limits/trainerize-rate-limits.yml)
- [Fin Ops](finops/trainerize-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
