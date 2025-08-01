# 🧠 Big Data Pipeline

This repository integrates multiple modular components of a production-grade big data analytics system, including ingestion, processing, warehousing, transformation, and caching layers.

---

## 📦 Modules Overview

| Module                         | Description                                                                 |
|--------------------------------|-----------------------------------------------------------------------------|
| [nifi-setup](./modules/nifi-setup)                       | Ingestion pipeline using Apache NiFi to fetch and load external data.      |
| [spark-jobs](./modules/spark-jobs)                       | PySpark jobs to clean, process, and ingest data into Hudi tables.          |
| [hive-metastore-setup](./modules/hive-metastore-setup)   | Standalone Hive Metastore with PostgreSQL backend for unified table schema.|
| [trino-config](./modules/trino-config)                   | Trino query engine configured for querying HDFS/Hive and federated sources.|
| [ignite-cache](./modules/ignite-cache)                   | Apache Ignite as SQL cache to accelerate queries from Trino.               |
| [dbt-transformation](./modules/dbt-transformation)       | dbt models for schema transformation, enrichment, and pushing to Ignite.   |

---

## 🛠️ Clone All Modules

```bash
git clone https://github.com/Strikersid07/nifi-setup.git modules/nifi-setup
git clone https://github.com/Strikersid07/spark-jobs.git modules/spark-jobs
git clone https://github.com/Strikersid07/hive-metastore-setup.git modules/hive-metastore-setup
git clone https://github.com/Strikersid07/trino-config.git modules/trino-config
git clone https://github.com/Strikersid07/ignite-cache.git modules/ignite-cache
git clone https://github.com/Strikersid07/dbt-transformation.git modules/dbt-transformation
