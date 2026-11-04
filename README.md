# Hi, I'm Parth 👋

### Blockchain Data Engineer

I build data pipelines that turn raw on-chain activity into reliable, analyst-ready data. I started in analytics and reporting, then grew into owning the engineering behind it: decoding EVM event logs, building ETL/ELT pipelines on Azure Databricks, and writing the data-quality and anomaly-detection rules that keep the numbers trustworthy.

Currently a Data Engineer at **Magpie XYZ** (omnichain DeFi protocol), tracking **$50M+ in assets** across Arbitrum, BNB Chain and Ethereum at **99.9% accuracy**.

📍Bannglore, India · 🌍 Open to remote roles globally

---

## 🛠 Core Stack

- **Ingestion & Processing:** PySpark · Spark Structured Streaming · Apache Kafka · Apache Airflow · Azure Data Factory
- **On-chain Decoding:** web3.py · eth-abi · JSON-RPC · proxy ABIs · indexed/non-indexed topics · reorg handling · decimal normalization
- **Storage & Warehousing:** Delta Lake · ADLS Gen2 · BigQuery · Snowflake · Synapse · DuckDB · Parquet · Iceberg
- **Transformation & Quality:** dbt (tests, incremental models, SCD Type 2) · Medallion Architecture · Great Expectations
- **Cloud & DevOps:** Azure (Databricks, ADF, DevOps) · GCP (BigQuery, Cloud Run, Dataflow) · AWS (S3, Glue, Redshift) · Terraform · Docker · GitHub Actions
- **On-chain Analytics:** Dune (Spellbook SQL) · Flipside · Nansen · Arkham · The Graph
- **Dashboards:** Power BI · Dune · Streamlit · Grafana

---

## 🔭 Featured Projects

### [chainproof](https://github.com/parthger/chainproof)

**Reorg-safe ERC-20 indexer that refuses to publish numbers it can't prove against chain state**

Most indexers can produce a number. chainproof proves the number is right before anyone sees it. Each run pulls `Transfer` logs from finalized blocks into a staging table, then runs a zero-tolerance reconciliation gate against the contract's own state: completeness against an independent second RPC, change in `totalSupply` vs mints minus burns, `balanceOf` deltas for 20 holders, canonical block hashes, and decimals. A planted one-unit fault proves the gate can actually fail. Rows are published only if every check passes, in a single transaction that also advances a hash-checked watermark.

- Tested live on USDC across Base, Ethereum and Arbitrum: 129K+ Base transfers (one hour of blocks) reconciled in 35 s with zero divergence
- 30 tests against an in-memory fake chain covering dropped logs, reorgs, wrong decimals and real provider errors
- CI on every push, plus a daily live reconciliation run on all three chains
- Pure Python and DuckDB, public RPCs only, no API keys

`Python` · `DuckDB` · `JSON-RPC` · `pytest` · `GitHub Actions`

<!-- Copy the block above for each new project you publish -->

---

## 💼 Professional Work

Code from my professional roles is private, so here is what that work covers.

**Magpie XYZ** · Data Analyst → Data Engineer · Jan 2024 to Present

- Decode on-chain event logs across Arbitrum, BNB Chain and Ethereum, handling proxy ABIs, indexed and non-indexed topics, and reorg buffers
- PySpark ETL/ELT pipelines ingesting 50K+ daily events from 10+ sources into ADLS Gen2, with 40% faster ingestion and lower compute cost
- Medallion architecture on Delta Lake with dbt models, tests and SCD Type 2, orchestrated through Airflow and ADF with SLA alerts
- Python business rules flagging anomalies across 200K+ monthly transactions
- 15+ dashboards for activity, utilization and asset flows, validated against Flipside, Nansen and Arkham
- CI/CD with Docker, GitHub Actions and Azure DevOps, cutting deployment time by 60%

**Quboid** · Product Analyst & Data Operations · Jan 2023 to Dec 2023

- Python pipelines (Pandas, SQLAlchemy) and Power BI dashboards tracking 10K+ transactions and user funnels
- Onboarded 3 vendor datasets via REST APIs, with data-quality profiling for exception alerts

---

## 📬 Get in Touch

- **Email:** <parthgera49@gmail.com>
