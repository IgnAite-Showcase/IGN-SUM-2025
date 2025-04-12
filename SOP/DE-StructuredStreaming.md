# Structured Streaming Approach

### Requirements - Ingest Source data file to Datalake
- Reduce latency and deliver data faster to BI Report
- Reduce Cost of Cloud resources
- Source (Providing business critical data in Realtime)
- Format: CSV, JSON, XML
- Big Data: Volume, Velocity, Verity
- Event: No specific file arrival Schedule
- Schema: Files could have varying schema
- Checkpoint: Avoid Duplicate loading load new files
- Exception: Deal with any failure

## Execution Option
- Schedule: 10K at 10PM. $
- File Arrival: 10K every Hour. $$
- Continuous: 10K at throught day. $$$
