``` mermaid
flowchart TD
    A[Develop] -->|git commit| B[Build]
    B --> C[TEST]
    C --> D[SIT]
    D --> E[PROD]

    %% Notes above SIT and Prod
    D:::annotated
    E:::annotated

    %% Annotation lines
    X1[Release branch made] -.-> D
    X2[CR approval] -.-> E

    classDef annotated fill:#f9f9f9,stroke:#333,stroke-width:1px;
```
