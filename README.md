# Customer Churn Analysis Dashboard

## Overview
An interactive Power BI / Microsoft Fabric report for analyzing customer churn patterns and retention metrics. This dashboard provides comprehensive visualizations to help understand customer behavior, identify at-risk segments, and develop retention strategies.

## Features
- **Key Performance Indicators (KPIs)**
  - Total customer count
  - Overall churn rate tracking
  
- **Interactive Visualizations**
  - Donut charts showing customer distribution by:
    - Gender
    - Activity status
    - Credit card status
    - Products owned
    - Country
  - Gauge chart for churn rate performance against targets
  - Combination column-line charts analyzing churn by:
    - Age groups
    - Account balance ranges
    - Credit score brackets

- **Interactive Filtering**
  - Dropdown slicer for filtering by churn status
  - Cross-filtering across all visuals

## Data Structure
The report uses the following data entities:
- **Customer Data** (primary table) - Core customer information including demographics, activity status, churn indicators
- **Age Groups** - Customer segmentation by age brackets
- **Acc Balance Groups** - Account balance categorization
- **Credit Score Groups** - Credit score segmentation

## Key Metrics Visualized
- Churn rate vs target performance
- Customer count by various demographics
- Country-wise customer distribution
- Correlation between account factors (age, balance, credit score) and churn

## Technical Details
- **Platform**: Microsoft Fabric / Power BI Report
- **Schema Version**: 3.2.0 (report), 2.8.0 (visuals)
- **Theme**: Tidal (custom) with CY26SU04 base theme

## Setup Instructions

### Prerequisites
- Microsoft Fabric workspace access or Power BI Desktop
- Proper data source connections configured

### Opening the Report
1. Clone this repository
2. Open the `.pbir` report file in Power BI Desktop or publish to Fabric workspace
3. Ensure data source connections are properly mapped

### Data Refresh
- Configure scheduled refresh in Fabric/Power BI Service
- Verify gateway connections if using on-premise data sources

## Dashboard Insights

The dashboard answers key business questions:
- Which customer segments have the highest churn rates?
- How do churn rates vary by demographics?
- What is the relationship between financial indicators and churn?
- Are retention targets being met?

## Customization
To modify this report:
1. Edit visual configurations in respective JSON files under `definition/`
2. Update `report.json` for report-level settings
3. Modify `themeCollection` settings for visual styling
4. Adjust `diagramLayout.json` for canvas arrangement

## Files Structure
├── definition/
│   ├── report.json (main report configuration)
│   ├── pages.json (page metadata)
│   ├── page.json (page-level settings)
│   ├── version.json (schema version)
│   ├── editorSettings.json (editor preferences)
│   ├── diagramLayout.json (canvas layout)
│   └── visual.json files (individual visual configs)
├── CY26SU04.json (base theme)
├── Tidal.json (custom theme)
├── localSettings.json (local environment settings)
└── README.md

## Requirements
- Microsoft Fabric / Power BI service access
- Appropriate data permissions
- Modern web browser for service viewing

## Support
For issues or questions, please refer to:
- Microsoft Fabric documentation
- Power BI community forums
