---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 17
api_specs:
- filename: 0si-ai-companies-api-openapi.yml
  format: yaml
  label: 공시.ai Companies API
  slug: 0si-ai-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-companies-api-openapi.yml
- filename: 0si-ai-disclosures-api-openapi.yml
  format: yaml
  label: 공시.ai Disclosures API
  slug: 0si-ai-disclosures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-disclosures-api-openapi.yml
- filename: 0si-ai-sec-api-openapi.yml
  format: yaml
  label: 공시.ai Sec API
  slug: 0si-ai-sec-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-sec-api-openapi.yml
- filename: 0si-ai-status-api-openapi.yml
  format: yaml
  label: 공시.ai Status API
  slug: 0si-ai-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-status-api-openapi.yml
- filename: 0si-ai-stream-api-openapi.yml
  format: yaml
  label: 공시.ai Stream API
  slug: 0si-ai-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-stream-api-openapi.yml
- filename: 0si-ai-usage-api-openapi.yml
  format: yaml
  label: 공시.ai Usage API
  slug: 0si-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-usage-api-openapi.yml
- filename: 0si-ai-webhooks-api-openapi.yml
  format: yaml
  label: 공시.ai Webhooks API
  slug: 0si-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0si-ai/openapi/0si-ai-webhooks-api-openapi.yml
consequence_counts:
  read: 17
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 0Si Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: '공시.ai exposes 22 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 공시.ai
provider_slug: 0si-ai
slug: 0si-ai-agentic-access
source_filename: 0si-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/0si-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 17\n    acting: 5\n  by_consequence:\n    read: 17\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies\n  method: get\n  operationId: listCompanies\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{stock_code}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{stock_code}/fundamentals/history\n  method: get\n  operationId: listCompanyFundamentalHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disclosures\n  method: get\n  operationId: listDisclosures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sec/filings\n  method: get\n  operationId: listSecFilings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /sec/filings/{accession_number}\n  method: get\n  operationId: getSecFiling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sec/filings/{accession_number}/delta\n  method: get\n  operationId: getSecFilingDelta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disclosures/{disclosure_id}\n  method: get\n  operationId: getDisclosure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disclosures/{disclosure_id}/delta\n  method: get\n  operationId: getDisclosureDelta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /disclosures/{disclosure_id}/revisions\n  method: get\n  operationId: getDisclosureRevisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disclosures/{disclosure_id}/market-reaction\n  method: get\n  operationId: getMarketReaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}/rotate-secret\n  method: post\n  operationId: rotateWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}/deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stream\n  method: get\n  operationId: streamDisclosures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sec/stream\n  method: get\n  operationId: streamSecFilings\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/0si-ai/agentic-access/0si-ai-agentic-access.yml
summary_line: 22 operations · 5 acting
tags:
- Artificial Intelligence
- Finance
- Filings
- South Korea
- USA
---
