# Article.AI.Transcripts.Python.GenAITranscriptsParseCountrySuppliers

Notebook shown in the "AI-Driven Insights: Uncovering Tariff Exposure from Transcripts" webinar

## Overview
This repository provides a Jupyter Notebook that demonstrates how to use LSEG data and generative AI to extract, parse, and analyze country and supplier information from company earnings call transcripts. The solution is designed to help users uncover tariff exposure and supply chain insights using advanced AI techniques.

## Features
- Automated extraction of country and supplier mentions from transcripts
- Parsing and structuring of unstructured text data
- Integration with LSEG data sources
- Example analysis of tariff exposure and supply chain risk
- Export of results to Excel for further analysis

## Prerequisites
- Python 3.8 or higher
- Jupyter Notebook or JupyterLab
- Required Python libraries:
  - pandas
  - numpy
  - openpyxl
  - requests
  - tqdm
  - ipywidgets
  - matplotlib

## Usage
1. Clone this repository or download the notebook file `GenAITranscriptsParseCountrySuppliers.ipynb`.
2. Ensure you have the required Python environment and dependencies installed.
3. Open the notebook in Jupyter Notebook or JupyterLab.
4. Follow the step-by-step instructions in the notebook to:
   - Load sample transcript data
   - Run the AI-driven extraction and parsing
   - Analyze and export the results

## Data Sources
- The notebook is designed to work with LSEG-provided transcript data. Sample data and output files (e.g., `supplier_countries_YYYYMMDD_HHMMSS.xlsx`) are included for demonstration purposes.
- For production use, connect to your LSEG data sources as described in the notebook.

## Output Excel File
The notebook generates an output Excel file (e.g., `supplier_countries_YYYYMMDD_HHMMSS.xlsx`) containing the extracted and structured results. The main columns in the output file are:

- **Id**: Unique identifier for each record.
- **lastUpdate**: Timestamp of the last update to the record.
- **eventTypeId**: Identifier for the type of event detected in the transcript.
- **eventTypeName**: Name or description of the event type.
- **EventStory**: Narrative or summary of the event as extracted from the transcript.
- **prompt_tokens**: Number of tokens used in the AI prompt for extraction.
- **sources**: Source(s) of the information, such as transcript file or section.
- **attempts**: Number of extraction attempts or passes for the record.
- **COUNTRY**: Country mentioned in relation to suppliers or supply chain.
- **SOURCING_PERCENT**: Percentage of sourcing attributed to the country, if available.
- **QUOTE**: The relevant quoted text or sentence from the transcript.
- **quote_in_transcript**: Boolean or indicator showing if the quote appears verbatim in the transcript.

These columns provide detailed, structured insights into supply chain events, country exposure, and sourcing information extracted from company transcripts.

## Support
For questions or support, please contact your LSEG representative or visit [LSEG Developer Portal](https://developers.lseg.com/).

## License
This sample is provided for demonstration purposes. Please refer to the LICENSE file or your LSEG agreement for usage terms.
