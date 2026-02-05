# Data Quality Rules

## Purpose

Data quality rules define the controls required to ensure that Critical Data Elements (CDEs) used in the FinCrime use case are accurate, complete, and reliable.

Effective data quality controls reduce the risk of missed suspicious activity, false positives, and regulatory findings.

## Data Quality Dimensions

Data quality rules are defined across the following dimensions:
- Completeness
- Validity
- Consistency
- Timeliness

## Completeness Rules

Completeness rules ensure that mandatory data elements are present before transactions are evaluated for monitoring.

### Examples
- customer_id must not be null for any transaction record
- account_id must be present for all monitored accounts
- transaction_amount must be populated for all financial transactions

## Validity Rules

Validity rules ensure that data values conform to expected formats and ranges.

### Examples
- transaction_amount must be greater than zero
- transaction_country must conform to approved country code standards
- customer_risk_category must be one of the approved risk classifications

## Consistency Rules

Consistency rules ensure alignment between related data elements across domains.

### Examples
- customer risk category used in transaction monitoring must align with the latest KYC assessment
- account-to-customer relationships must remain consistent across source systems

## Timeliness Rules

Timeliness rules ensure that data used for monitoring reflects current and relevant information.

### Examples
- transaction data must be available for monitoring within defined processing windows
- customer risk profile updates must be reflected in monitoring systems within an agreed timeframe

## Data Quality Escalation

Breaches of data quality rules are subject to investigation and escalation in accordance with data governance and incident management processes.

