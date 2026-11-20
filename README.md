# AudioInsight Data Platform

A portfolio-ready data engineering project for an audio-content product. It ingests listener events, applies data-quality rules, quarantines invalid records, and loads an analytics-ready star-schema warehouse.

## Highlights

- Python ETL pipeline with schema, referential-integrity, timestamp, and metric validation
- Star schema: listener, content, and date dimensions plus a granular listening-event fact table
- Quarantine output and ETL audit logging for traceability
- Idempotent loading, automated tests, PostgreSQL-ready DDL, and SQL business-insight queries
- Zero-dependency local demo using Python's standard library and SQLite

## Project layout

```text
audioinsight-data-platform/
├── data/raw/                 # Source listener, content, and user data
├── sql/                      # PostgreSQL DDL and analytics queries
├── src/audio_warehouse/      # ETL pipeline code
├── tests/                    # Data-quality and idempotency tests
└── run_pipeline.py           # Pipeline entry point
```

## Run locally

Requires Python 3.10+.

```bash
python run_pipeline.py
python -m unittest discover -s tests -v
```

## Resume-ready project entry

**AudioInsight Data Platform | Python, SQL, SQLite/PostgreSQL, Data Quality**

- Built an idempotent ETL pipeline to transform listener-event data into a star-schema warehouse.
- Implemented data-quality checks, quarantined invalid events, and recorded audit metrics.
- Wrote SQL analysis for engagement, completion rate, and content performance.
