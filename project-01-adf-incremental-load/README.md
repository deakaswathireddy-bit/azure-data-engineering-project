# Incremental Data Load using Azure Data Factory

## Objective
Build an incremental data load pipeline to process only new or updated records.

## Scenario
Source system sends daily data. Instead of full load, we load only delta records.

## Tools Used
- Azure Data Factory
- Azure Data Lake Gen2

## Incremental Logic
- Watermark column: last_updated_date
- Lookup activity fetches last processed date
- Copy activity filters new records

## Benefits
- Reduced processing time
- Cost-efficient ETL
