 ```mermaid 
flowchart TD
    U[User / Account Team] --> A[Authentication]
    A --> B["Access AI Assistant (SharePoint / UI)"]
    B --> C["Provide Application Data for Validation"]
    C --> D["AI Assistant Collects Data (CSV) from Sources"]
    D --> E["Decryption & Secure Storage"]
    E --> F["AI Assistant Compares Data (SailPoint vs Access Data)"]
    F --> G{"Discrepancies Found?"}
    G -- Yes --> H["AI Highlights Issues & Outliers"]
    G -- No --> I["AI Confirms Compliance"]
    H --> J["AI Generates Validation Report"]
    I --> J
    J --> K["Report Stored in SharePoint"]
    K --> L["User Notified & Can Access Report"]
    L --> M["Observability / Monitoring for Audit"]
