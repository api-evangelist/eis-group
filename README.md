# EIS Group (eis-group)

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

EIS Group (EIS Ltd) is a United States core-systems vendor for insurance, founded in 2008 out of Exigen Insurance Solutions and headquartered in San Francisco, California. EIS sells the EIS Platform and EIS OneSuite — a cloud-native, microservices core suite covering customer management, policy administration, billing, and claims — across group benefits, property and casualty / general, protection, life and annuities, and pet insurance.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/eis-group/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/eis-group/refs/heads/main/apis.yml)

## API Posture

EIS markets itself as API-first and claims thousands of open REST APIs — a 2019 press release announced "over 1,100 REST APIs" in the EIS DXP digital experience platform, and current EIS OneSuite marketing claims "9,000+ APIs." **None of that surface is public.**

- **No self-serve developer portal.** `developer.eisgroup.com`, `developers.eisgroup.com`, `api.eisgroup.com`, `apidocs.eisgroup.com`, `portal.eisgroup.com`, `sandbox.eisgroup.com` and `developerportal.eisgroup.com` do not resolve. `eisgroup.com/developers` and `eisgroup.com/developer` return HTTP 404.
- **Documentation is a login wall.** [docs.eisgroup.com](https://docs.eisgroup.com/) returns **HTTP 401** with `WWW-Authenticate: Basic realm="EIS Group Users"` on every path probed — a blanket HTTP Basic wall in front of the whole documentation tree.
- **No harvestable specifications.** Zero OpenAPI, Swagger, GraphQL SDL, AsyncAPI or `.proto` artifacts are published. `/openapi.json`, `/swagger.json` and `/api-docs` all 404 on the marketing host and 401 on the docs host.
- **No public Postman collections.** A team profile exists at [postman.com/eis-group-8390](https://www.postman.com/eis-group-8390) but publishes 0 collections, 0 workspaces, 0 APIs.
- **Open source is libraries, not APIs.** [github.com/eisgroup](https://github.com/eisgroup) publishes `kraken-rules` (Java business rules engine) and `ui-render` (React dynamic UI rendering). A second org, `eis-group-opensource`, holds 75 forks of third-party Java/Scala libraries.
- **Quote / bind / issue / FNOL** are all marketed — FNOL is a named use case — and none is exposed as a public API. Every verb is reachable only inside a licensed EIS implementation.
- **Auth model is undocumented publicly.** No `/.well-known/openid-configuration` and no `/.well-known/oauth-authorization-server` on any EIS host. The only observable scheme is HTTP Basic on the documentation wall.
- **No webhook or event catalog.** The platform is marketed as event-driven and an analyst evaluation names JMS, AMQP and Kafka as transports, but no schema, topic list or AsyncAPI document is public.

## ACORD Posture

ACORD and certified ACORD integration attested in an analyst evaluation hosted on eisgroup.com; no public ACORD/AL3/NGDS/IVANS artifacts.

The sole public evidence is the [Aite Matrix: 2020 US P&C Core Systems Evaluation](https://www.eisgroup.com/wp-content/uploads/2022/10/aite-matrix-2020-u-s-pc-core-systems-evaluation.pdf) PDF hosted on eisgroup.com, which states verbatim:

> The system uses web services, APIs, RESTful APIs, ACORD and certified ACORD to integrate ETPD. It can also use JMS, AMQP, and Kafka.

A site search for ACORD on eisgroup.com otherwise returns only a 2016 ACORD conference sponsorship press release. No ACORD XML schemas, AL3 mappings, NGDS references, IVANS / agency-download detail, or Applied Epic / Vertafore AMS360 connector documentation is published.

## Tags

- Insurance
- United States
- Core Systems
- Policy Administration
- Claims
- Billing
- Underwriting
- Property and Casualty
- Life Insurance
- Employee Benefits
- Insurtech
- ACORD

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

None. EIS Group publishes no public, self-serve API. Its entire API estate is sold with a licensed implementation and documented behind a customer login wall. See [review.yml](review.yml) for the full probe record and HTTP statuses.

## Common Properties

- [Website](https://www.eisgroup.com/)
- [Documentation](https://docs.eisgroup.com/) — gated, HTTP 401 Basic auth
- [Blog](https://www.eisgroup.com/blog/)
- [Blog RSS](https://www.eisgroup.com/feed/)
- [Newsroom](https://www.eisgroup.com/company/newsroom/)
- [Partners](https://www.eisgroup.com/company/partners/)
- [Partner Application](https://www.eisgroup.com/company/partner-application/)
- [GitHub Organization](https://github.com/eisgroup)
- [LinkedIn](https://www.linkedin.com/company/eisgroupltd)
- [Contact](https://www.eisgroup.com/company/contact/)

## Maintainers

- Kin Lane — kin@apievangelist.com
