```mermaid
graph LR
    subgraph Source Systems
        D365[Dynamics 365]
        PA[Power Automate]
        PApp[Power Apps]
    end

    subgraph Monitoring Layer
        AI[Azure Application Insights]
        LogA[Log Analytics Workspace]
    end

    subgraph Action Layer
        Alerts[Azure Alerts]
        Notify[Email / SMS / Teams Notification]
    end

    D365 --> AI
    PA --> AI
    PApp --> AI
    
    AI --> LogA
    LogA --> Alerts
    Alerts --> Notify

    style AI fill:#0078d4,color:#fff
    style Alerts fill:#d83b01,color:#fff
```
