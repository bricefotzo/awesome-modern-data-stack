# Awesome Modern Data Stack [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome tools, frameworks, and resources for the Modern Data Stack (MDS).

The **Modern Data Stack** refers to a collection of cloud-native tools and technologies that work together to help organizations collect, store, transform, and analyze data. This list aims to help data professionals navigate the ever-evolving data ecosystem.

## Contents

- [Data Integration & Ingestion](#data-integration--ingestion)
- [Data Warehouses & Lakehouses](#data-warehouses--lakehouses)
- [Data Lakes & Storage](#data-lakes--storage)
- [Data Transformation](#data-transformation)
- [Data Orchestration](#data-orchestration)
- [Data Quality & Testing](#data-quality--testing)
- [Data Observability](#data-observability)
- [Data Catalog & Discovery](#data-catalog--discovery)
- [Data Governance](#data-governance)
- [Business Intelligence & Analytics](#business-intelligence--analytics)
- [Metrics Layer & Semantic Layer](#metrics-layer--semantic-layer)
- [Reverse ETL](#reverse-etl)
- [Data Contracts](#data-contracts)
- [Streaming & Real-Time](#streaming--real-time)
- [Query Engines](#query-engines)
- [Data Notebooks & Exploration](#data-notebooks--exploration)
- [Feature Stores](#feature-stores)
- [ML Platforms & MLOps](#ml-platforms--mlops)
- [Vector Databases](#vector-databases)
- [Data Privacy & Security](#data-privacy--security)
- [Data Sharing](#data-sharing)
- [DataOps & Version Control](#dataops--version-control)
- [Learning Resources](#learning-resources)
- [Community](#community)

---

## Data Integration & Ingestion

*Tools for extracting data from various sources and loading it into data warehouses or lakes.*

### Open Source

- [Airbyte](https://airbyte.com/) - Open-source data integration platform with 300+ connectors. ELT-first approach.
- [dlt (data load tool)](https://dlthub.com/) - Python library for data loading with automatic schema inference.
- [Singer](https://www.singer.io/) - Open-source standard for writing scripts that move data (taps and targets).
- [Meltano](https://meltano.com/) - Open-source DataOps platform built on Singer. CLI-first, version-controlled pipelines.
- [Ingestr](https://github.com/bruin-data/ingestr) - CLI tool to copy data between databases with a single command.

### Commercial / Managed

- [Boomi](https://boomi.com/) - Modern data integration and agent management platform.
- [Fivetran](https://www.fivetran.com/) - Automated data integration with 500+ connectors. Industry leader in managed ELT.
- [Stitch](https://www.stitchdata.com/) - Simple, extensible ETL built for developers. Part of Talend.
- [Hevo Data](https://hevodata.com/) - No-code data pipeline platform.
- [Informatica](https://www.informatica.com/) - Enterprise data integration and management platform.
- [Talend](https://www.talend.com/) - Enterprise data integration suite.

---

## Data Warehouses & Lakehouses

*Cloud data warehouses and lakehouse platforms for storing and querying analytical data.*

### Cloud Data Warehouses

- [Snowflake](https://www.snowflake.com/) - Cloud-native data warehouse with separation of storage and compute.
- [Google BigQuery](https://cloud.google.com/bigquery) - Serverless, highly scalable data warehouse by Google.
- [Amazon Redshift](https://aws.amazon.com/redshift/) - Fast, scalable data warehouse by AWS.
- [Azure Synapse Analytics](https://azure.microsoft.com/en-us/products/synapse-analytics/) - Limitless analytics service by Microsoft.
- [Databricks SQL](https://www.databricks.com/product/databricks-sql) - Serverless SQL analytics on the Lakehouse.
- [Firebolt](https://www.firebolt.io/) - Cloud data warehouse built for high-performance analytics.
- [ClickHouse Cloud](https://clickhouse.com/cloud) - Managed ClickHouse for real-time analytics.
- [StarRocks](https://www.starrocks.io/) - High-performance analytical database.
- [MotherDuck](https://motherduck.com/) - Serverless analytics powered by DuckDB.

### Lakehouse Platforms

- [Databricks](https://www.databricks.com/) - Unified analytics platform combining data lake and warehouse.
- [Apache Iceberg](https://iceberg.apache.org/) - Open table format for huge analytic datasets.
- [Delta Lake](https://delta.io/) - Open-source storage layer with ACID transactions on data lakes.
- [Apache Hudi](https://hudi.apache.org/) - Data lake platform for incremental data processing.
- [Dremio](https://www.dremio.com/) - Lakehouse platform with Apache Iceberg support.
- [Onehouse](https://www.onehouse.ai/) - Managed lakehouse platform built on Apache Hudi.
- [Tabular](https://tabular.io/) - Managed Apache Iceberg service by its creators.

---

## Data Lakes & Storage

*Object storage and data lake solutions for storing raw and processed data.*

### Object Storage

- [Amazon S3](https://aws.amazon.com/s3/) - Industry-standard object storage by AWS.
- [Google Cloud Storage](https://cloud.google.com/storage) - Object storage by Google Cloud.
- [Azure Blob Storage](https://azure.microsoft.com/en-us/products/storage/blobs/) - Object storage by Microsoft Azure.
- [MinIO](https://min.io/) - High-performance, S3-compatible object storage.
- [Cloudflare R2](https://www.cloudflare.com/products/r2/) - S3-compatible storage with zero egress fees.

### Data Lake Formats

- [Apache Parquet](https://parquet.apache.org/) - Columnar storage file format.
- [Apache ORC](https://orc.apache.org/) - Columnar storage format for Hadoop.
- [Apache Avro](https://avro.apache.org/) - Row-based data serialization format.
- [Lance](https://github.com/lancedb/lance) - Modern columnar format for ML datasets.

---

## Data Transformation

*Tools for transforming, modeling, and preparing data for analysis.*

### SQL-Based Transformation

- [dbt (data build tool)](https://www.getdbt.com/) - Industry-standard SQL-first transformation tool. Version-controlled, tested, documented.
- [SQLMesh](https://sqlmesh.com/) - Data transformation framework with built-in data quality and CI/CD.
- [SDF (Semantic Data Fabric)](https://www.sdf.com/) - SQL compiler for data transformation with static analysis.
- [Coalesce](https://coalesce.io/) - Data transformation platform purpose-built for Snowflake.
- [Dataform](https://dataform.co/) - SQL-based data transformation (acquired by Google).

### Python-Based Transformation

- [Pandas](https://pandas.pydata.org/) - Data manipulation and analysis library for Python.
- [Polars](https://www.pola.rs/) - Lightning-fast DataFrame library written in Rust.
- [DuckDB](https://duckdb.org/) - In-process SQL OLAP database. Perfect for local data transformation.
- [PySpark](https://spark.apache.org/docs/latest/api/python/) - Python API for Apache Spark.
- [Vaex](https://vaex.io/) - Out-of-core DataFrames for large datasets.
- [Modin](https://modin.readthedocs.io/) - Parallel pandas using Ray or Dask.
- [Ibis](https://ibis-project.org/) - Python DataFrame API that compiles to SQL.
- [Fugue](https://fugue-tutorials.readthedocs.io/) - Unified interface for distributed computing.
- [Hamilton](https://github.com/dagworks-inc/hamilton) - Micro-framework for dataframe generation.

### Distributed Computing

- [Apache Spark](https://spark.apache.org/) - Unified analytics engine for large-scale data processing.
- [Dask](https://www.dask.org/) - Flexible parallel computing library for analytics.
- [Ray](https://www.ray.io/) - Unified framework for scaling AI and Python applications.
- [Apache Flink](https://flink.apache.org/) - Stream and batch processing framework.
- [Apache Beam](https://beam.apache.org/) - Unified programming model for batch and streaming.
- [Asgarde](https://github.com/tosun-si/asgarde) - Java library for simplified error handling in Beam pipelines.

---

## Data Orchestration

*Tools for scheduling, monitoring, and managing data pipelines and workflows.*

### Open Source

- [Apache Airflow](https://airflow.apache.org/) - Platform to programmatically author, schedule, and monitor workflows.
- [Dagster](https://dagster.io/) - Cloud-native orchestration platform with software-defined assets.
- [Prefect](https://www.prefect.io/) - Modern workflow orchestration with Python-native approach.
- [Mage](https://www.mage.ai/) - Open-source data pipeline tool with notebook-style interface.
- [Kestra](https://kestra.io/) - Event-driven orchestration platform with declarative YAML.
- [Luigi](https://github.com/spotify/luigi) - Python module for building complex pipelines (by Spotify).
- [Argo Workflows](https://argoproj.github.io/argo-workflows/) - Kubernetes-native workflow engine.

### Commercial / Managed

- [Astronomer](https://www.astronomer.io/) - Managed Airflow platform.
- [Dagster Cloud](https://dagster.io/cloud) - Managed Dagster platform.
- [Prefect Cloud](https://www.prefect.io/cloud) - Managed Prefect platform.
- [Google Cloud Composer](https://cloud.google.com/composer) - Managed Apache Airflow by Google.
- [Amazon MWAA](https://aws.amazon.com/managed-workflows-for-apache-airflow/) - Managed Airflow by AWS.
- [Azure Data Factory](https://azure.microsoft.com/en-us/products/data-factory/) - Cloud-based data integration service.
- [Orchestra](https://www.getorchestra.io/) - Unified data orchestration platform.

---

## Data Quality & Testing

*Tools for ensuring data accuracy, completeness, and reliability.*

### Open Source

- [Great Expectations](https://greatexpectations.io/) - Python library for data validation and documentation.
- [dbt Tests](https://docs.getdbt.com/docs/build/tests) - Built-in testing framework in dbt.
- [Elementary](https://www.elementary-data.com/) - Open-source data observability for dbt.


### Commercial / Managed

- [Soda](https://www.soda.io/) - Data quality platform with SodaCL language.
- [Monte Carlo](https://www.montecarlodata.com/) - Data observability platform with ML-powered anomaly detection.

---

## Data Observability

*Tools for monitoring, alerting, and understanding data pipeline health.*

- [Datadog](https://www.datadoghq.com/) - Monitoring and security platform for developers.
- [Elementary](https://www.elementary-data.com/) - Open-source dbt-native data observability.
- [Datafold](https://www.datafold.com/) - Data reliability platform with data diff and regression testing.
- [Sifflet](https://www.siffletdata.com/) - Full-stack data observability platform.

---

## Data Catalog & Discovery

*Tools for discovering, understanding, and documenting data assets.*

### Open Source

- [DataHub](https://datahubproject.io/) - Open-source metadata platform by LinkedIn.
- [Amundsen](https://www.amundsen.io/) - Open-source data discovery platform by Lyft.
- [OpenMetadata](https://open-metadata.org/) - Open-source metadata platform with discovery and governance.


### Commercial / Managed

- [Atlan](https://atlan.com/) - Active metadata platform with collaboration features.
- [Alation](https://www.alation.com/) - Enterprise data intelligence platform.
- [Collibra](https://www.collibra.com/) - Data intelligence platform with governance and catalog.

---

## Data Governance

*Tools for managing data policies, access, compliance, and security.*

- [Collibra](https://www.collibra.com/) - Comprehensive data governance platform.
- [Alation](https://www.alation.com/) - Data catalog with governance capabilities.

---

## Business Intelligence & Analytics

*Tools for data visualization, reporting, and self-service analytics.*

### Open Source

- [Apache Superset](https://superset.apache.org/) - Modern data exploration and visualization platform.
- [Metabase](https://www.metabase.com/) - Open-source business intelligence with SQL and visual query builder.
- [Redash](https://redash.io/) - Connect and query data sources, build dashboards.
- [Lightdash](https://www.lightdash.com/) - Open-source BI for dbt users.
- [Evidence](https://evidence.dev/) - Code-based BI with Markdown and SQL.
- [Grafana](https://grafana.com/) - Open-source analytics and monitoring platform.

### Commercial / Managed

- [Looker](https://looker.com/) - Enterprise BI with semantic modeling (Google Cloud).
- [Tableau](https://www.tableau.com/) - Visual analytics platform (Salesforce).
- [Power BI](https://powerbi.microsoft.com/) - Business analytics by Microsoft.
- [Qlik](https://www.qlik.com/) - Data analytics and business intelligence platform.
- [Preset](https://preset.io/) - Managed Apache Superset.
- [Omni](https://omni.co/) - Shared-model BI platform.
- [Holistics](https://www.holistics.io/) - Self-service BI platform with data modeling.


---

## Metrics Layer & Semantic Layer

*Tools for defining consistent business metrics and semantic models.*

- [dbt Semantic Layer](https://www.getdbt.com/product/semantic-layer) - Define metrics in dbt, query from any tool.
- [Cube](https://cube.dev/) - Headless BI and semantic layer with caching.
- [MetricFlow](https://github.com/dbt-labs/metricflow) - Semantic layer engine (now part of dbt).
- [Looker](https://looker.com/) - LookML semantic modeling language.
- [Transform (Acquired by dbt Labs)](https://transform.co/) - Metrics store platform.
- [Minerva (Airbnb)](https://medium.com/airbnb-engineering/how-airbnb-achieved-metric-consistency-at-scale-f23cc53dea70) - Airbnb's internal metrics platform.


---

## Reverse ETL

*Tools for syncing data from warehouses back to operational tools.*

- [Census](https://www.getcensus.com/) - Operational analytics platform for syncing data to business tools.
- [Hightouch](https://hightouch.com/) - Data activation platform for reverse ETL.
- [Polytomic](https://www.polytomic.com/) - Sync data bidirectionally between databases and SaaS.

---

## Data Contracts

*Tools and frameworks for defining and enforcing data contracts between producers and consumers.*

- [Soda Data Contracts](https://www.soda.io/data-contracts) - Define and verify data contracts.
- [Bitol](https://bitol.io/) - Open-source data contract specification.
- [DataContract CLI](https://github.com/datacontract/datacontract-cli) - CLI for managing data contracts.
- [Great Expectations](https://greatexpectations.io/) - Can be used for contract-like validations.
- [JSON Schema](https://json-schema.org/) - Schema specification for JSON data.
- [Protobuf](https://protobuf.dev/) - Protocol Buffers for schema definition.
- [Apache Avro](https://avro.apache.org/) - Data serialization with schema evolution.

---

## Streaming & Real-Time

*Tools for real-time data processing and event streaming.*

### Message Brokers & Streaming Platforms

- [Apache Kafka](https://kafka.apache.org/) - Distributed event streaming platform.
- [Confluent](https://www.confluent.io/) - Enterprise Kafka platform with managed cloud.
- [Amazon Kinesis](https://aws.amazon.com/kinesis/) - Real-time streaming data service by AWS.
- [Google Pub/Sub](https://cloud.google.com/pubsub) - Messaging service by Google Cloud.
- [Azure Event Hubs](https://azure.microsoft.com/en-us/products/event-hubs/) - Big data streaming platform by Azure.
- [RabbitMQ](https://www.rabbitmq.com/) - Open-source message broker.


### Stream Processing

- [Apache Flink](https://flink.apache.org/) - Stateful stream processing framework.
- [Apache Kafka Streams](https://kafka.apache.org/documentation/streams/) - Client library for stream processing.
- [ksqlDB](https://ksqldb.io/) - Database for stream processing on Kafka.
- [Apache Spark Streaming](https://spark.apache.org/streaming/) - Spark module for stream processing.


### Change Data Capture (CDC)

- [Boomi Data Integration](https://boomi.com/platform/boomi-data-integration/) - Automated CDC for operational databases and apps.
- [Debezium](https://debezium.io/) - Open-source distributed CDC platform.
- [Airbyte CDC](https://airbyte.com/connectors?category=cdc) - CDC connectors in Airbyte.
- [Fivetran CDC](https://www.fivetran.com/solutions/change-data-capture) - Managed CDC by Fivetran.

---

## Query Engines

*Distributed SQL query engines for data lakes and federated queries.*

- [PrestoDB](https://prestodb.io/) - Distributed SQL query engine by Meta.
- [Apache Drill](https://drill.apache.org/) - Schema-free SQL query engine.
- [Apache Impala](https://impala.apache.org/) - Massively parallel SQL query engine.
- [DuckDB](https://duckdb.org/) - In-process analytical database.
- [ClickHouse](https://clickhouse.com/) - Column-oriented DBMS for OLAP.
- [Apache Druid](https://druid.apache.org/) - Real-time analytics database.

---

## Data Notebooks & Exploration

*Interactive environments for data exploration and analysis.*

### Open Source

- [Jupyter](https://jupyter.org/) - Web-based interactive computing platform.
- [JupyterLab](https://jupyterlab.readthedocs.io/) - Next-generation Jupyter interface.
- [Zeppelin](https://zeppelin.apache.org/) - Web-based notebook for data analytics.
- [Marimo](https://marimo.io/) - Reactive Python notebook with reproducibility.
- [Streamlit](https://streamlit.io/) - Python framework for data apps.

### Commercial / Managed

- [Google Colab](https://colab.research.google.com/) - Free Jupyter notebooks by Google.
- [Amazon SageMaker Studio](https://aws.amazon.com/sagemaker/studio/) - ML IDE by AWS.
- [Databricks Notebooks](https://www.databricks.com/) - Collaborative notebooks on Databricks.
- [Hex](https://hex.tech/) - Collaborative data workspace with notebooks and apps.
- [Deepnote](https://deepnote.com/) - Collaborative data notebook for teams.

---

## Feature Stores

*Platforms for managing, storing, and serving ML features.*

- [Vertex AI Feature Store](https://cloud.google.com/vertex-ai/docs/featurestore) - Google Cloud feature store.
- [Amazon SageMaker Feature Store](https://aws.amazon.com/sagemaker/feature-store/) - AWS managed feature store.
- [Databricks Feature Store](https://www.databricks.com/product/feature-store) - Feature store in Databricks.
- [Feast](https://feast.dev/) - Open-source feature store for ML.
- [Hopsworks](https://www.hopsworks.ai/) - Platform with feature store and MLOps.





---

## ML Platforms & MLOps

*End-to-end platforms for building, deploying, and managing ML models.*

### Open Source

- [MLflow](https://mlflow.org/) - Open-source platform for ML lifecycle management.
- [Kubeflow](https://www.kubeflow.org/) - ML toolkit for Kubernetes.
- [Metaflow](https://metaflow.org/) - Framework for real-life data science (by Netflix).
- [ZenML](https://zenml.io/) - MLOps framework for reproducible pipelines.


### Commercial / Managed

- [Google Vertex AI](https://cloud.google.com/vertex-ai) - Unified ML platform by Google Cloud.
- [Databricks MLflow](https://www.databricks.com/product/managed-mlflow) - Managed MLflow on Databricks.
- [Amazon SageMaker](https://aws.amazon.com/sagemaker/) - Fully managed ML service by AWS.
- [Azure Machine Learning](https://azure.microsoft.com/en-us/products/machine-learning/) - ML platform by Microsoft.
- [Weights & Biases](https://wandb.ai/) - ML experiment tracking and model management.

---

## Vector Databases

*Databases optimized for storing and querying vector embeddings for AI/ML applications.*

- [MongoDB](https://www.mongodb.com/docs/atlas/atlas-vector-search/vector-search-overview/) - Managed vector store alognside your operational data in MongoDB Atlas.
- [Pinecone](https://www.pinecone.io/) - Managed vector database for similarity search.
- [Weaviate](https://weaviate.io/) - Open-source vector search engine.
- [Qdrant](https://qdrant.tech/) - Open-source vector similarity search engine.
- [Chroma](https://www.trychroma.com/) - Open-source embedding database.
- [pgvector](https://github.com/pgvector/pgvector) - Vector similarity search for PostgreSQL.
- [Elasticsearch](https://www.elastic.co/) - Search engine with vector search capabilities.



---

## Data Sharing

*Platforms for securely sharing data across organizations.*

- [Google Analytics Hub](https://cloud.google.com/analytics-hub) - Data exchange by Google Cloud.
- [Snowflake Data Marketplace](https://www.snowflake.com/data-marketplace/) - Data sharing and marketplace by Snowflake.
- [Databricks Delta Sharing](https://www.databricks.com/product/delta-sharing) - Open protocol for secure data sharing.
- [AWS Data Exchange](https://aws.amazon.com/data-exchange/) - Data marketplace by AWS.


---

## DataOps & Version Control

*Tools for DataOps practices, version control, and CI/CD for data.*

- [dbt](https://www.getdbt.com/) - Version-controlled data transformation.
- [DVC](https://dvc.org/) - Version control for data and ML models.

---

## Learning Resources

### Books

- [Fundamentals of Data Engineering](https://www.oreilly.com/library/view/fundamentals-of-data/9781098108298/) - by Joe Reis & Matt Housley
- [The Data Warehouse Toolkit](https://www.kimballgroup.com/data-warehouse-business-intelligence-resources/books/) - by Ralph Kimball
- [Designing Data-Intensive Applications](https://dataintensive.net/) - by Martin Kleppmann
- [Data Mesh](https://www.oreilly.com/library/view/data-mesh/9781492092384/) - by Zhamak Dehghani
- [Building a Scalable Data Warehouse with Data Vault 2.0](https://www.elsevier.com/books/building-a-scalable-data-warehouse-with-data-vault-20/linstedt/978-0-12-802510-9) - by Dan Linstedt

### Courses & Certifications

- [dbt Learn](https://courses.getdbt.com/) - Free dbt fundamentals course.
- [DataCamp](https://www.datacamp.com/) - Data science and engineering courses.
- [DataTalks.Club](https://datatalks.club/) - Free data engineering zoomcamp.
- [Coursera Data Engineering](https://www.coursera.org/professional-certificates/google-cloud-data-engineering) - Google Cloud Data Engineering certificate.
- [Snowflake Training](https://www.snowflake.com/education-and-training/) - Snowflake certifications.
- [Databricks Training](https://www.databricks.com/learn/training) - Databricks certifications.

### Blogs & Newsletters


- [Blef.fr](https://www.blef.fr/) - The hub to explore Data News links.
- [Joe Reis's Substack](https://joereis.substack.com/) - Insights on data engineering.
- [dbt Blog](https://www.getdbt.com/blog/) - Articles on analytics engineering.
- [Airbyte Blog](https://airbyte.com/blog) - Data integration and engineering content.

### Podcasts

- [DataGen](https://open.spotify.com/show/27XP61URSuKu9oeWR793D6) - Interviews with French data practitioners & leaders.
- [The Data Engineering Podcast](https://www.dataengineeringpodcast.com/) - Interviews with data engineering practitioners.
- [Data Engineering Show](https://www.dataengineeringshow.com/) - Discussions on data engineering topics.


---

## Community

### Slack Communities

- [dbt Community Slack](https://www.getdbt.com/community/) - 50k+ members discussing analytics engineering.
- [Airbyte Slack](https://airbyte.com/community) - Data integration community.
- [Apache Airflow Slack](https://apache-airflow.slack.com/) - Workflow orchestration.

### Conferences


- [Coalesce](https://coalesce.getdbt.com/) - dbt's annual conference.
- [Snowflake Summit](https://www.snowflake.com/summit/) - Snowflake user conference.

> Comming soon...
### Community Resources

- [r/dataengineering](https://www.reddit.com/r/dataengineering/) - Reddit community.
- [Data Engineering Wiki](https://dataengineering.wiki/) - Community-maintained wiki.
- [Awesome Data Engineering](https://github.com/igorbarinov/awesome-data-engineering) - Another curated list.
- [Modern Data Stack Glossary](https://www.secoda.co/glossary) - Data terminology.

---

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related or neighboring rights to this work.

---

## Acknowledgments

This list is maintained by the community. Special thanks to all contributors who help keep it up-to-date.

If you find this resource helpful, please give it a star and share it with others!
