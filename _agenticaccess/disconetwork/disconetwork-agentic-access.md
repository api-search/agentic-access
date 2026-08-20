---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: disconetwork-partner-api.yml
  format: yaml
  label: Disco Partner Integration API
  slug: disconetwork-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disconetwork/refs/heads/main/openapi/disconetwork-partner-api.yml
- filename: disconetwork-reporting-api-v1.yml
  format: yaml
  label: Disco Reporting API
  slug: disconetwork-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disconetwork/refs/heads/main/openapi/disconetwork-reporting-api-v1.yml
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Disconetwork Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Disconetwork exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Disconetwork
provider_slug: disconetwork
slug: disconetwork-agentic-access
source_filename: disconetwork-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: generated\nsource: openapi/disconetwork-partner-api.yml, openapi/disconetwork-reporting-api-v1.yml, openapi/disconetwork-reporting-api-v2.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 3\n    connected: 3\n  by_consequence:\n    write: 3\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /events\n  method: post\n  operationId: createAnEventUsedToRecordUserActions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/batch\n\
  \  method: post\n  operationId: createABatchOfEventsUsedToRecordUserActions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recommendations\n  method: post\n  operationId: getDiscoAdvertiserRecommendations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discobeat/reporting/v1/summary/\n  method: get\n  operationId: getReportingSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discobeat/reporting/v1/publishers/\n\
  \  method: get\n  operationId: getReportingPublishers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discobeat/reporting/v2/report/\n  method: get\n  operationId: getReportingV2Report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/disconetwork/refs/heads/main/agentic-access/disconetwork-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- Company
- Commerce Media
- Retail Media
- Post-Purchase
- Advertising
- E-Commerce
- AdTech
- Marketing
- Analytics
- Reporting
---
