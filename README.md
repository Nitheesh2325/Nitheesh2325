# Nitheesh Chanambatla

### Data Engineer | Cloud Data Engineering

Dayton, Ohio · Open to Data Engineering opportunities

I build reproducible data pipelines, analytical warehouses, validation systems,
and geospatial event-processing workflows. My projects emphasize clear data
contracts, repeat-safe execution, measurable reconciliation, and limitations
that can be explained directly from the implementation.

## Engineering focus

- Batch and event data processing with Python, Pandas, and Apache Spark
- Dimensional modelling, SCD Type 2, and analytical SQL
- Data validation, reconciliation, quarantine, and idempotency
- PostgreSQL/PostGIS and local analytical storage
- Reproducible testing and GitHub Actions
- AWS infrastructure design and local validation without deployment claims

## Featured systems

### 1. [NASA Earth Observation Event Intelligence Platform](https://github.com/Nitheesh2325/nasa-earth-observation-event-platform) — Flagship

Geospatial event-processing platform built around NASA FIRMS data and verified
locally with **1,000,000 replay events** using Spark and PostgreSQL/PostGIS. The
measured Spark batch completed in **149.502 seconds** at **6,688.88
events/second**, with PostgreSQL/PostGIS validation passing at one million rows.

AWS infrastructure is designed and locally validated, not deployed. A separate
10-million-event experiment verified deterministic generation and independent
read-back; Spark processing at that scale did not complete because of local JVM
memory limits. GitHub Actions passed.

### 2. [Customer360 Analytics Warehouse](https://github.com/Nitheesh2325/customer-360-analytics-warehouse) — Supporting

PostgreSQL dimensional warehouse verified with **400,000 sales facts** and
**25,000 customers**. It implements customer and product SCD Type 2 processing,
surrogate-key resolution, validation and rejected-record quarantine,
repeat-safe loading, and **20 executed analytical SQL queries**. Automated tests
and hosted CI passed.

Facts resolve the dimension version current at load time; event-time historical
attribution is not implemented.

### 3. [RetailSync Data Platform](https://github.com/Nitheesh2325/retailsync-data-platform) — Supporting

Deterministic local **100,000-order** batch pipeline with Pandas validation,
rejected-record persistence, transactional SQLite snapshot replacement,
rerun reconciliation, three analytical SQL queries, chart generation, and
logging. Six automated tests passed; hosted CI uses a 1,000-row full-pipeline
fixture.

Full-snapshot local batch processing—not incremental ingestion, CDC, streaming,
cloud orchestration, or production deployment.

## Technical toolkit

- **Languages:** Python, SQL
- **Processing:** Apache Spark, Pandas
- **Databases:** PostgreSQL, PostGIS, SQLite
- **Data engineering:** ETL, dimensional modelling, SCD Type 2, data-quality validation, reconciliation, idempotency
- **Engineering tools:** Git, GitHub Actions, Docker
- **Cloud:** AWS infrastructure design and local validation

## Engineering principles

- Evidence before claims and measurable validation before scale statements
- Reproducible execution with explicit data contracts and rerun behavior
- Reconciliation and failure handling treated as part of the pipeline
- Honest limitations and tradeoffs documented beside the implementation

## Contact

- [LinkedIn](https://www.linkedin.com/in/nitheesh2325/)
- [nitheeshc2325@gmail.com](mailto:nitheeshc2325@gmail.com)
- Open to Data Engineering opportunities
