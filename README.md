# AIDataValidation
```mermaid
flowchart TD
    A[User Accesses SharePoint AI Assistant] --> B[Chat Interface: Select Application for Validation]
    B --> C[AI Retrieves Encrypted Raw Access Data rom Network Share]
    C --> D[Cloud Decryption Service: Decrypts PGP File]
    D --> E[Decrypted File Stored in SharePoint Workspace]
    E --> F[User Uploads/Specifies SailPoint Status Report]
    F --> G[AI Compares: Active Accounts vs Total Assignments (Report)]
    G --> H{Discrepancy Found?}
    H -- No --> I[Validation Report Generated with Counts]
    H -- Yes --> J[AI Identifies Outliers (Duplicate, Missing, Malformed Data)]
    J --> K[AI Prepares Detailed Discrepancy Report]
    I --> L[Report Saved in SharePoint Library]
    K --> L
    L --> M[User Receives Notification & Link to Report]
