# Brady McCormick

Applied sports scientist moving into product, data, and engineering roles in sports and health tech.
MS Biokinesiology (USC) · CSCS · four years inside performance departments at Texas, Maryland, and Fresno State,
building the data systems coaches and performance staff rely on.

## Work by program

The same job in every program: get vendor data out of its own system and into one place, in one shape,
so a number can be trusted. My original code from each is in
[sports-data-pipelines](https://github.com/bradymccor24-arch/sports-data-pipelines).

| Program | Years | What I built |
|---|---|---|
| Texas Athletics | 2024-present | [AMS System Map](https://github.com/bradymccor24-arch/ams-system-map): lineage, data quality and monitoring over a Teamworks AMS |
| University of Maryland | 2023-24 | Nine-source pipeline into Azure and Power BI; [Catapult to PostgreSQL](https://github.com/bradymccor24-arch/sports-data-pipelines/tree/main/maryland-football-2023-24) |
| Fresno State | 2022-23 | [PCA to choose GPS metrics, snap counts, VBT vs force plate](https://github.com/bradymccor24-arch/sports-data-pipelines/tree/main/fresno-state-2022-23) |
| LA Giltinis (MLR) | 2021-22 | [Catapult game demands, z-scores, 10 Hz data into PostgreSQL, session RPE](https://github.com/bradymccor24-arch/sports-data-pipelines/tree/main/la-giltinis-2021-22) |
| USC Athletics | 2021 | [Catapult and PFF into PostgreSQL, ForceDecks z-scores, NordBord, wearables](https://github.com/bradymccor24-arch/sports-data-pipelines/tree/main/usc-athletics-2021) |
| USC MS Biokinesiology | 2020-22 | [Sensor-derived velocity, first workload model](https://github.com/bradymccor24-arch/sports-data-pipelines/tree/main/usc-graduate-work-2020-22); research at the Clinical Exercise Research Center |

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
