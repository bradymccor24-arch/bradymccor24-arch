# Brady McCormick

Applied sports scientist moving into product, data, and engineering roles in sports and health tech.
MS Biokinesiology (USC) · CSCS · four years inside performance departments at Texas, Maryland, and Fresno State,
building the data systems coaches and performance staff rely on.

## Featured work

### [AMS System Map](https://github.com/bradymccor24-arch/ams-system-map)
A read-only map of a Teamworks AMS site (570 forms, 40,861 fields, 256 dashboards) that answers what the platform
can't: what a change will break, where a number comes from, and whether a stored value is right.
- Lineage graph across 71,187 links; formula evaluator and data-quality checks over 18M+ records
- Found 871 broken references and 893 stored values that differ from a fresh calculation
- Daily health report, 13 connector checks, written governance rules · R, static web app, built with Claude Code

### [Athlete Data Platform](https://github.com/bradymccor24-arch/athlete-data-platform)
A PostgreSQL backend for athlete monitoring, built with Claude Code and modelled on
the Catapult, ForceDecks and AMS pipelines from my own jobs. Synthetic data throughout.
- Typed schema with database-enforced rules; Catapult and ForceDecks loaders (R) that validate, reject with reasons
  and reload safely
- Legacy JSON/XML form store migrated in batches with nothing lost (310k records, accounting test)
- Rolling workload (ACWR) computed by a `SKIP LOCKED` job queue, not on page load; team isolation via row-level security
- Indexes chosen from query plans (up to 247x faster); SQL and R tests in CI on PostgreSQL 15-17

### [Job Search Toolkit](https://github.com/bradymccor24-arch/job-search-toolkit)
A self-hosted job board: an hourly watcher over 36 employer job-board APIs (plain Python, no AI), an AI judgement
pass that follows written hard rules, and a local board with a Refresh button. Cheap work in code; judgement in AI.
I designed it and set its rules; the code was written with Claude Code.

## Portfolio

- **[Portfolio (PDF, 34 pages)](Brady-McCormick-Portfolio.pdf)**: design case studies, reporting systems, and
  applied sports science work. Athlete identifiers removed.
- **[AMS System Map presentation (PDF, 27 slides)](AMS-System-Map-presentation.pdf)**: the problem, the
  architecture, the governance rules, and the results.

## What I work with

R · SQL (PostgreSQL) · REST APIs · data pipelines and data quality · Power BI · Microsoft Azure ·
Catapult, VALD, Perch, 1080 Sprint, Teamworks AMS · AI-assisted development (Claude Code)

## Contact

bradymccor24@gmail.com
