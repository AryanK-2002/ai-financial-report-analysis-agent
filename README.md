# AI Financial Report Analysis Agent

An AI-powered workflow that automates the extraction and analysis of financial statements from company annual reports.

Built as an MVP for a Private Equity investment workflow, this project demonstrates how Large Language Models can significantly reduce manual effort involved in reviewing financial reports.

---

## Problem Statement

Investment teams spend significant time manually reviewing annual reports to extract financial metrics before performing investment analysis.

The objective of this project is to automate this repetitive workflow while keeping a human-in-the-loop for final investment decisions.

---

## Solution Overview

The workflow automatically:

- Downloads the financial report
- Parses PDF documents
- Extracts financial statements
- Identifies key financial metrics
- Performs financial health assessment
- Generates investment recommendations
- Stores structured results in Google Sheets

---

## Workflow Architecture

Workflow Trigger

↓

Fetch Financial Report

↓

Parse Financial Document (LlamaParse)

↓

Prepare Document Metadata

↓

Extract Financial Statements

↓

Financial Data Extraction Agent (Google Gemini)

↓

Parse Financial Metrics

↓

Financial Health Analysis Agent

↓

Parse Investment Assessment

↓

Merge Financial Results

↓

Store Results in Google Sheets

---

## Tech Stack

- n8n
- Google Gemini API
- Google AI Studio
- LlamaParse
- Google Drive
- Google Sheets
- JavaScript
- REST APIs

---

## Key Features

### Automated Financial Statement Parsing

Extracts:

- Revenue
- Net Income
- Total Debt
- Assets
- Liabilities
- Equity
- Cash Flow Metrics

---

### Financial Health Assessment

Generates

- Financial Health Rating
- Confidence Score
- Red Flags
- Investment Recommendation

---

### Structured Output

Results are automatically stored inside Google Sheets for downstream investment workflows.

---

## AI Agents

### Financial Data Extraction Agent

Responsibilities:

- Parse annual reports
- Detect consolidated financial statements
- Extract financial metrics
- Validate reporting period
- Normalize extracted data

---

### Financial Health Analysis Agent

Responsibilities:

- Analyze extracted metrics
- Identify financial risks
- Generate confidence score
- Recommend:

- Auto Approve

or

- Needs Human Review

---

## Sample Output

| Company | Revenue (Cr) | Net Income (Cr) | Total Debt (Cr) | Financial Health |
|----------|---------|------------|------|---------|
| TCS | 63,437 | 12,760 | Not Reported | Healthy |
| HDFC Bank | 724.2 | 164.7 | 5,993 | Moderate |
| ICICI Prudential AMC | 1,564.2 | 964.6 | Not Reported | Moderate |

---

## Future Improvements

- Multi-document support
- OCR fallback
- Vector database integration
- Historical trend analysis
- RAG-based financial question answering
- Portfolio-level risk scoring
- Investment memo generation
- Dashboard integration

---




