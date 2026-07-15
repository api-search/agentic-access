---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 14
api_specs:
- filename: outbrain-amplify-api-openapi.yml
  format: yaml
  label: Outbrain Amplify API
  slug: outbrain-amplify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-amplify-api-openapi.yml
- filename: outbrain-engage-api-openapi.yml
  format: yaml
  label: Outbrain Engage API
  slug: outbrain-engage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-engage-api-openapi.yml
- filename: outbrain-teads-conversion-api-openapi.yml
  format: yaml
  label: Teads / Outbrain Conversion API
  slug: outbrain-teads-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/openapi/outbrain-teads-conversion-api-openapi.yml
consequence_counts:
  physical: 2
  read: 14
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Outbrain Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /capi/event
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /capi/event/batch
operation_count: 24
overview: 'Outbrain exposes 24 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 8 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Outbrain
provider_slug: outbrain
slug: outbrain-agentic-access
source_filename: outbrain-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/outbrain-amplify-api-openapi.yml, openapi/outbrain-engage-api-openapi.yml, openapi/outbrain-teads-conversion-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 14\n    acting: 10\n  by_consequence:\n    read: 14\n    write: 8\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /login\n  method: get\n  operationId: login\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketers\n  method: get\n  operationId: listMarketers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketers/{marketerId}\n  method: get\n  operationId: getMarketer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketers/{marketerId}/campaigns\n  method: get\n  operationId: listCampaignsByMarketer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketers/{marketerId}/campaigns\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{campaignId}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{campaignId}\n  method: put\n  operationId: updateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{campaignId}/promotedLinks\n  method: get\n  operationId: listPromotedLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{campaignId}/promotedLinks\n  method: post\n  operationId: createPromotedLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /promotedLinks/{promotedLinkId}\n  method: get\n  operationId: getPromotedLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /promotedLinks/{promotedLinkId}\n  method: put\n  operationId: updatePromotedLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /marketers/{marketerId}/budgets\n  method: get\n  operationId: listBudgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketers/{marketerId}/budgets\n  method: post\n  operationId: createBudget\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /budgets/{budgetId}\n  method: get\n  operationId: getBudget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{campaignId}/targeting/audience\n  method: get\n  operationId: getAudienceTargeting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{campaignId}/targeting/audience\n  method: put\n  operationId: updateAudienceTargeting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/marketers/{marketerId}/campaigns\n  method: get\n  operationId: reportPerformanceByCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/marketers/{marketerId}/periodicContent\n  method: get\n  operationId: reportPerformanceByPeriodicContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/marketers/{marketerId}/realtime\n  method: get\n  operationId: reportPerformanceRealtime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /utils/get\n  method: get\n  operationId: getRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/impression\n  method: post\n  operationId: reportImpression\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /report/click\n  method: post\n  operationId: reportClick\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /capi/event\n  method: post\n  operationId: sendConversionEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /capi/event/batch\n  method: post\n  operationId: sendConversionEventBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outbrain/refs/heads/main/agentic-access/outbrain-agentic-access.yml
summary_line: 24 operations · 10 acting
tags:
- Advertising
- Native Advertising
- Open Web
- CTV
- Connected TV
- Video Advertising
- Content Discovery
- Programmatic
- Performance Marketing
- AdTech
- Teads
---
