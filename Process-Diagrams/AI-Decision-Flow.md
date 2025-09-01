# AI Decision Flow

```mermaid
flowchart TD
    A[Customer Uploads Documents] --> B[OCR Extracts Data]
    B --> C{Validation Checks}
    C -->|Aadhaar Match| D[UIDAI e-KYC Validation]
    C -->|PAN Match| E[NSDL PAN Validation]
    C -->|Mismatch Detected| F[Flag for Manual Review]
    D --> G{Fraud/AML Screening}
    E --> G
    F --> G
    G -->|Passed| H[Auto-Approval <10 mins]
    G -->|Failed| I[Rejected & Notified]
