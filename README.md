### Pay transparency, measured rather than surveyed

I publish a free dataset of **job postings where the employer states a pay range**,
pulled from public ATS feeds (Greenhouse, Lever, Ashby, Workable) and normalised to
annual USD. 266 companies, ~18.7k live postings, ~8k of them with a published range.
Regenerated weekly, so the same companies can be compared over time.

- **[The dataset and the method](https://sjdfi0wjvosdju9.github.io/salary-data.html)** -- distributions, per-board
  publication rates, per-company medians, every number dated
- **[What changed and why](https://sjdfi0wjvosdju9.github.io/changes.html)** -- a public change log, including the
  bugs I found in my own pipeline (a date field read from `updated_at`, a dedupe key that
  ignored location, a hard-coded FX table that silently dropped ~1,170 postings)
- **[Raw CSV](https://sjdfi0wjvosdju9.github.io/data/salary-ranges-full.csv)** -- CC BY 4.0, no login
- **[Open data mirror](https://github.com/sjdfi0wjvosdju9/job-salary-open-data)**

Tools, if you would rather pay for the plumbing than rebuild it:
[ATS Job Feed](https://apify.com/contributory_garnet_hyz/ats-job-feed) (pay per job returned)
and [Freelance Lead Radar](https://apify.com/contributory_garnet_hyz/freelance-lead-radar).

Written up honestly rather than promotingly on [dev.to](https://dev.to/sdijjxcfs).
