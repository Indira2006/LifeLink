# LifeLink – Project Flowchart

```mermaid
flowchart TD
    A[Donor / Recipient Registration] --> B[Validate & Encrypt Data]
    B --> C[Cloud Storage (Firebase Database)]
    C --> D[Compatibility Check (Blood / Organ)]
    D --> E[Urgency & Location Analysis (Google Maps API)]
    E --> F{Best Match Found? (AI)}

    F -- No --> G[Predictive Analytics (Forecast Organ Demand) + Chatbot Assistance]
    F -- Yes --> H[Notify Hospitals & Doctors]

    H --> I{Logistics Feasible?}
    I -- No --> G
    I -- Yes --> J[Route Planning & Tracking]

    J --> K[Transplant Execution]
    K --> L[Outcome Data & Continuous Improvement]
    L --> M[Feedback into Predictive Analytics & Support]
    M --> G
