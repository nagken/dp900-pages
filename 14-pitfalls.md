# DP-900 Pitfalls

> Mistakes that cost points on a fundamentals exam.

## Concepts

- Confusing semi-structured (JSON) with unstructured (PDF / images).
- Putting OLAP queries on an OLTP DB -> blocking.
- Using "report" and "dashboard" interchangeably in Power BI.

## Relational

- Picking Azure SQL DB when cross-DB queries / SQL Agent are required (-> use Managed Instance).
- Picking SQL on VM when PaaS would suffice -> avoidable patching.
- Forgetting firewall rule on Azure SQL DB -> connection refused.

## Non-relational

- Choosing Strong consistency in a globally-distributed write app -> single-region only.
- Picking Table storage for new workloads -> Cosmos Table API is recommended.
- Forgetting Archive tier rehydration is hours.
- Confusing Azure Files (SMB share) with Blob (object store).

## Analytics

- Using Synapse dedicated SQL pool for ad-hoc small-team analytics -> Fabric is usually simpler.
- Doing transforms in Power BI for huge data -> push to Spark / Warehouse.
- Mixing Fabric Eventstream and Stream Analytics in same hop -> pick one.
- Forgetting Direct Lake requires OneLake parquet.
- Treating ETL and ELT as identical.

## Tools

- Authoring paginated reports in Power BI Desktop -> use Report Builder.
- Using account keys instead of Microsoft Entra ID auth + Managed Identity.

---

[Master Index](00-MASTER-INDEX.md)
