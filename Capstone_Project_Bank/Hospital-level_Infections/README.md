# README

## Dataset description
This project combines publicly available hospital quality measures from the Centers for Medicare & Medicaid Services (CMS) to investigate the relationship between healthcare-associated infections and hospital quality measures. Unfortunately, by their very nature, hospitals have the potential to spread infection and many patients will leave the hospital after a procedure with a new infection. Infection measures collected by the CMS include central line-associated bloodstream infections (CLABSI), catheter-associated urinary tract infections (CAUTI), surgical-site infections, MRSA bloodstream infections, and _C. difficile_ intestinal infections. Primary uses could include:

- developing interpretable statistical models and visualizations to support hospital quality improvement
- identifying hospital characteristics and quality measures associated with higher infection rates
- comparing patterns across infection types, hospital groups, and geographic regions

### Possible question
Are hospital quality metrics a reliable indicator of hospital infection rates?

## Source Citation
Centers for Medicare & Medicaid Services (CMS). Healthcare Associated Infections - Hospital. Provider Data Catalog. https://data.cms.gov/provider-data/dataset/77hc-ibv8

Centers for Medicare & Medicaid Services (CMS). Complications and Deaths - Hospital. Provider Data Catalog. https://data.cms.gov/provider-data/dataset/ynj2-r877

## Data documentation
Data dictionaries, measure descriptions, collection periods, and API documentation are available through the CMS Provider Data Catalog. The API provides programmatic access without an API key.

- Infection data API: https://data.cms.gov/provider-data/api/1/datastore/query/77hc-ibv8/0
- CMS API documentation: https://data.cms.gov/provider-data/docs
- Hospital measure collection periods: https://data.cms.gov/provider-data/topics/hospitals/measures-and-current-data-collection-periods

## Additional notes:
You will be required to use the CMS API for this analysis in order to avoid temporal structure in the data because of the limited timeframe of Capstone.