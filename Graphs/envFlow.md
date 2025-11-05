``` mermaid
flowchart TD
    A[Develop] -->|git commit via ALM| B[Build]
    B --> C[UAT]
    C --> D[Preprod]
    D --> E[Prod]

    %% Notes above Preprod and Prod
    D:::annotated
    E:::annotated

    %% Annotation lines
    X1[Release branch made] -.-> D
    X2[CR approval] -.-> E

    classDef annotated fill:#f9f9f9,stroke:#333,stroke-width:1px;
```
