# Structured Streaming Approach

### Requirements - Ingest Source data file to Datalake
- Reduce latency and deliver data faster to BI Report
- Source (Providing business critical data in Realtime)
- Format: CSV, JSON, XML
- Big Data: Volume, Velocity, Verity
- Event: No specific file arrival Schedule
- Schema: Files could have varying schema
- Checkpoint: Avoid Duplicate loading load new files
- Exception: Deal with any failure
