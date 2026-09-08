# Opportunity Mapping

## The Business Case 
### Baseline Numbers - And What They Mean for Clients
- **Weekly throughput**: ~5,000 product validations + ~1,000 product modifications = ~6,000 items per weekly cycle (Monday-Sunday).
- **Overall success rate**: 91-94%. At 6% average failure: 300-450 products per week pass through or fail validation with errors. These products are potential inputs to 5-6 downstream modules generating client-facing reports and visualizations. There is currently no mechanism to determine which client outputs have been affected by a given data error.
- **New-category success rate**: ~65%. Approximately 35% of new-category products fail validation. Because the cycle is fixed at 7 days, a failing product misses the entire weekly publish window - but a product with an undetected error that passes validation goes directly into client-facing modules. Clients reviewing reports on new product categories are interacting with data that has a meaningful probability of being incorrect.
- **Client impact framing**: The catalog is not the end of the data journey. It is the beginning of the client-facing one. Reports, visualizations, and module outputs built on bad catalog data deliver wrong insights to paying clients. Clients who make decisions based on those insights - or who simply notice the errors - face a trust and credibility problem with the platform. That is a churn signal, not just a data quality flag.

> The 7-day cycle penalty for new-category products means errors can persist in client-facing outputs for 14+ days before correction. For a client actively using those reports to make purchasing, category, or strategic decisions, 14 days of bad data is a relationship-level risk.
