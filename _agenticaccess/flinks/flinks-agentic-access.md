---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 1
api_specs:
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Authorize / Connect API
  slug: flinks-authorize-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Accounts Detail API
  slug: flinks-accounts-detail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Accounts Summary API
  slug: flinks-accounts-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Statements API
  slug: flinks-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Identity API
  slug: flinks-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Attributes / Analytics API
  slug: flinks-attributes-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Score API
  slug: flinks-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
- filename: flinks-openapi.yml
  format: yaml
  label: Flinks Fraud / KYC API
  slug: flinks-fraud-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/openapi/flinks-openapi.yml
consequence_counts:
  read: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Flinks Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Flinks exposes 12 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Flinks
provider_slug: flinks
slug: flinks-agentic-access
source_filename: flinks-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/flinks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 11\n    connected: 1\n  by_consequence:\n    write: 11\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /GenerateAuthorizeToken\n  method: post\n  operationId: generateAuthorizeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Authorize\n  method: post\n  operationId: authorize\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetAccountsDetail\n  method: post\n  operationId: getAccountsDetail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetAccountsDetailAsync/{requestId}\n  method: get\n  operationId: getAccountsDetailAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /GetAccountsSummary\n  method: post\n  operationId: getAccountsSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetStatements\n  method: post\n  operationId: getStatements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /FieldMatch\n  method: post\n  operationId: fieldMatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetCategorization\n  method: post\n  operationId: getCategorization\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetIncomeAttributes\n  method: post\n  operationId: getIncomeAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetCreditRiskAttributes\n  method: post\n  operationId: getCreditRiskAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Upload\n  method: post\n  operationId:\
  \ upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /FraudAnalysis\n  method: post\n  operationId: fraudAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flinks/refs/heads/main/agentic-access/flinks-agentic-access.yml
summary_line: 12 operations · 11 acting
tags:
- Financial Data
- Open Banking
- Bank Aggregation
- Fintech
- Canada
---
