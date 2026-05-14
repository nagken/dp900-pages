# DP-900 Reference Architectures

> Foundational data architecture shapes you should recognize.

## 1. Modern data warehouse

```mermaid
flowchart LR
    OLTP[OLTP DBs] --> ADF[Azure Data Factory / Fabric Pipelines]
    Files[SaaS files] --> ADF
    ADF --> OL[OneLake / ADLS Gen2 raw]
    OL --> Spark[Spark / Dataflows]
    Spark --> WH[Fabric Warehouse / Synapse]
    WH --> SemModel[Power BI semantic model]
    SemModel --> Reports[Reports + Dashboards]
```

## 2. Real-time analytics (lambda)

```mermaid
flowchart LR
    IoT[IoT devices] --> EH[Event Hubs / IoT Hub]
    EH --> Hot[Stream Analytics / Eventstream]
    Hot --> KQL[KQL DB / ADX]
    KQL --> RTD[Real-Time Dashboards]
    EH --> Cold[Capture to Lake]
    Cold --> Batch[Daily batch ELT]
    Batch --> WH[Warehouse]
```

## 3. Cosmos DB globally distributed app

```mermaid
flowchart LR
    User1[User EU] --> CDC1[Cosmos DB EU region]
    User2[User US] --> CDC2[Cosmos DB US region]
    User3[User APAC] --> CDC3[Cosmos DB APAC region]
    CDC1 <--> CDC2
    CDC2 <--> CDC3
    CDC3 <--> CDC1
```

## 4. Power BI publishing flow

```mermaid
flowchart LR
    PBIX[Power BI Desktop .pbix] --> WS[Workspace in Service]
    WS --> SemModel[Semantic model]
    SemModel --> Rpt[Report]
    Rpt --> Tile[Pinned tile]
    Tile --> Dash[Dashboard]
    SemModel --> Mobile[Mobile app]
```

## 5. Azure Storage tier lifecycle

```mermaid
flowchart LR
    New[New blob] -- Hot --> Mature[After 30d]
    Mature -- Cool --> Quarter[After 90d]
    Quarter -- Cold --> Archive[After 180d]
    Archive -- Rehydrate hours --> Restored[Restored to Hot]
```

---

[Master Index](00-MASTER-INDEX.md)
