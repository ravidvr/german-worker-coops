# 🇩🇪 German Worker-Owned Business Directory

**Community-curated directory of worker-owned businesses (Produktivgenossenschaften) in Germany.**

A unified, deduplicated database of German worker cooperatives and democratic workplaces, aggregated from publicly available grassroots sources. Contains **60 verified entries** across diverse sectors.

## 🎯 What this is

This directory tracks businesses where the workers collectively own and control the enterprise. In Germany, these are primarily registered as **eG** (eingetragene Genossenschaft) but also exist as other legal forms. The governance classifications follow the definitions from [worker-coops.de](https://www.worker-coops.de):

| Classification | Meaning |
|---------------|---------|
| **worker_majority** | 51%+ of employees are member-owners with voting rights |
| **governance_based** | Elevated worker decision power through governance structures |
| **statute_based** | Elevated worker decision power by statutory provisions |
| **in_founding** | In the process of being established |

## 📊 Data

- **60 entries** from 3 sources
- **44 sector categories** — from IT/Software to Agriculture to Manufacturing
- **Deduplicated** — cross-referenced across all sources
- **Sourced from:**
  - [worker-coops.de](https://www.worker-coops.de/verzeichnis/worker-coops-deutschland) — curated directory of German worker co-ops
  - [Wikipedia: List of worker cooperatives](https://en.wikipedia.org/wiki/List_of_worker_cooperatives) — community-maintained global list
  - [GitHub: tech-coops](https://github.com/hng/tech-coops) — global tech cooperative directory

### Files

| File | Format | Description |
|------|--------|-------------|
| `data/worker_coops_germany.json` | JSON | Full database with all fields |
| `data/worker_coops_germany.csv` | CSV | Tabular export for spreadsheets |

### Schema

```json
{
  "id": "WCOOP-0001",
  "name": "Example eG",
  "url": "https://example.coop",
  "description": "Description of what they do",
  "sector": "IT/Software",
  "location": "Berlin, Germany",
  "legal_form": "eG",
  "governance": "worker_majority",
  "source": "worker-coops.de"
}
```

## ⚠️ Disclaimer

This directory is **community-curated**, not an official register. It aims to track worker-owned businesses in Germany but is **not comprehensive**. The official German cooperative register (Genossenschaftsregister) at handelsregister.de contains all registered eGs but does not classify them by ownership structure (worker-owned vs. housing vs. banking vs. agricultural).

## 📜 License

This database is made available under the **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)** license.

**You must attribute:**
- [worker-coops.de](https://www.worker-coops.de) for contributed entries
- [Wikipedia](https://en.wikipedia.org/wiki/List_of_worker_cooperatives) (CC BY-SA) for contributed entries
- [hng/tech-coops](https://github.com/hng/tech-coops) (MIT) for contributed entries
- This repository for the compilation

## 🤝 Contributing

This directory grows through community contributions. See [CONTRIBUTING.md](CONTRIBUTING.md) for how to add or update entries.

## 📬 Contact

Questions, corrections, or additions? Open an issue or submit a PR.

---

*Built by aggregating publicly available data from worker-coops.de, Wikipedia, and GitHub tech-coops.*
