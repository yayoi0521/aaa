graph LR
    subgraph 直接效应
    A[水流功率 ω] -->|β=0.58***| E[土壤分离能力 Dc]
    B[剪切力 τ] -->|β=0.34**| E
    C[容重 BD] -->|β=0.26**| E
    D[水稳性团聚体 WR0.25] -->|β=-0.19*| E
    end

    subgraph 间接效应
    F[流速 V] -->|β=0.65***| B
    F -->|β=0.72***| A
    C -->|β=-0.36**| G[孔隙度 TP]
    G -.->|β=-0.12| E
    end

    style A fill:#f9d5e5,stroke:#e47297
    style B fill:#d5e8d4,stroke:#82b366
    style C fill:#e1d5e7,stroke:#9673a6
    style D fill:#fff2cc,stroke:#d6b656
    style F fill:#dae8fc,stroke:#6c8ebf
    style G fill:#f8cecc,stroke:#b85450
