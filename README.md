# Bidco Africa Sales Performance and Pricing Engine
A data engineering solution transforming raw retail sales data for Bidco Africa into actionable KPIs: Data Health Score, Promotional Uplift and Competitive Pricing Index.

## Context & Executive Summary
This analysis converts one week of raw supermarket transactions into three actionable deliverables for Bidco:
  1. a data health report per store and supplier so you can trust numbers
  2. promotion performance metrics that quantify uplift, discount depth and coverage
  3. a pricing index that shows where Bidco sits versus peers by Section/Sub-Department and store.

My approach prioritises business value first: identify high impact SKUs and stores where pricing or promo changeswill most quickly increase sales or margin. All assumptions, definations and calculations are documented below.

## Data Health: Key Findings
### What's Working
- 99.8% data completeness across 30,000+ transactions
- All stores show >95% data quality
- Zero critical data gaps that would block decision-making

### What Needs Attention
1. **15 records missing supplier** (includes potential Bidco products)
   - Impact: Cannot include in competitive pricing analysis
   - Fix: Cross-reference with Bidco product catalog
2. **32 records missing RRP** (0.1% of the dataset)
   - Impact: Cannot detect promotions for these SKUs
   - Fix: Use category average as proxy for low-value items
  
### Recommended Actions
- **For Bidco** Proceed with annalysis using 99.9% of the data
- **For Retailer** Request RRP/Supplier updates for flagged records
- **For Duck** This data quality is suficient for real-time decision making

### Business Confidence Level: HIGH 
This dataset can reliably inform:
- Promotion strategy decisions
- Pricing adjustments
- Inventory planning


