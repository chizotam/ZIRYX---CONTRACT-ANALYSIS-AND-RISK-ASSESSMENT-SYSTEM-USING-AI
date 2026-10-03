# Automated Legal Contract Analysis & Risk Assessment System

An AI-powered system that analyzes legal contracts, identifies potential risks and loopholes, performs compliance checks, and backs its findings with evidence from the uploaded document.

> **Note:** This system is intended for analysis and research purposes only and does not provide legal advice.

## Overview

Legal contracts can contain complex clauses, obligations, risks, and compliance requirements that are difficult to review manually.

This project is an automated contract analysis system. A user uploads a contract and receives a structured analysis of its contents. The system combines large language model analysis with rule-based checks to identify potential risks, summarize important clauses, and point to supporting evidence in the original document.

It was developed as a final-year Computer Science project.

## Key Features

- **Contract upload:** upload PDF and DOCX contracts for analysis.
- **Contract extraction:** extracts text from the uploaded document while preserving page-level information.
- **Clause analysis:** identifies and analyzes important clauses and provisions.
- **Risk assessment:** detects potential contractual risks and explains each one.
- **Loophole detection:** highlights ambiguous, incomplete, or problematic provisions.
- **Compliance checks:** runs rule-based checks against defined compliance requirements.
- **Evidence tracking:** links each identified issue back to the relevant page and section of the contract.
- **Conversational analysis:** a chat interface for asking questions about an analyzed contract.
- **Analysis history:** keeps previous analyses for easy reference.

## System Workflow

```
Contract Upload
      ↓
Document Extraction
      ↓
Clause & Content Processing
      ↓
AI-Based Analysis
      ↓
Rule-Based Compliance Checks
      ↓
Risk & Loophole Detection
      ↓
Evidence Tracking
      ↓
Analysis Results
```

## System Architecture

The system follows a client-server architecture: a React frontend, a FastAPI backend, AI analysis components, and a PostgreSQL database.

```
┌──────────────────────────┐
│      React Frontend      │
│      + Tailwind CSS      │
└────────────┬─────────────┘
             │
             ↓
┌──────────────────────────┐
│      FastAPI Backend     │
└────────────┬─────────────┘
             │
       ┌─────┴─────┐
       ↓           ↓
┌────────────┐ ┌───────────────┐
│ AI Analysis│ │  Rule-Based   │
│   Agent    │ │  Compliance   │
└─────┬──────┘ └───────┬───────┘
      │                │
      └───────┬────────┘
              ↓
┌──────────────────────────┐
│        PostgreSQL        │
│ Contract / Clause /      │
│ Results & Reports        │
└──────────────────────────┘
```

## Technology Stack

| Area | Technologies |
| --- | --- |
| Frontend | React, Tailwind CSS, Vite |
| Backend | Python, FastAPI |
| AI & analysis | Large language models, rule-based reasoning, natural language processing |
| Database | PostgreSQL |
| Authentication | JWT, bcrypt |
| Document processing | PDF and DOCX text extraction, page-level document tracking |

## AI and Rule-Based Approach

The system combines two complementary approaches.

**AI-based analysis:** large language models interpret contract language, summarize clauses, identify potential risks, and answer questions about the document.

**Rule-based analysis:** predefined rules handle structured compliance checks and deterministic conditions, where explicit requirements can be evaluated without relying entirely on model interpretation.

Using both lets the system apply AI to language understanding while keeping deterministic checks for defined compliance requirements.

## Interface

The application provides a document-focused interface for uploading contracts, reviewing analysis results, investigating identified risks, and asking questions about the analyzed document.

### Contract Upload

![Contract upload screen](images/contract-upload.png)

### Contract Analysis

![Contract analysis screen](images/contract-analysis-1.png)

### Contract Analysis (continued)

![Contract analysis screen, second view](images/contract-analysis-2.png)

### Loophole Analysis

![Loophole analysis screen](images/loophole-analysis.png)

## Project Objectives

1. Automate key parts of contract analysis.
2. Identify potential contractual risks and loopholes.
3. Support compliance checking using defined rules.
4. Provide traceable evidence for identified issues.
5. Reduce the manual effort required to review contracts.
6. Provide an interactive interface for querying analyzed contracts.

## Limitations

- AI-generated analysis can contain inaccuracies and should be reviewed by qualified professionals.
- The system does not replace professional legal advice.
- The accuracy of the analysis depends on the quality and structure of the uploaded document.
- Compliance rules depend on the requirements implemented within the system.
- The system was developed as an academic project and has not been evaluated as a production-grade legal service.

## Project Status

**Completed academic project.** The application was developed and tested locally as part of a final-year Computer Science project.

## Source Code

The source code is not publicly available in this repository. This repository is a project showcase, with documentation, the system architecture, and screenshots of the implemented application.

## Disclaimer

This project is an academic and technical demonstration of automated contract analysis. It is not a legal service and does not provide legal advice. Contractual decisions should be reviewed by an appropriately qualified legal professional.

## Project Information

- **Project type:** Final-Year Computer Science Project
- **Domain:** Artificial Intelligence, Natural Language Processing, Legal Technology
- **Application:** Automated Contract Analysis and Risk Assessment

## Author

Chiaghanam Chizotam · [GitHub](https://github.com/chizotam)
