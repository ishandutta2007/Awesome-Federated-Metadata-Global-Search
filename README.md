# Awesome-Federated-Metadata-Global-Search

# Top Federated Metadata & Global Search Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on Cross-Silo Search, Metadata Federation & Self-Hosted Enterprise Search*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Federated Metadata & Global Search**. These tools help organizations query across disparate systems—SaaS apps, databases, file shares, and legacy repositories—without migrating data into a central store. The category spans **enterprise search platforms** with pre-built connectors and AI assistants (Glean, Coveo, Lucidworks) and **federated query engines** that leave data in place while unifying results (Swirl, Sercha).

**Examples** include Glean, Coveo, Lucidworks Fusion, Sinequa, Swirl, Sercha, Turing ES, and Apache Solr (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted federated search, open-source enterprise search engines, and community-driven metadata federation—ideal for organizations seeking data sovereignty and avoiding per-user or per-query SaaS pricing. The open-source landscape is genuinely functional: **Swirl** is a purpose-built federated search engine that queries across 100+ sources without moving data , **Sercha** provides a self-hosted team search platform with 11+ connectors and hybrid Vespa-powered ranking , and **Turing ES** delivers a Coveo/Algolia alternative with RAG and AI agents on Solr/Elasticsearch .

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Glean](https://www.glean.com/)** | **The enterprise search and AI assistant standard for tech companies.** 100+ SaaS integrations (Slack, Notion, Confluence, GDrive, SharePoint, Jira, GitHub) with **permission ACL inheritance** enforced at query time. **Glean Assistant** for RAG-based answers. **Valued at $4.6B**, 800+ enterprise customers including Databricks, Webflow, and Reddit . | **~$300/user/year** (Enterprise); Starter tier ~$240/user/year  | No free tier; sales-led |
| **[Coveo](https://www.coveo.com/)** | **Customer support and e-commerce search leader.** Relevance Cloud with native Salesforce/ServiceNow integration and **Coveo for Commerce**. 70+ connectors. **Market cap ~$700M** (TSX:CVO), 2,000+ customers including Xerox, Salesforce, and Tableau . | **$250K–$2M/year** (enterprise)  | No free tier; sales-led |
| **[Lucidworks Fusion](https://www.lucidworks.com/)** | **E-commerce site search and workplace search.** Built on Apache Solr with a commercial control plane. **~$326M valuation**, 400+ customers including Lowe's and REI . | **$100K–$1M/year**  | No free tier; sales-led |
| **[Sinequa](https://www.sinequa.com/)** | **Enterprise search for regulated industries** (pharma, financial services). Strong permission fidelity and compliance features. Deployments typically **$1–3M/year** for large enterprises . | Quote-only (enterprise contract) | No free tier; sales-led |
| **[AWS Kendra](https://aws.amazon.com/kendra/)** | Managed enterprise search with NLP and deep learning. **End of support: no longer open to new customers starting July 30, 2026.** Existing customers can continue using the service . | Base capacity: ~$100.80/month (1,000 queries/day) | **750 hours free for first 30 days**; no new customer signups after July 2026  |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Swirl](https://github.com/swirlai/swirl-search)** | [![Stars](https://img.shields.io/github/stars/swirlai/swirl-search?style=social&color=white)](https://github.com/swirlai/swirl-search/stargazers) | **The most purpose-built open-source federated search engine.** Queries **100+ sources simultaneously without moving data**—results come back from where they live, ranked with cosine similarity and Relevancy. **Sources include** Microsoft (Teams, Outlook, SharePoint, OneDrive), Google, AWS Kendra, BigQuery, Collibra, Elasticsearch, MongoDB, OpenSearch, Oracle, PostgreSQL, Qdrant, Snowflake, Solr, Vespa, Algolia, Confluence, GitHub, HubSpot, Jira, Salesforce, ServiceNow, Slack, and many more . **AI-powered metasearch** adapts queries to each source's API and understands true intent. **Community edition available on Azure Marketplace at $20/month** for private cloud deployment . **Best for organizations wanting true federated search** across heterogeneous silos without centralizing data . |
| **[Sercha](https://github.com/sercha-oss/sercha-core)** | [![Stars](https://img.shields.io/github/stars/sercha-oss/sercha-core?style=social&color=white)](https://github.com/sercha-oss/sercha-core/stargazers) | **Self-hosted team search with hybrid Vespa-powered ranking.** Apache-2.0. **11+ connectors** including GitHub, GitLab, Slack, Notion, Confluence, Jira, Google Drive, Google Docs, Linear, Dropbox, and S3 . **Hybrid search** combining BM25 lexical and semantic embeddings, with query expansion and optional LLM integration (OpenAI or Ollama) . **OAuth2 authentication** (GitHub, Google) and **team management with RBAC**. **Docker Compose quickstart** with pre-built images; requires 4GB+ RAM (Vespa dependency) . **Best for teams wanting a self-hosted unified search layer** across SaaS sources with hybrid ranking . |
| **[Turing ES](https://github.com/openviglet/turing)** | [![Stars](https://img.shields.io/github/stars/openviglet/turing?style=social&color=white)](https://github.com/openviglet/turing/stargazers) | **Open-source enterprise search + generative AI platform—a self-hosted Algolia/Coveo alternative.** **Apache-2.0 with no per-query, per-record, or per-seat metering** . **Multi-engine**: one API over Apache Solr, Elasticsearch, or embedded Apache Lucene—swap without rewriting . **Hybrid ranking**: BM25 keyword + kNN vector retrieval fused with Reciprocal Rank Fusion. **RAG chat with inline source citations**; AI agents with MCP servers. **Connectors** for Adobe AEM, WordPress, databases, filesystem, and web crawls via Viglet Dumont (separate extraction product) . **Runs fully offline** for air-gapped/regulated deployments . **Docker Compose or Kubernetes** deployment . **Best for teams wanting a complete search + AI platform** with zero licensing fees and full data control . |
| **[Apache Solr](https://github.com/apache/solr)** | [![Stars](https://img.shields.io/github/stars/apache/solr?style=social&color=white)](https://github.com/apache/solr/stargazers) | **The foundational open-source enterprise search engine.** Apache-2.0, Apache Software Foundation governance. **Mature faceting, schema control, and streaming expressions** for document and site search. **SolrCloud** uses ZooKeeper for cluster coordination; user-managed mode runs without central coordination . **Vector search** via DenseVectorField with HNSW since Solr 9.0. **Trade-off**: more manual configuration than Elasticsearch—schema.xml and collections define the contract between indexing and relevance tuning . **Best for teams wanting a proven, vendor-independent search foundation** that they operate themselves . |
| **[Elasticsearch](https://github.com/elastic/elasticsearch)** | [![Stars](https://img.shields.io/github/stars/elastic/elasticsearch?style=social&color=white)](https://github.com/elastic/elasticsearch/stargazers) | **The most widely deployed full-text and analytics search server.** **License**: Elastic License 2.0 by default (with free portions under SSPL/AGPLv3); **OpenSearch is the Apache-2.0 fork** . **JSON REST API**, built-in cluster discovery, and **Kibana** for dashboards. **Trade-off**: license terms have shifted historically—verify compatibility for your use case. **Best for teams already in the Elastic ecosystem** or needing log/observability search alongside enterprise content . |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[OpenSearch](https://github.com/opensearch-project/OpenSearch)** | [![Stars](https://img.shields.io/github/stars/opensearch-project/OpenSearch?style=social&color=white)](https://github.com/opensearch-project/OpenSearch/stargazers) | **Apache-2.0 fork of Elasticsearch 7.10.2.** Elasticsearch-compatible REST API with **OpenSearch Dashboards**. **Linux Foundation governance** and AWS-managed service available. **Best for teams wanting Elasticsearch-style APIs without Elastic License restrictions** . |
| **[Vespa](https://github.com/vespa-engine/vespa)** | [![Stars](https://img.shields.io/github/stars/vespa-engine/vespa?style=social&color=white)](https://github.com/vespa-engine/vespa/stargazers) | **Norwegian open-source engine for search, recommendation, and vector serving** with real-time updates. Powers Sercha's semantic search layer. **Best for teams needing low-latency vector and hybrid search** at scale . |
| **[Datafari](https://github.com/francelabs/datafari)** | [![Stars](https://img.shields.io/github/stars/francelabs/datafari?style=social&color=white)](https://github.com/francelabs/datafari/stargazers) | **French open-source enterprise search solution built on Apache Solr** by France Labs. **Best for European organizations prioritizing EU-maintained search software** . |

**Frameworks for building custom systems**: Choose **Swirl** for true federated search across 100+ sources without data movement , **Sercha** for a self-hosted unified search layer with hybrid ranking , or **Turing ES** for a complete search + RAG platform on Solr/Elasticsearch —all without per-user or per-query SaaS fees that compound at enterprise scale.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Federated search platforms query sensitive enterprise data across silos; **permission fidelity is critical**—ensure the search layer inherits source ACLs rather than exposing restricted content to unauthorized users. Glean and Sinequa are specifically noted for enforcing source permissions at query time .
- **AWS Kendra is closing to new customers on July 30, 2026**—do not plan new deployments on it . **Commercial pricing is enterprise-scale and opaque**: Glean runs **~$300/user/year** , Coveo **$250K–$2M/year** , and Lucidworks **$100K–$1M/year** . **Open-source federated search is genuinely viable but requires operational effort**: Swirl is purpose-built for federation without data movement but requires configuring each source connector , Sercha needs Vespa and 4GB+ RAM , and Turing ES requires Java 21+ and Maven for source builds . **Validate whether you need true federated query (Swirl) or a unified index (Sercha, Turing)** before committing.

---

**Made for IT architects, knowledge managers, and organizations building cross-silo search infrastructure.**  
Let's make federated metadata and global search more open, permission-aware, and data-sovereign.
