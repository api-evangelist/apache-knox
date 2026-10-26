# Apache Knox (apache-knox)

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

Apache Knox is a REST API and application gateway for the Apache Hadoop ecosystem. It provides a single access point for all REST and HTTP interactions with Apache Hadoop clusters, with authentication, authorization, SSO, and audit capabilities.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/apache-knox/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - API Gateway, Authentication, Hadoop, Open Source, Security, SSO

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-04-19

## APIs

### Apache Knox Admin REST API
The Knox Admin REST API provides endpoints for topology management, service descriptor management, provider configuration, and version information.

**Human URL:** [https://knox.apache.org/books/knox-2-0-0/user-guide.html](https://knox.apache.org/books/knox-2-0-0/user-guide.html)

#### Tags:

 - Administration, API Gateway, REST

#### Properties

- [Documentation](https://knox.apache.org/books/knox-2-0-0/user-guide.html)
- [OpenAPI](openapi/apache-knox-admin-api.yaml)

### Apache Knox Gateway API
The Knox gateway proxies and secures access to Hadoop ecosystem services including HDFS, Hive, HBase, YARN, and Oozie.

**Human URL:** [https://knox.apache.org/books/knox-2-0-0/user-guide.html#Service+Details](https://knox.apache.org/books/knox-2-0-0/user-guide.html#Service+Details)

#### Tags:

 - API Gateway, Hadoop, Proxy, Security

#### Properties

- [Documentation](https://knox.apache.org/books/knox-2-0-0/user-guide.html#Service+Details)

## Common Properties

- [GitHubOrganization](https://github.com/apache)
- [GitHubRepository](https://github.com/apache/knox)
- [Documentation](https://knox.apache.org/books/knox-2-0-0/user-guide.html)
- [GettingStarted](https://knox.apache.org/books/knox-2-0-0/user-guide.html#Quick+Start)
- [TermsOfService](https://www.apache.org/licenses/LICENSE-2.0)
- [SpectralRules](rules/apache-knox-spectral-rules.yml)
- [Vocabulary](vocabulary/apache-knox-vocabulary.yaml)
- [NaftikoCapability](capabilities/gateway-management.yaml)

## Features

| Name | Description |
|------|-------------|
| Single Access Point | Unified gateway for all Hadoop REST services eliminating direct cluster access. |
| Authentication | Kerberos, LDAP, OAuth2, and JWT authentication support. |
| SSO Integration | SAML2-based SSO and token-based federation across Hadoop services. |
| Authorization | Fine-grained authorization via Apache Ranger integration. |
| SSL/TLS Termination | SSL/TLS termination at the gateway for encrypted communication. |
| Service Discovery | Automatic service discovery via Ambari and Cloudera Manager integration. |
| Topology Management | Dynamic topology configuration without gateway restarts. |
| Audit Logging | Comprehensive audit logs for all gateway interactions. |

## Use Cases

| Name | Description |
|------|-------------|
| Hadoop Cluster Security | Secure and centralize access to all Hadoop REST APIs through Knox. |
| Cloud Hadoop Access | Provide secure REST access to EMR, HDInsight, and Dataproc clusters. |
| Hadoop SSO | Enable single sign-on across Ambari, Hue, Spark UI, and other Hadoop UIs. |
| REST API Proxying | Proxy WebHDFS, Hive JDBC/REST, HBase REST, and YARN REST through Knox. |

## Integrations

| Name | Description |
|------|-------------|
| Apache Hadoop HDFS | WebHDFS REST API proxied and secured through Knox. |
| Apache Hive | Hive JDBC and REST API access via Knox gateway. |
| Apache HBase | HBase REST API proxied through Knox with authentication. |
| Apache Ranger | Authorization policy enforcement via Ranger Knox plugin. |
| Apache Ambari | Ambari REST API proxied through Knox for cluster management. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Apache Knox Admin REST API](openapi/apache-knox-admin-api.yaml)

### JSON Schema

5 schema files extracted from the Admin REST API OpenAPI specification.

### JSON Structure

5 JSON Structure files converted from JSON Schema files.

### Examples

5 example JSON files generated from JSON Schema definitions.

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Apache Knox Admin REST API](capabilities/shared/knox-admin-api.yaml) — 4 operations for topology management

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Apache Knox Gateway Management](capabilities/gateway-management.yaml) | Apache Knox Admin REST API | 5 | Hadoop Administrator, Security Engineer |

## Vocabulary

- [Apache Knox Vocabulary](vocabulary/apache-knox-vocabulary.yaml) — Unified taxonomy mapping 4 resources, 4 actions, 1 workflow, and 2 personas

## Rules

- [Apache Knox Spectral Rules](rules/apache-knox-spectral-rules.yml) — 13 rules across 7 categories enforcing Apache Knox Admin API conventions

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
