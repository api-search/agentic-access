---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 21
api_specs:
- filename: figure-technology-solutions-heloc-inquiries-openapi.yml
  format: yaml
  label: HELOC Inquiries API
  slug: heloc-inquiries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-heloc-inquiries-openapi.yml
- filename: figure-technology-solutions-heloc-pre-qualification-openapi.yml
  format: yaml
  label: HELOC Pre-Qualification API
  slug: heloc-pre-qualification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-heloc-pre-qualification-openapi.yml
- filename: figure-technology-solutions-portfolio-manager-openapi.yml
  format: yaml
  label: Portfolio Manager API
  slug: portfolio-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-portfolio-manager-openapi.yml
consequence_counts:
  read: 21
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Figure Technology Solutions Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 36
overview: 'Figure Technology Solutions exposes 36 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Figure Technology Solutions
provider_slug: figure-technology-solutions
slug: figure-technology-solutions-agentic-access
source_filename: figure-technology-solutions-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/figure-technology-solutions-heloc-inquiries-openapi.yml, openapi/figure-technology-solutions-heloc-pre-qualification-openapi.yml,\n  openapi/figure-technology-solutions-portfolio-manager-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 15\n    connected: 21\n  by_consequence:\n    write: 15\n    read: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /products/heloc/v1/inquiry/{appUuid}/verify-liens\n  method: put\n  operationId: verifyInquiryLiens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/heloc/v1/inquiry/{appUuid}/select-property\n  method: put\n  operationId: selectProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/heloc/v1/inquiry/{appUuid}/select-offer\n  method: put\n  operationId: selectInquiryOffer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/heloc/v1/inquiry/{appUuid}/cancel\n  method: put\n  operationId: cancelInquiry\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/heloc/v1/inquiry/{appUuid}/asset-depletion\n  method: put\n  operationId: assetDepletion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/heloc/v1/inquiry/{appUuid}/add-ssn\n  method: put\n  operationId: addInquirySsn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /products/heloc/v1/inquiry/{appUuid}/add-property-estimate\n  method: put\n  operationId: addInquiryPropertyEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/heloc/v1/inquiry/{appUuid}/add-income\n  method: put\n  operationId: addInquiryIncome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/heloc/v1/inquiry/{appUuid}/repull-credit\n  method: post\n  operationId: repullCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/heloc/v1/inquiry/start\n  method: post\n  operationId: startInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encryption/v1/encrypt\n  method: post\n  operationId: encryptPayload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/heloc/v1/lead/{appUuid}/reassign\n  method: patch\n  operationId: reassignLead\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/heloc/v1/inquiry/{appUuid}/attributions\n  method: patch\n  operationId: updateInquiryAttributions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/heloc/v1/inquiry/{appUuid}/properties\n  method: get\n  operationId: fetchMatchingProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/heloc/v1/inquiry/{appUuid}/direct-debt-payoff-offers\n  method: get\n  operationId:\
  \ fetchDirectDebtPayoffDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/heloc/v1/inquiry/{appUuid}/borrower-costs\n  method: get\n  operationId: getBorrowerCosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/heloc/v1/document/{appUuid}/list\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/heloc/v1/document/{appUuid}/download\n  method: get\n  operationId: downloadAllDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/heloc/v1/document/{appUuid}/download/{documentUuid}\n\
  \  method: get\n  operationId: downloadDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/heloc/v1/details/{appUuid}\n  method: get\n  operationId: fetchAppDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/v1/loan-originator\n  method: get\n  operationId: fetchLoanOriginators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/heloc/pre-qualify/v2\n  method: post\n  operationId: getHelocOffersV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /products/heloc/pre-qualify/v1\n  method: post\n  operationId: prequalifyHeloc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external/secure/api/v1/portfolio/asset/types\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/secure/api/v1/portfolio/layouts/{assetType}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/secure/api/v1/portfolio/download/owned/{assetType}/{layout}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/secure/api/v1/portfolio/download/owned/{assetType}/{layout}/{date}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/secure/api/v1/portfolio/download/pledged/{assetType}/{layout}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/secure/api/v1/portfolio/download/pledged/{assetType}/{layout}/{date}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/secure/api/v1/portfolio/download/owned/payment-history\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/secure/api/v1/portfolio/download/owned/payment-history/{assetType}/{reportDate}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/secure/api/v1/portfolio/download/owned/payment-history/{assetType}/{reportStartDate}/{reportEndDate}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/secure/api/v2/portfolio/asset/types\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/secure/api/v2/portfolio/layouts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /external/secure/api/v2/portfolio/download/owned/{layout}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external/secure/api/v2/portfolio/download/owned/payment-history\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/agentic-access/figure-technology-solutions-agentic-access.yml
summary_line: 36 operations · 15 acting
tags:
- Company
- Fintech
- Lending
- HELOC
- Home Equity
- Mortgage
- Capital Markets
- Blockchain
- Loan Origination
- Financial Services
---
