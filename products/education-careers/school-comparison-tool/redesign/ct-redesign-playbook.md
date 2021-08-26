# Comparison Tool Redesign Playbook

NOTE: 
- links to complete data for each of the sections below is welcome and encouraged.
- This document serves the requirement of an incident response procedure for your product. This document should be iterated upon as changes are made to the product.

## Product Description
Use the GI Bill Comparison Tool to see how VA education benefits can pay for your education.

[**Product Outline**](https://github.com/department-of-veterans-affairs/va.gov-team/blob/master/products/education-careers/school-comparison-tool/redesign/ct-redesign-discovery_product-outline.md)

## Routes to code
links here
issue tickets (if they add value when describing known errors for your product)

## Contacts

### Team Members:
- OCTO-DE product lead: Matt Self (Matthew.Self2@va.gov)
- Product manager: Darrell Neel (Neel_Darrell@bah.com) / Will McCormack (McCormack_Will@bah.com)
- Lead engineer: Dan Shawkey (Shawkey_Daniel@bah.com)

#### Note: This project is in the process of going through a transition and the above contacts will be changing on or around 09/20/21.

### Outage Contacts:
- Senior developer: Devin McCurdy McCurdy_Devin@bah.com
- Senior developer: Matt Roth Roth_Matthew@bah.com

## Troubleshooting

### Errors and Metrics
  - **Performance Metrics**
    -  CT Search Autocomplete - [latency](http://grafana.vfs.va.gov/d/000000050/backend-service-report?viewPanel=141&orgId=1&from=now-7d&to=now) should remain stable at well below 500 ms
    -  CT Keyword Search - [latency](http://grafana.vfs.va.gov/d/000000050/backend-service-report?viewPanel=141&orgId=1&from=now-7d&to=now) should remain stable averaging 1 s with peaks below 2 s

### Issue investigation steps
- The most common issues that arise are data issues noticed by the EDU stakeholders. Since the backend GI Bill Comparison Tool Data Source (GIDS) is manually updated from several sources, anomolies in the data sources files cause unexpected display issues. The best way to troubleshoot is to get copies of the latest source files in question from EDU and load in to the staging [GIDS Dashboard](https://staging.va.gov/gids/dashboards). The data can be reviewed manually and the issue can be reproduced by generating a new version in the dashboard. Primary datasource is built in the [GIDS Institution Builder](https://github.com/department-of-veterans-affairs/gibct-data-service/blob/master/app/models/institution_builder.rb).

### Flipper Features and Rollback
- There will be a feature flag for the limited rollout. This will be updated prior to rollout.
- This redesign will replace the current [GI Bill Comparison Tool](https://www.va.gov/gi-bill-comparison-tool). For the limited rollout, it will reside in parallel with the existing tool. Once limited rollout is complete, the redesign will replce the existing tool.

## Security
N/A

