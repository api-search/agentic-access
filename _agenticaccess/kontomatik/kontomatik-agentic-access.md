---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 17
api_specs:
- filename: kontomatik-ais-api-openapi.yml
  format: yaml
  label: Kontomatik Account Information Service API
  slug: kontomatik-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-ais-api-openapi.yml
- filename: kontomatik-pdf-parsing-api-openapi.yml
  format: yaml
  label: Kontomatik PDF Parsing API
  slug: kontomatik-pdf-parsing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-pdf-parsing-api-openapi.yml
- filename: kontomatik-data-analysis-api-openapi.yml
  format: yaml
  label: Kontomatik Data Analysis API
  slug: kontomatik-data-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-data-analysis-api-openapi.yml
- filename: kontomatik-report-api-openapi.yml
  format: yaml
  label: Kontomatik Report API
  slug: kontomatik-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/openapi/kontomatik-report-api-openapi.yml
consequence_counts:
  read: 17
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kontomatik Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'Kontomatik exposes 30 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kontomatik
provider_slug: kontomatik
slug: kontomatik-agentic-access
source_filename: kontomatik-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kontomatik-ais-api-openapi.yml, openapi/kontomatik-data-analysis-api-openapi.yml,\n  openapi/kontomatik-pdf-parsing-api-openapi.yml, openapi/kontomatik-report-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    acting: 13\n    connected: 17\n  by_consequence:\n    write: 13\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /signin/redirection\n  method: post\n  operationId: initiateRedirectionSignIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /signin/redirection-status\n  method: get\n  operationId: getRedirectionSignInStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /command/default-import.xml\n  method: post\n  operationId: startDefaultImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /command/{id}.xml\n  method: get\n  operationId: getCommandById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /command/reuse-multiple-access.xml\n  method: post\n  operationId: reuseMultipleAccess\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /command/delete-multiple-access.xml\n  method: post\n  operationId: deleteMultipleAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mock-session.xml\n  method: post\n  operationId: createMockSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ais-catalog\n  method:\
  \ get\n  operationId: getAisCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labeling\n  method: get\n  operationId: getLabeling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external-data-labeling\n  method: post\n  operationId: labelExternalData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vendors\n  method: get\n  operationId:\
  \ getVendors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /score\n  method: get\n  operationId: getScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /owner-features\n  method: get\n  operationId: getOwnerFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-summary\n  method: get\n  operationId: getDataSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /data-summary-catalog\n  method: get\n  operationId: getDataSummaryCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /income-confirmation\n  method: get\n  operationId: getIncomeConfirmation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/aggregated\n  method: get\n  operationId: getAggregatedData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/delete\n  method: post\n  operationId: deleteOwnerData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /owner-upload\n  method: post\n  operationId: uploadOwnerData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pdf/statement\n  method: post\n  operationId: parseStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pdf/statement-trusted\n  method: post\n  operationId: parseStatementTrusted\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pdf/statements\n  method: get\n  operationId: listStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pdf/confirmation\n  method: post\n  operationId: parseConfirmation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pdf/confirmation-trusted\n  method: post\n  operationId: parseConfirmationTrusted\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /pdf-catalog\n  method: get\n  operationId: getPdfCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/token\n  method: post\n  operationId: createReportToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /report/tokens\n  method: get\n  operationId: listReportTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/{token}\n  method: get\n  operationId: getReportByToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kontomatik/refs/heads/main/agentic-access/kontomatik-agentic-access.yml
summary_line: 30 operations · 13 acting
tags:
- Open Banking
- PSD2
- AIS
- Bank Data Aggregation
- CEE
- KYC
- Credit Scoring
- Transaction Labeling
- PDF Parsing
---
