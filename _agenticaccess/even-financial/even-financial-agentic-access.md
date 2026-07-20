---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 17
api_specs:
- filename: even-financial-openapi-original.json
  format: json
  label: Engine by MoneyLion API
  slug: engine-by-moneylion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/even-financial/refs/heads/main/openapi/even-financial-openapi-original.json
consequence_counts:
  read: 17
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Even Financial Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Even Financial exposes 22 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Even Financial
provider_slug: even-financial
slug: even-financial-agentic-access
source_filename: even-financial-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/even-financial-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 5\n    connected: 17\n  by_consequence:\n    write: 5\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /leads/rateTables\n  method: post\n  operationId: submitLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads/{leadUuid}/rateTables\n  method: post\n  operationId: getRateTableForSpecifiedLead\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /originator/prefills/{prefillToken}\n  method: get\n  operationId: getPrefill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /originator/prefills\n  method: post\n  operationId: prefill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /originator/rateTables/{uuid}\n  method: get\n  operationId: getRateTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/{uuid}\n  method: get\n  operationId: getLead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/{uuid}\n  method: patch\n  operationId: updateLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /approvalProbability/loanReports\n  method: post\n  operationId: createLoansApprovalProbabilityReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /approvalProbability/loanReports/{uuid}\n  method: get\n  operationId: getLoansApprovalProbabilityReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offerPreview/loanOffers\n  method: get\n  operationId: getPreviewLoanOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offerPreview/creditCardOffers\n  method: get\n  operationId: getPreviewCreditCardOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offerPreview/savingsOffers\n  method: get\n  operationId: getPreviewSavingsOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supplyAnalytics/leadEvents\n\
  \  method: get\n  operationId: getLeadEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supplyAnalytics/leadPayouts\n  method: get\n  operationId: getLeadPayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supplyAnalytics/leadClientTags\n  method: get\n  operationId: getLeadClientTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supplyAnalytics/leadsInfo/{leadUuid}\n  method: get\n  operationId: getLeadsInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/universities\n  method: get\n  operationId: getUniversities\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/vehicles/years\n  method: get\n  operationId: getVehicleYears\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/vehicles/makes\n  method: get\n  operationId: getVehicleMakes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/vehicles/models\n  method: get\n  operationId: getVehicleModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/vehicles/trims\n  method: get\n  operationId: getVehicleTrims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /uiUtil/featuredFinancialInstitutions\n  method: get\n  operationId: getFeaturedFinancialInstitutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/even-financial/refs/heads/main/agentic-access/even-financial-agentic-access.yml
summary_line: 22 operations · 5 acting
tags:
- Company
- Financial Services
- Embedded Finance
- Fintech
- Lending
- Personal Loans
- Credit Cards
- Marketplace
- Recommendation Engine
- Lead Generation
---
