# LLM-enabled-literature-mining
Python scripts for literature-based extraction and structuring of pore-structure and CO2 adsorption data of activated carbons using an LLM-assisted workflow.
# CO2 Adsorption Data Extraction for Activated Carbon

This repository contains four Python scripts used for literature-based extraction and structuring of pore-structure and CO2 adsorption data for activated carbons.

## Included files
- `porous_co2_extra.py`
- `CO2_capture_carbon_prompts.py`
- `TextProcess.py`
- `convert_to_csv_co2.py`

## What this code does
This workflow is designed for literature-based data extraction of activated-carbon CO2 adsorption studies.

- `porous_co2_extra.py`  
  Calls the LLM API to perform a two-step extraction workflow:
  1. extract semi-structured information from literature text;
  2. convert the extracted content into a structured JSON format.

- `CO2_capture_carbon_prompts.py`  
  Stores the prompts used for information extraction and JSON structuring.

- `TextProcess.py`  
  Provides utility functions for reading and preprocessing text/PDF/JSON content.

- `convert_to_csv_co2.py`  
  Merges the structured JSON outputs into a tabular CSV file.

## Notes
- This repository does **not** include any API keys, `.env` files, raw publisher full texts, intermediate extraction outputs, or final generated datasets.
- API access is configured through environment variables on the local machine.
- Users should prepare their own input data and set local paths before running the scripts.
- Some file paths in the scripts are local absolute paths and should be replaced by users according to their own environment.

## Environment
The scripts are intended to run in a local Python environment with the required dependencies installed by the user.

Example dependencies may include:
- `zhipuai`
- `json_repair`
- `tqdm`
- `PyMuPDF` (`fitz`)

## Important
Please do **not** upload:
- `.env`
- any API key or token
- raw full-text files obtained from publishers
- intermediate JSON outputs
- merged CSV outputs

## Disclaimer
This repository is intended for code sharing and methodological reference only.  
Users are responsible for ensuring that their use of literature content, APIs, and generated outputs complies with applicable publisher policies, database terms, and institutional requirements.
