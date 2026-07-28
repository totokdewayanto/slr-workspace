# SLR Workspace — Systematic Literature Review

Dikelola oleh **OpenWorker** + **aisuite** + **GROQ (Llama 3.3 70B)**

## Struktur Folder

```
slr-workspace/
├── protocol/              # Protocol SLR (PRISMA-P)
├── search/                # Search strategy & logs
├── data/
│   ├── screening/         # Log screening (title/abstract + full-text)
│   ├── extraction/        # Data extraction forms
│   └── quality/           # Risk of bias assessment
├── analysis/
│   ├── deduplication/     # Dedup scripts (Python/Colab)
│   └── synthesis/         # Meta-analysis & narrative synthesis
├── report/
│   ├── draft/             # Naskah manuscript
│   ├── figures/           # Forest plot, PRISMA flow diagram
│   └── appendix/          # Appendix & supplementary materials
└── docs/
    ├── templates/         # Template extraction forms
    └── references/        # PDFs & reference manager exports
```

## Tools Stack

| Tool | Fungsi |
|---|---|
| OpenWorker | AI orchestrator — manage seluruh workflow SLR |
| GROQ (Llama 3.3 70B) | LLM untuk screening, extraction, synthesis |
| NotebookLM | Deep document analysis, Q&A, research |
| Google Colab | Python computing (dedup, meta-analysis) |
| Google Sheets | Screening log, data extraction, PRISMA tracker |
| Google Docs | Protocol & manuscript writing |
| GitHub | Version control & collaboration |

## Google Sheet — SLR Data

[SLR_Data](https://docs.google.com/spreadsheets/d/17bCiWVi_KhXYw0kqSoHUk1Zrk7Py1YXlXmKtVbixnPk/edit)

| Sheet | Fungsi |
|-------|--------|
| Search_Log | Log pencarian dari database (Scopus, WoS, PubMed, IEEE) |
| Screening | Keputusan title/abstract & full-text screening |
| Extraction | Data extraction form |
| Quality | Risk of bias assessment (RoB 2, NOS, CASP) |
| PRISMA | PRISMA 2020 flow diagram tracker |

## Status Setup

- ✅ Folder struktur lokal siap
- ✅ GitHub repo: totokdewayanto/slr-workspace
- ✅ Google Sheet SLR_Data — 5 sheets siap
- ✅ GROQ API terkonfigurasi di OpenWorker
- ⏳ **Google Docs** — klik [Connect](https://connect.composio.dev/link/lk_dcOK08RtHkJU) di browser
- ⏳ **NotebookLM** — perlu `notebooklm login` ulang (token expired)
- ⏳ **Local git push** — 403 auth mismatch (repo via Composio sudah terisi)

## Cara Pakai

1. Jalankan `notebooklm login` di terminal untuk autentikasi ulang
2. Buka link Google Docs di browser
3. Mulai SLR: **"Bantu setup SLR tentang [topik]"**
4. OpenWorker akan orchestrasi seluruh proses sesuai PRISMA 2020
