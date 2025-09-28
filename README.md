# Bank Statement Extraction and Visualization

## Overview
This project extracts account details and transaction tables from ICICI Bank PDF statements, cleans the data, and visualizes transaction trends over time.

## Features
- Extracts account information (Account Number, IFSC, Bank Name)
- Parses transaction history (Date, Description, Deposit, Withdrawal, Balance)
- Generates a timeline plot for deposits and withdrawals
- Outputs cleaned CSV/Excel for further analysis

## Methodology
1. Extract text and tables using **pdfplumber** and regex.
2. Clean and structure data into a pandas DataFrame.
3. Visualize transaction trends with **Matplotlib**.
4. Summarize results in a report (PDF).

## Challenges
- Inconsistent PDF layouts.
- Low accuracy with pdfplumber for multi-line tables.
- Parsing account info with varied formats.

## Future Scope
- Use **DeepDeSRT/TableNet** for robust table extraction.
- Integrate **LLM + RAG** for advanced document understanding.
- Extend to multiple bank formats.

## Requirements
Install dependencies with:
```bash
pip install -r requirements.txt
