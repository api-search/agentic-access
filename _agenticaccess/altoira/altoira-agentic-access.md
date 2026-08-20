---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 6
api_specs:
- filename: altoira-handoffs-api-openapi.yml
  format: yaml
  label: AltoIRA Handoffs API
  slug: altoira-handoffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-handoffs-api-openapi.yml
- filename: altoira-investment-api-openapi.yml
  format: yaml
  label: AltoIRA Investment API
  slug: altoira-investment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-investment-api-openapi.yml
- filename: altoira-oauth-api-openapi.yml
  format: yaml
  label: AltoIRA OAUTH API
  slug: altoira-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-oauth-api-openapi.yml
- filename: altoira-offering-api-openapi.yml
  format: yaml
  label: AltoIRA Offering API
  slug: altoira-offering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-offering-api-openapi.yml
- filename: altoira-user-api-openapi.yml
  format: yaml
  label: AltoIRA User API
  slug: altoira-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/openapi/altoira-user-api-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Altoira Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/platform/investment/{external_id}/{alto_user_id}/refund
operation_count: 17
overview: 'AltoIRA exposes 17 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 10 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AltoIRA
provider_slug: altoira
slug: altoira-agentic-access
source_filename: altoira-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: generated\nsource: openapi/altoira-partner-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 6\n    acting: 11\n  by_consequence:\n    read: 6\n    write: 10\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/authorize\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offering/platform/{platform_code}/{external_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/token\n  method: post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/user\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user\n  method: put\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/offerings\n  method: get\n  operationId: getOfferings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/platform/offering/{external_id}\n  method: get\n  operationId: getOffering\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/offering/{external_id}\n  method: post\n  operationId: createOffering\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/offering/{external_id}\n  method: put\n  operationId: updateOffering\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/platform/offering/{external_id}/documents\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/offering/{external_id}/documents_as_zip\n  method: post\n  operationId: createDocumentViaZip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/offering/{external_id}/enable_for_investor/{alto_user_id}\n  method: put\n  operationId: enableOffering\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/offering/{external_id}/{alto_user_id}/investment\n  method: get\n  operationId: getInvestment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/investment/{external_id}/{alto_user_id}/refund\n  method: post\n  operationId: investmentRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/investment/{external_id}/{alto_user_id}/cancel\n  method: post\n  operationId: investmentCancel\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/investment/{external_id}/{alto_user_id}/distribution\n  method: post\n  operationId: investmentDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/platform/investment/{external_id}/{alto_user_id}/issue_new_capital_call\n  method: post\n  operationId: issueNewCapitalCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altoira/refs/heads/main/agentic-access/altoira-agentic-access.yml
summary_line: 17 operations · 11 acting
tags:
- Company
- Financial-Services
- Retirement
- Self-Directed IRA
- Alternative Investments
- Private Markets
- Fintech
- Custody
- Cryptocurrency
- Wealth Management
- Investing
- Capital Raising
---
