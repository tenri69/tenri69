<div align="center">
  <img src="./header.svg" alt="Henrik af Geijerstam Westerholm — Terminal" width="100%" />
</div>

<div align="center">
  <a href="mailto:henkawesterholm@outlook.com">
    <img src="https://img.shields.io/badge/Email-henkawesterholm%40outlook.com-161b22?style=flat-square&logo=minutemailer&logoColor=58a6ff&labelColor=0d1117" alt="Email" />
  </a>
  <a href="https://www.linkedin.com/in/henrik-af-geijerstam-w-093520229/">
    <img src="https://img.shields.io/badge/LinkedIn-Henrik_af_Geijerstam_W-161b22?style=flat-square&logo=linkedin&logoColor=58a6ff&labelColor=0d1117" alt="LinkedIn" />
  </a>
  <img src="https://img.shields.io/badge/Focus-C%2B%2B17_%7C_Java_%7C_Python-161b22?style=flat-square&logo=cplusplus&logoColor=ff7b72&labelColor=0d1117" alt="Tech Stack" />
</div>

---

### `01` // Featured Architecture: [TnsrLang](https://github.com/tenri69/TnsrLang)

A standalone domain-specific language (DSL) and deep learning engine built from scratch in modern **C++17** with **zero external runtime dependencies**.

```mermaid
graph LR
    A[Source .tnsr] -->|Custom Tokenizer| B(Token Stream)
    B -->|Recursive-Descent| C(AST)
    C -->|Tree-Walk Evaluator| D{AutoGrad Engine}
    D -->|Contiguous Buffers| E[Row-Major Tensor DAG]
    E -->|Reverse-Mode Backprop| F[Trained Weights]
    F -->|Embedded C++ HTTP| G((< 1ms Inference))

    style A fill:#0d1117,stroke:#30363d,color:#c9d1d9
    style B fill:#0d1117,stroke:#30363d,color:#c9d1d9
    style C fill:#0d1117,stroke:#58a6ff,color:#c9d1d9
    style D fill:#161b22,stroke:#ff7b72,color:#ff7b72
    style E fill:#0d1117,stroke:#30363d,color:#c9d1d9
    style F fill:#0d1117,stroke:#3fb950,color:#c9d1d9
    style G fill:#161b22,stroke:#3fb950,color:#3fb950
```

- **Language Frontend:** Custom tokenizer, recursive-descent AST parser, and lexically scoped tree-walk evaluator.
- **Compute Engine:** Cache-friendly reverse-mode AutoGrad engine using flat contiguous row-major tensor buffers and non-owning DAG captures.
- **Deployment:** End-to-end neural network training (`MNIST`, `XOR`) with an embedded C++ HTTP server for sub-millisecond browser inference.

---

### `02` // Systems & Engineering

| Project / Role | Stack | Architecture & Impact |
| :--- | :--- | :--- |
| **[Production Management System](https://github.com/Anton-Johannesson/krusty-skeleton)** | `Java` `Spark` `MySQL` | Concurrency-safe REST API and 8-table normalized schema using `SERIALIZABLE` transactions for inventory & pallet production. |
| **Bränslekollen** <br/> *Co-Founder & Lead Backend* | `Python` `Pipelines` | Engineered automated data ingestion pipelines and statistical modeling systems from the ground up. |
| **Large-Scale Software Project** <br/> *Test Group Lead* | `Java` `TDD` `CI/CD` | Led quality assurance across an 18-engineer project, architecting 120+ automated Java test suites. |
| **[ABAS Alarm System](https://github.com/tenri69/python-ABAS-alarm-system)** | `Python` `Hardware` | Code-driven intrusion detection system designed for real-time door and window sensor monitoring. |
