# AI LeadOps Engine

## Overview

AI LeadOps Engine is an end-to-end lead generation, qualification, outreach, and pipeline management system built using n8n, Google Maps API, Google Sheets, and Gmail.

The system automatically discovers businesses from Google Maps, enriches and scores leads, stores them in a CRM, generates personalized outreach messages, sends emails, and tracks lead progression through a sales pipeline.

The project was built as a practical demonstration of how modern AI-assisted automation can replace repetitive sales operations and create scalable lead management workflows for small and medium-sized businesses.

## Features

### Lead Discovery
- Google Maps Places API integration
- Business information extraction
- Contact data collection
- Website detection
- Operational status validation

### Lead Enrichment
- Lead normalization
- City and country classification
- Business niche categorization
- Opening hours extraction
- Contact information standardization

### Lead Scoring
Rule-based scoring system using:
- Phone availability
- Website availability
- Business operational status
- Business maturity indicators
- Open/closed status

### AI-Powered Outreach
- Personalized email generation
- Dynamic messaging based on:
    - Business name
    - City
    - Niche
    - Website presence
    - Lead quality

### CRM Management
- Google Sheets CRM
- Automated lead updates
- Status tracking
- Priority assignment
- Contact history logging

### Pipeline Management
- Lead lifecycle tracking
- Follow-up scheduling
- Stage progression management
- Appointment tracking
- Opportunity monitoring

### Reporting
- Lead statistics
- Contact metrics
- High-priority lead tracking
- Pipeline visibility

## Architecture

The system consists of four major components:

1.  **Lead Acquisition Layer**
    - Google Maps API
    - Business discovery
    - Data collection
2.  **Automation Layer**
    - n8n workflows
    - Lead enrichment
    - Scoring engine
    - Outreach generation
3.  **CRM Layer**
    - Google Sheets CRM
    - Lead database
    - Pipeline tracking
4.  **Reporting Layer**
    - Operational metrics
    - Sales activity monitoring
    - Performance reporting

> See the diagrams folder for:
> - Overall Architecture Diagram
> - Workflow Flowchart
> - CRM Schema Diagram
> - Pipeline Lifecycle Diagram

## Workflows

### Workflow 1 - WhatsApp Lead Intake
**Purpose:** Capture inbound leads and automatically store them in a CRM.
**Flow:** Webhook → Classification → Google Sheets → Gmail Notification
**Key Features:**
- Lead categorization
- Automated storage
- Instant notifications

### Workflow 2 - Google Maps Lead Scraper
**Purpose:** Automatically discover and enrich business leads.
**Flow:** Google Maps API → Lead Normalization → Lead Scoring → CRM Storage
**Key Features:**
- Business discovery
- Contact extraction
- Data enrichment
- Lead scoring

### Workflow 3 - AI Follow-Up Pipeline
**Purpose:** Manage outreach and pipeline progression automatically.
**Flow:** Google Sheets Trigger → Personalized Outreach → Gmail → CRM Update → Pipeline Tracking
**Key Features:**
- Personalized outreach
- Follow-up management
- Pipeline tracking
- Status automation

## Tech Stack

- **Automation:** n8n
- **Data Sources:** Google Maps Places API
- **CRM:** Google Sheets
- **Communication:** Gmail
- **Logic Layer:** JavaScript
- **Documentation:** LaTeX (TikZ Diagrams), Markdown

## Pipeline Logic

The system follows the following lead lifecycle:

New Lead
↓
Contacted
↓
Waiting Reply
↓
Follow-Up Attempt 1
↓
Follow-Up Attempt 2
↓
Interested
↓
Meeting Requested
↓
Appointment Booked
↓
Proposal Sent
↓
Closed / Lost


This lifecycle provides visibility into every stage of lead progression and prevents duplicate outreach.

## CRM Design

The CRM stores:

### Lead Information
- Name
- Phone
- Address
- Website
- Business Status
- Source

### Business Classification
- Niche
- City
- Country

### Lead Quality
- Lead Score
- Priority

### Outreach Tracking
- Status
- Contacted At
- Follow-Up Message
- Next Action

### Pipeline Tracking
- Lead Stage
- Follow-Up Attempts
- Last Contacted At
- Next Follow-Up At

## Demo Screenshots

- **Workflow 1:** WhatsApp Lead Intake Workflow
- **Workflow 2:** Google Maps Scraper Workflow
- **Workflow 3:** AI Follow-Up Pipeline Workflow
- **CRM Screenshots:** Leads CRM, Pipeline Tracking, Lead Status Updates
- **Communication Screenshots:** Gmail Outreach Example, Follow-Up Example
- **Architecture Screenshots:** System Architecture Diagram, Workflow Flowchart, CRM Schema Diagram, Pipeline Lifecycle Diagram

## Demo Videos

| Demo | Link |
|--------|--------|
| Workflow 1 – WhatsApp Lead Intake | [Watch Demo](https://drive.google.com/file/d/13Q6i6xxPEzNSjb0hTPoBAsGJSSaqH3f4/view?usp=sharing) |
| Workflow 2 & 3 – AI LeadOps Engine | [Watch Demo](https://drive.google.com/file/d/1RSb3kybMOPcgb9Qgt8Ub3fvF4l7JOoCU/view?usp=sharing) |

## Future Improvements

### Short-Term
- Automated follow-up sequences
- Enhanced lead scoring
- Additional CRM reporting

### Medium-Term
- Multi-channel outreach
- LinkedIn integration
- WhatsApp outreach automation
- Appointment booking integration

### Long-Term
- AI-based lead qualification
- Multi-client support
- SaaS deployment
- Dashboard application
- Real-time analytics

## Author

**Yonatan Moges**
Master's Student in Artificial Intelligence
University of Sharjah
Focused on AI Automation, Workflow Engineering, and Business Process Automation.

