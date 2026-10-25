### Pay transparency, measured rather than surveyed

I publish a free dataset of **job postings where the employer states a pay range**, pulled
from public ATS feeds (Greenhouse, Lever, Ashby, Workable) and normalised to annual USD.
The same companies are re-read every week, so two snapshots can be compared instead of
guessing whether a number moved.

**Latest snapshot: 2026-10-26** — [snapshot-2026-10-26](https://github.com/sjdfi0wjvosdju9/job-salary-open-data/releases/tag/snapshot-2026-10-26) · 266 companies · 18,758 live postings · 8,049 with a published range (43%) · median $200,000

p25 $150,000 / p75 $253,000 · CC BY 4.0 · regenerated weekly, no login anywhere.

- **[The dataset and the method](https://sjdfi0wjvosdju9.github.io/salary-data.html)** — distributions, per-board
  publication rates, per-company medians, every number dated
- **[What changed and why](https://sjdfi0wjvosdju9.github.io/changes.html)** — a public change log, including the
  bugs I found in my own pipeline (a date read from `updated_at`, a dedupe key that ignored
  location, a hard-coded FX table that silently dropped ~1,170 postings, a role classifier
  that hid 21.5% of rows in "other")
- **[Raw CSV](https://sjdfi0wjvosdju9.github.io/data/salary-ranges-full.csv)** — one row per posting, local currency
  plus USD
- **[Open data mirror](https://github.com/sjdfi0wjvosdju9/job-salary-open-data)** — same files, with one dated
  [release](https://github.com/sjdfi0wjvosdju9/job-salary-open-data/releases) per snapshot

Tools, if you would rather pay for the plumbing than rebuild it:
[ATS Job Feed](https://apify.com/contributory_garnet_hyz/ats-job-feed) (pay per job returned) and
[Freelance Lead Radar](https://apify.com/contributory_garnet_hyz/freelance-lead-radar).

Written up honestly rather than promotingly on [dev.to](https://dev.to/sdijjxcfs).
