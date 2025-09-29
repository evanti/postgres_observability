# Postgres database performance observability and investigation 

<!-- This repository consists of a single readme file that contains description of how I recommend to approach Postgres database performance observability and investigation, how I use Grafana dashboards as an analytical DB interface for investigations, which data I collect and how I visualize the data to support thinking and analysis.


Tone reminder (keep handy)

Purpose: describe what is observed and how, not a case study.
Voice:
Neutral third person for architecture and mechanics.
“I” only for measured rationale or tradeoffs written inline.
“We” only for genuine shared standards or reader walk-through steps.
Diction: precise, concrete, low-ego. Prefer metrics and nouns over adjectives.
Claims: tie every assertion to a mechanism, a metric, or a procedure.
Brevity: one idea per sentence. Short paragraphs.
Consistency: keep the same person and tense within a section.
No sales language: avoid superlatives, hype, and abstractions without data.
Human signal: specific choices and thresholds that a practitioner would make.

Templates to mirror

Neutral architectural:
“Panel charts top CPU query fingerprints at 1-minute resolution. The stack exposes hotspot dominance, with tail grouped as ‘Other’. Overlays include host CPU and run-queue to separate database pressure from scheduler contention.”

Inline first person (sparingly):
“I cap the top-N at 8 to keep patterns legible. For multi-host views I pin y-axes per host to avoid cross-node misreads.”

Legitimate plural (team or tutorial):
“We standardize on pg_stat_statements with per-minute exports and reject samples with clock skew greater than 200 ms. We align exporter and database clocks via NTP.” -->



