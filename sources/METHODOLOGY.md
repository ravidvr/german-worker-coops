# Methodology

## How this directory was built

The database was compiled by aggregating, normalizing, and deduplicating entries from three publicly available grassroots sources.

## Sources

### 1. worker-coops.de
- **URL**: https://www.worker-coops.de/verzeichnis/worker-coops-deutschland
- **Type**: Curated directory by a German worker-coop advocacy project
- **Method**: The page was fetched directly and all list entries were extracted with their categories, descriptions, and external links
- **Governance**: Explicitly classifies co-ops into four categories based on worker control
- **Date accessed**: July 2, 2026 (page last updated May 6, 2026)
- **Entries contributed**: 44

### 2. Wikipedia: List of worker cooperatives
- **URL**: https://en.wikipedia.org/wiki/List_of_worker_cooperatives
- **Type**: Community-maintained global directory
- **Method**: The Germany section was extracted via the MediaWiki API
- **License**: CC BY-SA 4.0
- **Date accessed**: July 2, 2026
- **Entries contributed**: 5 (after deduplication)

### 3. GitHub: hng/tech-coops
- **URL**: https://github.com/hng/tech-coops
- **Type**: Community-maintained global tech cooperative directory
- **Method**: The README.md was fetched and the Europe/Germany table rows were parsed
- **License**: Repository license (MIT)
- **Date accessed**: July 2, 2026
- **Entries contributed**: 14 (after deduplication)

## Deduplication process

1. Entries were normalized by stripping legal form suffixes (eG, e.G.) and whitespace
2. Fuzzy matching on normalized names was used to identify potential duplicates
3. The entry with the most complete data (preferring worker-coops.de as primary source) was retained
4. Fields from deduplicated entries were merged into the surviving record

## Classification notes

- **worker_majority**: Source explicitly states 51%+ of employees are member-owners
- **governance_based**: Source indicates elevated decision-making power through governance structures (typically consumer co-ops with democratic governance)
- **statute_based**: Source indicates elevated decision-making power by statutory provisions
- **in_founding**: Cooperatives in the process of being established
- **unknown**: Governance model not specified in any source

## Limitations

- The directory is **not comprehensive** — there are an estimated 300-800 Produktivgenossenschaften in Germany, of which this directory captures ~60
- Industry/sector classification was inferred from descriptions and may be imprecise
- Location data is incomplete — many entries only have region-level location information
- The database relies on the accuracy of the source directories, which are community-maintained
