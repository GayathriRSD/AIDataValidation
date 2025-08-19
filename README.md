 ```mermaid 
flowchart TD
    A[User / Account Team] --> B[Authentication]
    B --> C[Access AI Assistant (SharePoint / UI)]
    C --> D[Provide Application for Validation]
    D --> E[AI Assistant Collects Data from Sources]
    E --> F[Decryption & Secure Storage]
    F --> G[AI Assistant Compares Data (SailPoint vs Access Data)]
    G --> H{Discrepancies Found?}
    H -- Yes --> I[AI Highlights Issues & Outliers]
    H -- No --> J[AI Confirms Compliance]
    I --> K[AI Generates Validation Report]
    J --> K[AI Generates Validation Report]
    K --> L[Report Stored in SharePoint]
    L --> M[User Notified & Can Access Report]
    M --> N[Observability / Monitoring for Audit]
