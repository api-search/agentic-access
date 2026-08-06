---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 10
api_specs:
- filename: fundrise-connect-openapi.yml
  format: yaml
  label: Fundrise Connect API
  slug: fundrise-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/openapi/fundrise-connect-openapi.yml
consequence_counts:
  read: 10
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fundrise Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Fundrise exposes 17 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fundrise
provider_slug: fundrise
slug: fundrise-agentic-access
source_filename: fundrise-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/fundrise-connect-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 7\n    connected: 10\n  by_consequence:\n    write: 7\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/oauth/token\n  method: post\n  operationId: GetAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/{accountId}/liquidation\n  method: post\n  operationId: CreateShareLiquidationRequest\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/{accountId}/liquidation/{shareLiquidationRequestId}/cancel\n  method: put\n  operationId: CancelShareLiquidationRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offerings\n  method: get\n  operationId: GetOfferings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offering/{offeringId}/nav\n  method: get\n  operationId: GetHistoricalNav\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offering/{offeringId}/documents\n  method: get\n  operationId: GetOfferingDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/liquidation/acknowledgments\n  method: get\n  operationId: GetLiquidationAcknowledgments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offering/{offeringId}/acknowledgments\n  method: get\n  operationId: GetInvestmentAcknowledgments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/{accountId}/holdings\n  method: get\n  operationId: GetHoldings\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/client\n  method: post\n  operationId: CreateClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/client\n  method: get\n  operationId: GetClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/client\n  method: put\n  operationId: UpdateClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/{accountId}/investment\n\
  \  method: post\n  operationId: PlaceInvestment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/{accountId}/investment/{transactionId}/cancel\n  method: put\n  operationId: CancelInvestment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/{accountId}/tax-forms\n  method: get\n  operationId: GetTaxForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/{accountId}/transaction/{transactionType}/{transactionId}\n\
  \  method: get\n  operationId: GetTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/{accountId}/transactions\n  method: get\n  operationId: GetTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundrise/refs/heads/main/agentic-access/fundrise-agentic-access.yml
summary_line: 17 operations · 7 acting
tags:
- Company
- Financial Services
- Investing
- Real Estate
- Private Credit
- Venture Capital
- Alternative Assets
- Wealth Management
- Fintech
- Embedded Investing
---
