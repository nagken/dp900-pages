# DP-900 - Azure Data Fundamentals - Visual Study Guide

> Concept-only study aid. No exam questions reproduced. Source PDF (if any) stays local + gitignored.

**Skills outline:** https://learn.microsoft.com/credentials/certifications/resources/study-guides/dp-900

> [!NOTE]
> DP-900 is a **fundamentals** exam. Focus on concepts and Azure service mapping - not deep T-SQL or KQL syntax.

## Master mind map

```mermaid
mindmap
  root((DP-900))
    Core data concepts
      Data types
        Structured
        Semi-structured
        Unstructured
      Workloads
        Transactional OLTP
        Analytical OLAP
      Roles
        Database admin
        Data engineer
        Data analyst
      Visualization
        Reports
        Dashboards
    Relational on Azure
      Services
        Azure SQL DB
        Azure SQL MI
        SQL on VM
        Azure Database for PostgreSQL
        Azure Database for MySQL
      Tasks
        Provision
        Connect
        Query with T-SQL
      Tools
        SSMS
        Azure Data Studio
        sqlcmd
    Non-relational on Azure
      Services
        Cosmos DB
          NoSQL
          MongoDB
          Cassandra
          Gremlin
          Table
        Table storage
        Blob storage
        File storage
      Capabilities
        Multi-region writes
        Consistency levels
    Analytics workload
      Modern data warehouse
      ELT vs ETL
      Services
        Microsoft Fabric
        Synapse Analytics
        Databricks
        Data Factory
        Stream Analytics
        Event Hubs
        Power BI
      Real-time
        Streaming ingestion
        Hot path
        Cold path
```

## Domain map

```mermaid
flowchart LR
    Master["DP-900 Master Index"]
    D01["Core data concepts"]
    Master --> D01
    D02["Relational data on Azure"]
    Master --> D02
    D03["Non-relational data on Azure"]
    Master --> D03
    D04["Analytics workload on Azure"]
    Master --> D04
```

## Domain weights

```mermaid
pie showData
    title DP-900 domain weights
    "Core data concepts" : 28
    "Relational on Azure" : 22
    "Non-relational on Azure" : 18
    "Analytics workload" : 32
```

## Recommended study order

```mermaid
gantt
    title Suggested study plan
    dateFormat X
    axisFormat Day %d
    section Plan
    Core concepts          :t1, 0, 2d
    Relational on Azure    :t2, after t1, 2d
    Non-relational         :t3, after t2, 2d
    Analytics              :t4, after t3, 2d
    Cheatsheet review      :t5, after t4, 1d
```

---

**Next:** open [01-core-data-concepts.md](01-core-data-concepts.md)
