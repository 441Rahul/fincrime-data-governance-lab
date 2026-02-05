# Data Lineage

## Purpose

Data lineage describes how data flows through the FinCrime monitoring process, from source systems to alert generation and investigation.

Clear lineage supports explainability, auditability, and root cause analysis during regulatory reviews.

## Scope

This document provides a conceptual view of data lineage relevant to the FinCrime use case.  
It does not represent physical system integrations or implementation-specific data flows.

## High-Level Lineage Overview

FinCrime monitoring relies on the combination of customer, account, and transaction data originating from core banking and onboarding systems.

This data is evaluated against monitoring rules, resulting in alerts that are reviewed by compliance operations and, where necessary, escalated for regulatory reporting.

## Conceptual Data Flow

1. Customer and account data are sourced from onboarding and core banking systems and maintained in accordance with KYC requirements.

2. Transaction data is generated through customer activity and captured with relevant attributes such as amount, timing, and geography.

3. Customer risk profiles derived from KYC assessments are associated with transactions to provide contextual risk information.

4. Transactions are evaluated against predefined monitoring rules and risk indicators.

5. Alerts are generated when monitoring thresholds are breached and are logged with supporting data for investigation.

6. Compliance analysts review alerts, document outcomes, and determine whether escalation or regulatory reporting is required.

## Governance Alignment

Critical Data Elements identified for the FinCrime use case are tracked across this lineage to ensure completeness, accuracy, and consistency.

Data quality rules are applied at key points in the lineage to prevent incorrect or incomplete data from impacting monitoring outcomes.

## Explainability and Audit Support

Clear data lineage enables:
- Explanation of why specific alerts were generated
- Identification of data quality issues impacting monitoring
- Demonstration of control effectiveness during regulatory reviews

Lineage documentation supports both proactive risk management and reactive investigation scenarios.


