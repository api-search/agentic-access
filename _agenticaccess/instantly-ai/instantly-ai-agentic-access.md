---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 5
api_specs:
- filename: api_v2.json
  format: json
  label: Instantly Campaigns API
  slug: campaigns-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Leads API
  slug: leads-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Accounts API
  slug: accounts-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Email Verification API
  slug: email-verification-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Inbox Placement Test API
  slug: inbox-placement-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Analytics API
  slug: analytics-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly API Keys API
  slug: api-keys-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
- filename: api_v2.json
  format: json
  label: Instantly Workspaces API
  slug: workspaces-api
  spec_type: OpenAPI
  url: https://api.instantly.ai/openapi/api_v2.json
consequence_counts:
  read: 5
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Instantly Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Instantly exposes 13 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Instantly
provider_slug: instantly-ai
slug: instantly-ai-agentic-access
source_filename: instantly-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/instantly-ai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 5\n    acting: 8\n  by_consequence:\n    read: 5\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/campaigns\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/campaigns/{id}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/campaigns/{id}\n  method: patch\n  operationId: updateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/campaigns/{id}\n  method: delete\n  operationId: deleteCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v2/campaigns/{id}/activate\n  method: post\n  operationId: activateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/campaigns/{id}/pause\n  method: post\n  operationId: pauseCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/campaigns/search-by-contact\n  method: get\n  operationId: searchCampaignsByContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v2/campaigns/{id}/share\n  method: post\n  operationId: shareCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/campaigns/{id}/duplicate\n  method: post\n  operationId: duplicateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/campaigns/{id}/export\n  method: post\n  operationId: exportCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/campaigns/count-launched\n  method: get\n  operationId: countLaunchedCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/campaigns/{id}/sending-status\n  method: get\n  operationId: getSendingStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instantly-ai/refs/heads/main/agentic-access/instantly-ai-agentic-access.yml
summary_line: 13 operations · 8 acting
tags:
- Cold Email
- Outbound
- Sales
- Deliverability
- Lead Database
- Email Verification
- Webhooks
---
