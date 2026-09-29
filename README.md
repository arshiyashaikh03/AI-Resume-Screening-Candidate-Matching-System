# AI Resume Screening & Candidate Analysis System

## Overview

An AI-powered recruitment assistance workflow that automates resume information extraction, job-requirement comparison, candidate skill-gap analysis, structured data storage, and recruiter analytics.

The system uses n8n for workflow automation, an AI model for resume analysis, Google Drive for document storage, Google Sheets for structured candidate data, and Power BI for analytics.

## Business Problem

Recruiters may receive a large number of resumes for a single job opening. Manually extracting candidate information and comparing resumes against job requirements can be time-consuming and inconsistent.

## Solution

The system automates the repetitive analysis process while keeping the final employment decision with a human recruiter.

### Workflow

```text
Resume PDF
    ↓
Google Drive
    ↓
n8n
    ↓
Extract Resume Text
    ↓
AI Analysis
    ↓
Structured Candidate Data
    ↓
Google Sheets
    ↓
Power BI Dashboard
    ↓
Human Recruiter Review
```

## Features

* Automated resume ingestion
* PDF text extraction
* AI-based information extraction
* Job requirement comparison
* Matched and missing requirement identification
* Structured candidate records
* Skill-gap analysis
* Power BI recruitment analytics
* Automated recruiter notification
* Human-in-the-loop review

## Technology Stack

* n8n
* Google Drive
* AI / LLM
* Google Sheets
* Power BI
* JSON
* GitHub

## AI Analysis

The AI extracts information explicitly present in the resume and compares it with job-related requirements.

The system is designed to avoid inventing qualifications or using irrelevant personal characteristics.

## Dashboard

### Page 1 — Executive Overview

* Candidates processed
* Average requirement coverage
* Candidates requiring review
* Common skill gaps

### Page 2 — Candidate Analysis

* Candidate information
* Skills
* Experience evidence
* Matched requirements
* Missing requirements

### Page 3 — Skill Gap Analysis

* Most frequently missing requirements
* Requirement coverage by candidate
* Skill availability across applicants

## Business Value

The workflow reduces repetitive resume-processing work and creates a consistent structure for recruiter review.

It also converts resume data into business insights such as:

* Which skills are commonly available?
* Which requirements are frequently missing?
* What skill gaps appear across applicants?
* How much candidate-review work is being generated?

## Human-in-the-Loop Design

The system does not make the final hiring decision.

AI-generated candidate analysis is provided as structured information for recruiter review.

## Sample Data

This repository uses fictional/sample candidate resumes and does not contain private candidate information.

## Project Structure

```text
AI-Resume-Screening-System/
│
├── README.md
│
├── data/
│   ├── resumes/
│   └── job_description/
│
├── workflow/
│   └── resume_screening_workflow.json
│
├── documentation/
│   ├── architecture.md
│   ├── ai_prompt.md
│   ├── data_dictionary.md
│   └── test_cases.md
│
├── dashboard/
│   └── dashboard_screenshots/
│
└── sample_output/
    └── candidate_analysis.json
```

## Future Improvements

* Resume format validation
* Duplicate resume detection
* OCR for scanned documents
* Multi-job support
* Recruiter feedback loop
* Candidate status tracking
* API-based integration with recruitment systems
* Additional analytics and monitoring
