# DP-900 Flashcards

> Click any card to reveal the answer.

<section class="fc-section" data-fc-title="Core data concepts">
<h2>1 - Core data concepts</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">JSON / XML / Avro - which data type?</div><div class="fc-a"><strong>Semi-structured</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Many small writes per second?</div><div class="fc-a"><strong>OLTP</strong> workload.</div></div>

<div class="flashcard"><div class="fc-q">Few large analytical queries?</div><div class="fc-a"><strong>OLAP</strong> workload.</div></div>

<div class="flashcard"><div class="fc-q">Tunes indexes and runs backups?</div><div class="fc-a"><strong>Database administrator</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Builds pipelines into the data lake?</div><div class="fc-a"><strong>Data engineer</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Builds reports and KPIs?</div><div class="fc-a"><strong>Data analyst</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Pixel-perfect printable Power BI doc?</div><div class="fc-a"><strong>Paginated report</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Live tile monitoring view in Power BI Service?</div><div class="fc-a"><strong>Dashboard</strong>.</div></div>

</div>
</section>

<section class="fc-section" data-fc-title="Relational on Azure">
<h2>2 - Relational on Azure</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">Cloud-native single DB - which Azure service?</div><div class="fc-a"><strong>Azure SQL Database</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Need cross-DB queries and SQL Agent?</div><div class="fc-a"><strong>Azure SQL Managed Instance</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Need OS-level access to SQL host?</div><div class="fc-a"><strong>SQL Server on Azure VM</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Open-source PostgreSQL on Azure PaaS?</div><div class="fc-a"><strong>Azure Database for PostgreSQL</strong> (Flexible Server).</div></div>

<div class="flashcard"><div class="fc-q">SQL command to retrieve rows?</div><div class="fc-a"><code>SELECT</code>.</div></div>

<div class="flashcard"><div class="fc-q">Two T-SQL ways to authenticate?</div><div class="fc-a">SQL auth or <strong>Microsoft Entra ID</strong> auth.</div></div>

</div>
</section>

<section class="fc-section" data-fc-title="Non-relational">
<h2>3 - Non-relational</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">Globally distributed JSON docs?</div><div class="fc-a">Cosmos DB <strong>NoSQL API</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Existing MongoDB app?</div><div class="fc-a">Cosmos DB <strong>MongoDB API</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Graph traversal vertices + edges?</div><div class="fc-a">Cosmos DB <strong>Gremlin API</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Cosmos DB default consistency?</div><div class="fc-a"><strong>Session</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Strongest Cosmos DB consistency?</div><div class="fc-a"><strong>Strong</strong> (single-region writes only).</div></div>

<div class="flashcard"><div class="fc-q">Lowest-latency Cosmos DB consistency?</div><div class="fc-a"><strong>Eventual</strong>.</div></div>

<div class="flashcard"><div class="fc-q">SMB / NFS file share on Azure?</div><div class="fc-a"><strong>Azure Files</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Object store for large blobs?</div><div class="fc-a"><strong>Blob storage</strong> (ADLS Gen2 if hierarchical).</div></div>

<div class="flashcard"><div class="fc-q">Rarely accessed - rehydration in hours OK?</div><div class="fc-a"><strong>Archive</strong> tier.</div></div>

</div>
</section>

<section class="fc-section" data-fc-title="Analytics">
<h2>4 - Analytics</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">All-in-one SaaS analytics platform?</div><div class="fc-a"><strong>Microsoft Fabric</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Single tenant-wide lake in Fabric?</div><div class="fc-a"><strong>OneLake</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Power BI mode reading parquet from OneLake without import?</div><div class="fc-a"><strong>Direct Lake</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Open-source Spark analytics platform?</div><div class="fc-a"><strong>Azure Databricks</strong>.</div></div>

<div class="flashcard"><div class="fc-q">Code-free orchestration / ETL service?</div><div class="fc-a"><strong>Azure Data Factory</strong> (or Fabric Data Factory).</div></div>

<div class="flashcard"><div class="fc-q">High-throughput event ingestion?</div><div class="fc-a"><strong>Event Hubs</strong> (or IoT Hub).</div></div>

<div class="flashcard"><div class="fc-q">Real-time SQL over streams?</div><div class="fc-a"><strong>Stream Analytics</strong> or Fabric Eventstream / KQL DB.</div></div>

<div class="flashcard"><div class="fc-q">ELT vs ETL - modern pattern?</div><div class="fc-a"><strong>ELT</strong> - transforms run in the target's compute.</div></div>

</div>
</section>

<section class="fc-section" data-fc-title="Gotchas">
<h2>5 - Gotchas</h2>

<div class="flashcard-grid">

<div class="flashcard"><div class="fc-q">Cosmos Strong consistency limit?</div><div class="fc-a">Single-region writes only.</div></div>

<div class="flashcard"><div class="fc-q">Difference: dashboard vs report (Power BI)?</div><div class="fc-a">Report = pages of visuals; Dashboard = pinned tiles in Service.</div></div>

<div class="flashcard"><div class="fc-q">Archive tier rehydration time?</div><div class="fc-a">Hours.</div></div>

<div class="flashcard"><div class="fc-q">Direct Lake requirement?</div><div class="fc-a">Parquet stored in OneLake.</div></div>

<div class="flashcard"><div class="fc-q">Azure SQL DB - does it support cross-DB queries / SQL Agent?</div><div class="fc-a">No - that's Azure SQL Managed Instance.</div></div>

<div class="flashcard"><div class="fc-q">Table storage vs Cosmos Table API for new workloads?</div><div class="fc-a">Cosmos Table API (Table storage is legacy).</div></div>

</div>
</section>

---

[Master Index](00-MASTER-INDEX.md)
