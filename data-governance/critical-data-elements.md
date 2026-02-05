# Critical Data Elements (CDEs)

## Purpose

Critical Data Elements (CDEs) are data items that are essential to the effectiveness, accuracy, and regulatory defensibility of the FinCrime monitoring process.

Incorrect, incomplete, or inconsistent CDEs may result in missed suspicious activity, false positives, or regulatory non-compliance.

## CDE Structure

Each CDE is documented with:
- Description
- Associated data domain
- Usage in the FinCrime use case
- Risk of data failure

## customer_id

**Description**  
Unique identifier representing an individual or corporate customer.

**Data Domain**  
Customer Domain

**Usage in FinCrime**  
Links customer profiles to accounts, transactions, and alerts.

**Risk of Data Failure**  
Incorrect or inconsistent customer identifiers may result in transactions being misattributed, leading to missed suspicious activity or incorrect alert generation.

## customer_risk_category

**Description**  
Risk classification assigned to a customer based on KYC assessment.

**Data Domain**  
Customer Domain

**Usage in FinCrime**  
Influences transaction monitoring sensitivity and alert prioritisation.

**Risk of Data Failure**  
Incorrect risk categorisation may suppress alerts for high-risk customers or generate excessive false positives for low-risk customers.

## account_id

**Description**  
Unique identifier for a customer account.

**Data Domain**  
Account Domain

**Usage in FinCrime**  
Associates transactions with customers and supports behavioural analysis.

**Risk of Data Failure**  
Missing or incorrect account identifiers may break transaction lineage and hinder effective monitoring.

## account_id

**Description**  
Unique identifier for a customer account.

**Data Domain**  
Account Domain

**Usage in FinCrime**  
Associates transactions with customers and supports behavioural analysis.

**Risk of Data Failure**  
Missing or incorrect account identifiers may break transaction lineage and hinder effective monitoring.

## transaction_amount

**Description**  
Monetary value of a financial transaction.

**Data Domain**  
Transaction Domain

**Usage in FinCrime**  
Used in threshold-based rules and behavioural analysis.

**Risk of Data Failure**  
Incorrect transaction amounts may prevent detection of reportable or suspicious activity.

## transaction_country

**Description**  
Country associated with the origin or destination of a transaction.

**Data Domain**  
Transaction Domain

**Usage in FinCrime**  
Supports identification of high-risk jurisdictions and sanctions exposure.

**Risk of Data Failure**  
Incorrect country data may result in failure to identify cross-border or high-risk transactions.

## Governance Note

CDEs are subject to enhanced data quality controls, ownership accountability, and periodic review to ensure ongoing regulatory compliance.