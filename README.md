# Cartography (cartography)

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
