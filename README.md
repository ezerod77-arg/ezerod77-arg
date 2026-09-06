# Ezequiel Rodríguez Cabrera

Production engineer. 20+ years keeping Oracle and PostgreSQL databases alive at scale — now building LLM-based knowledge systems and automation pipelines.

[LinkedIn](https://www.linkedin.com/in/ezequielgrodriguez1977)

---

### What I've been doing for 20 years

- **Databases at scale** — Oracle 10g–21c (RAC, Data Guard, RMAN, ASM, GoldenGate, Multitenant), PostgreSQL 13–17, MySQL, SQL Server. Estates from 200 to ~2,500 databases; a ~1,500-database migration to Exadata / 19c / Multitenant; led a 25-person DBA team.
- **Cloud & infrastructure** — OCI, AWS, Azure, Exadata, RHEL, Linux/Unix, Ansible, shell.
- **Production engineering** — incident response, root cause analysis, performance troubleshooting, backup & recovery, capacity planning, SLA management.

### What I've been building lately

Seven LLM-based systems, each deliberately harder than the last. What they have in common is the engineering, not the subject matter:

- **Multimodal ingestion** — nine audio/video formats normalized through `ffmpeg` into a single canonical form (mono 16 kHz MP3) matched to the transcriber's native input, then Whisper → timestamped SRT, so a citation can point at the exact minute of a recording. An hour of source material drops from hundreds of MB to ~15 MB *before* the expensive step.
- **Document ingestion** — native PDF text extraction plus OCR for scanned material, and web sources that aren't always machine-readable.
- **Grounded generation** — pipelines that hand the model real reference data (astronomical ephemerides, published financial statements) instead of letting it invent the facts it writes from.
- **Real-time market data** — integration with crypto exchange APIs (Binance, OKX, Bybit) for live data and multi-source aggregation.
- **Generative media chains** — script → cloned voice → video timed to the audio → synced subtitles, fanned out across parallel outputs from one workflow.
- **Knowledge bases with provenance** — ~3,000 markdown pages across several domains, where every page records whether a claim comes from a source or from the model's own reasoning. That distinction is the point; without it a knowledge base rots within months.

Most of it is Python. Some stages are still orchestrated by hand while I get them right.

### Why there are no public repositories here

These systems run against corpora I can't redistribute — licensed books, client material, third-party academic content — so the repositories are private. It's a licensing constraint, not an absence of work.

I'm happy to walk through the architecture of any of them, or show one running.
