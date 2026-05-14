# DP-900 Hands-On Labs

> Free / sandbox-friendly exercises.

## Lab 1: Provision Azure SQL DB and run T-SQL

1. Create a free Azure SQL Database.
2. Open Azure Data Studio -> connect using Microsoft Entra ID.
3. Run `SELECT`, `INSERT`, `JOIN` over `AdventureWorksLT`.

## Lab 2: Cosmos DB NoSQL API

1. Create a Cosmos DB account (NoSQL API).
2. Add a database + container with partition key `/customerId`.
3. Insert 5 documents in Data Explorer.
4. Run a SQL-style query: `SELECT * FROM c WHERE c.city = 'Seattle'`.
5. Toggle consistency level; observe trade-off.

## Lab 3: Blob storage tiers

1. Create a storage account.
2. Upload a blob; set access tier to Hot.
3. Move it to Cool, Cold, Archive.
4. Try to download from Archive -> rehydrate first.

## Lab 4: Power BI Desktop -> Service

1. Connect Power BI Desktop to Azure SQL DB.
2. Build a simple report (bar + KPI).
3. Publish to Power BI Service workspace.
4. Pin a visual to a dashboard.

## Lab 5: Microsoft Fabric end-to-end

1. Start a Fabric trial.
2. Create a Lakehouse; ingest a CSV.
3. Use a SQL endpoint to query.
4. Build a Power BI Direct Lake report.

## Lab 6: Real-time with Eventstream

1. In Fabric, create an Eventstream from a sample source.
2. Land into a KQL Database.
3. Build a Real-Time Dashboard tile from a KQL query.

---

[Master Index](00-MASTER-INDEX.md)
