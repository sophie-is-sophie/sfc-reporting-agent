# sfc-reporting-agent

# Autonomous SFC Short Position Reporting Agent

## Overview
This project is an autonomous multi-agent system designed to automate the SFC short position reporting process for compliance teams.

Built using Microsoft Copilot Studio, Power Automate, and SharePoint, the solution replaces manual checks and fragmented workflows with a fully automated, auditable reporting pipeline.

---

## Problem Statement
Compliance teams must manually collect position data, verify file availability, apply SFC reporting thresholds, and prepare reports for submission.

This process is:
- Time-consuming
- Prone to human error
- Difficult to audit
- Operationally risky due to tight deadlines

---

## Solution
This project implements a multi-agent system that automates the entire reporting workflow:

- Detects incoming position files automatically
- Validates data availability and completeness
- Applies SFC reporting thresholds (≥0.02% OR ≥ HKD 30M)
- Generates reporting outputs
- Notifies teams and supports approval workflows

---

## Target Users
- Compliance teams responsible for regulatory reporting
- Investment operations teams managing position data

---

## What Success Looks Like
- Fully automated weekly SFC reporting process
- Zero manual file checking
- Reduced reporting errors
- Complete audit trail for compliance
- Faster reporting turnaround

---

## Architecture

### Multi-Agent Design

#### 1. Data Agent
- Triggered on a schedule (Power Automate)
- Checks SharePoint for position file
- Validates file existence and readiness

#### 2. Calculation Agent
- Applies SFC thresholds:
  - ≥ 0.02% of issued share capital  
  - OR ≥ HKD 30 million
- Processes position data

#### 3. Reporting Agent
- Generates output/report
- Sends notification via Microsoft Teams
- Supports approval workflow via SharePoint

---

## Tech Stack
- Microsoft Copilot Studio
- Power Automate (cloud flows)
- SharePoint Online
- Excel (data source)
- Python (optional for calculations)

---

## Demo
👉 (Add your demo video link here)

---

## Repository Structure
