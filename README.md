# Cartography (cartography)

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

Cartography is an open-source Python security-graph tool originally built at Lyft that consolidates infrastructure assets and the relationships between them into an intuitive Neo4j graph. It ingests data from 30+ cloud, identity, DevOps, and security providers (AWS, GCP, Azure, OCI, Okta, Entra ID, GitHub, Kubernetes, CrowdStrike, and more) and lets security teams answer cross-provider questions such as "which identities can reach which datastores," "which compute instances are exposed to the internet," and "what are the blast radii of a compromised credential."

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/cartography/refs/heads/main/apis.yml)

## Scope

- **Type:** Standard
- **Position:** Consumer
- **Access:** Open

## Tags

 - Security, Cloud Security, Graph, CSPM, Neo4j, Open Source, Lyft, Asset Inventory, Identity

## Timestamps

- **Created:** 2025-01-01
- **Modified:** 2026-04-23

## APIs

### Cartography

Python tool that ingests infrastructure data from 30+ providers into a Neo4j graph for cross-provider security analysis.

**Human URL:** [https://lyft.github.io/cartography/](https://lyft.github.io/cartography/)

#### Tags

 - Security, Cloud Security, Graph, Neo4j

#### Properties

- [Documentation](https://lyft.github.io/cartography/)
- [Repository](https://github.com/lyft/cartography)
- [Cypher Query Language](https://neo4j.com/docs/cypher-manual/current/)

### Cartography AWS Intel Module

Cartography intel module that calls AWS APIs (EC2, IAM, S3, RDS, EKS, Lambda, ECS, DynamoDB, CloudWatch, ACM, KMS, CodeBuild, API Gateway, Bedrock, and more) to populate AWS nodes and relationships in the graph.

**Human URL:** [AWS Module](https://lyft.github.io/cartography/modules/aws/index.html)

#### Tags

 - AWS, Cloud, Ingest

### Cartography Google Cloud Intel Module

Cartography intel module that calls Google Cloud APIs (Compute, IAM, Cloud SQL, GKE, Cloud Functions, Artifact Registry, Vertex AI) to populate GCP nodes and relationships in the graph.

**Human URL:** [GCP Module](https://lyft.github.io/cartography/modules/gcp/index.html)

#### Tags

 - GCP, Cloud, Ingest

### Cartography Azure Intel Module

Cartography intel module that calls Azure APIs (App Service, AKS, CosmosDB, Container Instance, Key Vault, Storage, Virtual Machines) to populate Azure nodes and relationships in the graph.

**Human URL:** [Azure Module](https://lyft.github.io/cartography/modules/azure/index.html)

#### Tags

 - Azure, Cloud, Ingest

### Cartography Oracle Cloud Intel Module

Cartography intel module that calls Oracle Cloud Infrastructure APIs (starting with IAM) to populate OCI nodes and relationships.

#### Tags

 - OCI, Cloud, Ingest

### Cartography Okta Intel Module

Ingests Okta users, groups, applications, and factors into the graph for identity-focused security analysis.

#### Tags

 - Identity, Okta, Ingest

### Cartography Entra ID Intel Module

Ingests Microsoft Entra ID users, groups, applications, and role assignments into the graph.

#### Tags

 - Identity, Entra ID, Ingest

### Cartography GitHub Intel Module

Ingests GitHub organizations, repositories, users, and access relationships, enabling code-ownership and secret-exposure graph queries.

#### Tags

 - GitHub, SCM, Ingest

### Cartography Kubernetes Intel Module

Ingests Kubernetes cluster objects (nodes, pods, services, service accounts) for graph-based cluster-security analysis.

#### Tags

 - Kubernetes, Containers, Ingest

### Cartography CrowdStrike Intel Module

Ingests CrowdStrike Falcon hosts and detections, connecting endpoint telemetry to the infrastructure graph.

#### Tags

 - EDR, CrowdStrike, Ingest

### Cartography Cloudflare Intel Module

Ingests Cloudflare zones, DNS, and security configurations into the graph for edge-exposure analysis.

#### Tags

 - DNS, Edge, Ingest

## Use Cases

- Cross-provider access review — "which Okta users ultimately have admin on any AWS account?" using Okta-to-AWS identity federation relationships.
- Exposure analysis — enumerating all EC2 instances, GCP VMs, or Azure VMs with a public IP plus a permissive security group and no patching telemetry.
- Datastore blast-radius — tracing all IAM principals and assumed-role paths that can read a specific S3 bucket, RDS instance, or CosmosDB.
- Code-to-cloud ownership — joining GitHub repository ownership with the cloud resources those repos deploy, to route security findings to the responsible team.
- EDR correlation — connecting CrowdStrike detections to the underlying cloud compute instance, owning service, and responsible identity in a single Cypher query.
- Continuous asset inventory — scheduled Cartography runs feeding dashboards and ticketing based on drift, new exposures, or new principals.
- Compliance graph queries — answering auditor questions like "which production databases are un-encrypted or publicly reachable" with a single Cypher query.

## Common Properties

- [Website](https://lyft.github.io/cartography/)
- [Documentation](https://lyft.github.io/cartography/)
- [Lyft GitHub Org](https://github.com/lyft)
- [Repository](https://github.com/lyft/cartography)
- [Issues](https://github.com/lyft/cartography/issues)
- [Getting Started](https://lyft.github.io/cartography/install.html)
- [Tutorial](https://lyft.github.io/cartography/usage/tutorial.html)
- [License (Apache 2.0)](https://github.com/lyft/cartography/blob/master/LICENSE)
- [Releases](https://github.com/lyft/cartography/releases)
- [Lyft Engineering Blog](https://eng.lyft.com/open-sourcing-cartography-4611ba31a72)
- [JSON-LD Context](json-ld/cartography-context.jsonld)
- [Vocabulary Definition](vocabulary.yml)
- [Spectral Rules](spectral/cartography.spectral.yml)

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
