# DP-900 Exam Decision Reference

> Wording -> service. Use during last-minute review.

## Data types

| Wording | Pick |
|---|---|
| "rows and columns, fixed schema" | Structured |
| "JSON / XML / Avro / Parquet" | Semi-structured |
| "PDF / images / video / raw text" | Unstructured |

## Workloads

| Wording | Pick |
|---|---|
| "many small transactions per second" | OLTP |
| "aggregate millions of rows for trends" | OLAP |
| "live ops monitoring tiles" | Power BI dashboard |
| "pixel-perfect printable doc" | Power BI paginated report |

## Roles

| Wording | Pick |
|---|---|
| "tunes indexes and runs backups" | Database administrator |
| "builds pipelines into the lake" | Data engineer |
| "creates reports and KPIs" | Data analyst |

## Relational services

| Wording | Pick |
|---|---|
| "cloud-native single DB" | Azure SQL Database |
| "lift-and-shift with cross-DB queries" | Azure SQL Managed Instance |
| "needs OS-level access" | SQL Server on Azure VM |
| "open-source Postgres" | Azure Database for PostgreSQL |
| "open-source MySQL" | Azure Database for MySQL |

## Cosmos DB API

| Wording | Pick |
|---|---|
| "globally distributed JSON" | NoSQL API |
| "existing MongoDB app" | MongoDB API |
| "Cassandra workload" | Cassandra API |
| "graph traversal" | Gremlin API |
| "drop-in for Azure Table" | Table API |
| "sharded Postgres" | PostgreSQL API |

## Consistency

| Wording | Pick |
|---|---|
| "linearizable, single region writes" | Strong |
| "lag bounded by K or time" | Bounded staleness |
| "default, read-your-own-writes" | Session |
| "no out-of-order, otherwise relaxed" | Consistent prefix |
| "lowest latency, no order" | Eventual |

## Storage

| Wording | Pick |
|---|---|
| "blobs, parquet, large files" | Blob storage (ADLS Gen2 if hierarchical) |
| "SMB/NFS share" | Azure Files |
| "small async messages" | Queue storage |
| "simple key-value rows" | Table storage / Cosmos Table API |
| "rarely accessed, restore in hours OK" | Archive tier |

## Analytics

| Wording | Pick |
|---|---|
| "all-in-one SaaS analytics" | Microsoft Fabric |
| "open-source Spark" | Azure Databricks |
| "MPP SQL warehouse" | Fabric Warehouse / Synapse dedicated SQL |
| "code-free ELT pipelines" | Data Factory / Fabric Data Factory |
| "stream ingest at scale" | Event Hubs / IoT Hub / Eventstream |
| "real-time SQL over streams" | Stream Analytics / Fabric KQL DB |
| "BI reports and KPIs" | Power BI |

## Common gotchas

- ELT (modern) leverages target's compute; ETL is older.
- Direct Lake reads parquet only inside OneLake.
- Dashboard != report in Power BI - exam tests the distinction.
- Cosmos Strong consistency forbids multi-region writes.
- Archive tier rehydration takes hours.
- Managed Instance, not Azure SQL DB, supports cross-DB queries / SQL Agent.
- Table storage is legacy - new workloads should use Cosmos Table API.

---

[Master Index](00-MASTER-INDEX.md)
