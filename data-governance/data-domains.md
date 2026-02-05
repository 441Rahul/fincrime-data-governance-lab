# Data Domains

## Purpose

Data domains provide a logical grouping of data elements used in the FinCrime use case.  
They establish ownership, accountability, and scope boundaries to support effective data governance, auditability, and regulatory compliance.

## Customer Domain

The Customer Domain contains data related to the identity, profile, and risk attributes of individual and corporate customers.

This domain supports customer due diligence, risk classification, and ongoing monitoring activities.

### Example Data Elements
- Customer identifier
- Customer type (individual / corporate)
- Country of residence or incorporation
- KYC risk category

### Ownership Considerations
This domain is typically owned by Customer Operations or Compliance functions, with stewardship responsibilities shared across onboarding and KYC teams.

## Account Domain

The Account Domain includes data related to customer accounts and their operational status.

It provides the structural linkage between customers and transactional activity.

### Example Data Elements
- Account identifier
- Account type
- Account status
- Customer-to-account relationship

### Ownership Considerations
This domain is commonly owned by Core Banking or Operations teams, with defined interfaces to FinCrime monitoring systems.

## Transaction Domain

The Transaction Domain captures financial movements initiated by or involving customer accounts.

This domain is central to transaction monitoring and suspicious activity detection.

### Example Data Elements
- Transaction identifier
- Transaction amount
- Transaction date and time
- Originating and destination accounts
- Counterparty country

### Ownership Considerations
This domain is typically owned by Payments or Core Banking teams, with strict controls due to its direct impact on regulatory monitoring outcomes.

## Alert Domain

The Alert Domain contains data generated as part of the transaction monitoring process, including alerts, investigation outcomes, and audit trails.

### Example Data Elements
- Alert identifier
- Triggering rule or scenario
- Alert status
- Investigation outcome
- Escalation indicator

### Ownership Considerations
This domain is owned by Compliance Operations, with oversight from Financial Crime Risk and Internal Audit functions.

## Governance Note

Clear definition of data domains supports consistent data ownership, reduces ambiguity during regulatory reviews, and enables effective data quality and lineage controls across the FinCrime operating model.

