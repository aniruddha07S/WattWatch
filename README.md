# WattWatch (Evonence Campus Drive Assessment Hackathon)

This repository contains **WattWatch**, an AI Utility Auditor Agent developed for the Evonence  Assessment Hackathon.

## What is WattWatch?

WattWatch is an AI-powered agent designed to perform energy audits. The agent ingest energy usage data (kWh per hour) and combines it with external context to identify inefficiencies and anomalies. 

### Core Agent Logic
1. **Data Ingestion**: Parses hourly energy readings from a CSV file (e.g., college apartment energy data).
2. **Context Enrichment**: Integrates with the Sunrise-Sunset API to determine daylight hours for the specific days the data was recorded.
3. **Energy Audit & Rules Engine**: Analyzes the usage based on a set of rules:
   - Identifies top peak usage hours.
   - Detects abnormal spikes in usage.
   - Audits energy consumption in relation to daylight hours (e.g., leaving lights or appliances on when natural light is available).
4. **Reporting**: Generates comprehensive reports on energy efficiency to help reduce energy waste.

## Project Structure
- `app.js` / `generate_report.py`: The core scripts containing the agent logic.
- `energy_usage.csv`: Sample energy usage data.
- User interface files (`index.html`, `index.css`) for potential front-end integration.
