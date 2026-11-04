# Hi, I'm Parth 👋

### Blockchain Data Engineer

I build data pipelines that turn raw on-chain activity into reliable, analyst-ready data. I started in analytics and reporting, then grew into owning the engineering behind it: decoding EVM event logs, building ETL/ELT pipelines on Azure Databricks, and writing the data-quality and anomaly-detection rules that keep the numbers trustworthy.

Currently a Data Engineer at **Magpie XYZ** (omnichain DeFi protocol), tracking **$50M+ in assets** across Arbitrum, BNB Chain and Ethereum at **99.9% accuracy**.

📍 Chandigarh, India · 🌍 Open to remote roles globally

---

## 🛠 Core Stack

- **Ingestion & Processing:** PySpark · Spark Structured Streaming · Apache Kafka · Apache Airflow · Azure Data Factory
- **On-chain Decoding:** web3.py · eth-abi · proxy ABIs · indexed/non-indexed topics · reorg buffers · decimal normalization
- **Storage & Warehousing:** Delta Lake · ADLS Gen2 · BigQuery · Snowflake · Synapse · Parquet · Iceberg
- **Transformation & Quality:** dbt (tests, incremental models, SCD Type 2) · Medallion Architecture · Great Expectations
- **Cloud & DevOps:** Azure (Databricks, ADF, DevOps) · GCP (BigQuery, Cloud Run, Dataflow) · AWS (S3, Glue, Redshift) · Terraform · Docker · GitHub Actions
- **On-chain Analytics:** Dune (Spellbook SQL) · Flipside · Nansen · Arkham · The Graph
- **Dashboards:** Power BI · Dune · Streamlit · Grafana

---

## 🔭 Featured Projects

### [onchain-flows-gcp](https://github.com/parthger/onchain-flows-gcp)

**Multi-chain stablecoin flow tracker on GCP**

Tracks USDC and USDT flows using Google's public Ethereum dataset (`bigquery-public-data.crypto_ethereum`). Transfer events are decoded with BigQuery JavaScript UDFs and decimal-normalized at the silver layer. A canonical schema aggregates daily net flows by address category (CEX, bridge, contract, EOA), and every run is reconciled against each token's `totalSupply()` to catch data-quality drift. Results are served as a Streamlit dashboard on Cloud Run.

`BigQuery` · `JS UDFs` · `Medallion Architecture` · `Streamlit` · `Cloud Run`

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
