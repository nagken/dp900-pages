# DP-900 Glossary

| Term | Definition |
|---|---|
| **Structured data** | Fixed schema rows + columns. |
| **Semi-structured data** | Schema-on-read; JSON / XML / Avro / Parquet. |
| **Unstructured data** | No internal schema; text / images / video. |
| **OLTP** | Online Transaction Processing - many small writes. |
| **OLAP** | Online Analytical Processing - few large reads. |
| **Normalization** | Removing redundancy via 1NF/2NF/3NF. |
| **Primary key** | Unique row identifier. |
| **Foreign key** | Reference to another table's primary key. |
| **Index** | Lookup acceleration structure. |
| **View** | Saved query treated as a table. |
| **Azure SQL DB** | PaaS single-database. |
| **Azure SQL MI** | PaaS instance with high SQL Server compat. |
| **SQL on VM** | IaaS SQL Server on Azure VM. |
| **Azure DB for PostgreSQL** | PaaS Postgres. |
| **Azure DB for MySQL** | PaaS MySQL. |
| **Cosmos DB** | Globally distributed multi-model NoSQL DB. |
| **Cosmos NoSQL API** | Native JSON document API. |
| **Consistency level** | Read guarantee strength: strong .. eventual. |
| **Blob storage** | Object store; tiers Hot/Cool/Cold/Archive. |
| **ADLS Gen2** | Blob storage + hierarchical namespace + ACLs. |
| **Azure Files** | Managed SMB / NFS share. |
| **Queue storage** | Simple async messaging. |
| **Table storage** | Cheap key-value NoSQL rows. |
| **ETL** | Extract -> Transform -> Load (transform external). |
| **ELT** | Extract -> Load -> Transform (transform in target). |
| **Microsoft Fabric** | SaaS unified analytics: OneLake + Lakehouse + Warehouse + RTI + Power BI. |
| **OneLake** | Single tenant-wide data lake in Fabric. |
| **Lakehouse** | Combined data lake + warehouse semantics. |
| **Warehouse** | MPP SQL endpoint over OneLake. |
| **Direct Lake** | Power BI mode that reads OneLake parquet directly. |
| **Synapse Analytics** | Azure analytics service (dedicated SQL pool, Spark). |
| **Databricks** | Spark-based unified analytics platform. |
| **Data Factory** | Code-free pipeline / orchestration service. |
| **Stream Analytics** | Managed real-time SQL over streams. |
| **Event Hubs** | High-throughput event ingestion. |
| **IoT Hub** | Event Hubs + device registry + cloud-to-device messaging. |
| **Real-Time Intelligence** | Fabric KQL DB + Eventstream + Real-Time Dashboard. |
| **Power BI workspace** | Collaboration container. |
| **Semantic model (dataset)** | Power BI data + measures + relationships. |
| **Report** | Pages of visuals authored in Desktop / Service. |
| **Dashboard** | Pinned-tile single-page monitoring view in Service. |
| **Paginated report** | Pixel-perfect printable report (Report Builder). |

---

[Master Index](00-MASTER-INDEX.md)
