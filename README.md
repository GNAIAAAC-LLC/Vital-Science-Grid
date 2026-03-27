graph TD
    subgraph "Orbital Layer"
        A[Solar Harvesting Satellites] -->|Wireless Energy| B[Terrestrial Tower Grid]
    end

    subgraph "Terrestrial Grid (USA, BD, IN)"
        B -->|$10/mo Power| C[Residential Households]
        B -->|Telemetry Data| D[VSG-Mesh Controller]
    end

    subgraph "Sovereign Health Layer"
        C -->|Metabolic Vitals| E[GNAI Health Scanner]
        E -->|Scan Result| F{Pharma-Forensic Analysis}
        F -->|Diseconomy Alert| G[Sovereign Medical Advice]
        F -->|Verified Meds| H[Continue Protocol]
    end

    subgraph "Data Backbone (Azure)"
        D -->|Cloud Sync| I[(Azure Cosmos DB)]
        F -->|Sync| I
        I -->|Global Ledger| J[GNAIAAAC LLC HQ]
    end

    %% Styling
    style A fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#ffd700,stroke:#333,stroke-width:4px
    style C fill:#bbf,stroke:#333,stroke-width:2px
    style I fill:#0072C6,stroke:#fff,stroke-width:2px,color:#fff
