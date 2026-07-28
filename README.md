# SLR Workspace — Systematic Literature Review

Dikelola oleh **OpenWorker** + **aisuite** + **GROQ (Llama 3.3 70B)**

## Struktur Folder

```
slr-workspace/
├── protocol/              # Protocol SLR (PRISMA-P)
├── search/                # Search strategy & logs
├── data/
│   ├── screening/         # Log screening
│   ├── extraction/        # Data extraction
│   └── quality/           # Risk of bias assessment
├── analysis/
│   ├── deduplication/     # Dedup scripts
│   └── synthesis/         # Meta-analysis & synthesis
├── report/
│   ├── draft/             # Naskah manuscript
│   ├── figures/           # Forest plot, PRISMA flow
│   └── appendix/          # Appendix
└── docs/
    ├── templates/         # Template forms
    └── references/        # PDFs
```

## Tools

| Tool | Fungsi |
|---|---|
| OpenWorker | AI orchestrator |
| GROQ (Llama 3.3 70B) | LLM |
| NotebookLM | Document analysis |
| Google Colab | Python computing |
| Google Sheets | Screening & extraction |
| Google Docs | Protocol & manuscript |
| GitHub | Version control |

## Cara Pakai

1. Buka folder ini di **OpenWorker** (grant read-write)
2. Mulai dengan task: *"Bantu setup SLR tentang [topik]"*
3. OpenWorker akan orchestrasi seluruh proses sesuai PRISMA 2020
