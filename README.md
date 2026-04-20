# Apache Knox (apache-knox)
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
