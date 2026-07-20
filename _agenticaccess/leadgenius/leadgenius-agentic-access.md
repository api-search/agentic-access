---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 6
api_specs:
- filename: leadgenius-enrichment-api-openapi.yml
  format: yaml
  label: LeadGenius Enrichment API
  slug: leadgenius-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadgenius/refs/heads/main/openapi/leadgenius-enrichment-api-openapi.yml
consequence_counts:
  read: 6
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Leadgenius Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'LeadGenius exposes 11 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LeadGenius
provider_slug: leadgenius
slug: leadgenius-agentic-access
source_filename: leadgenius-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/leadgenius-enrichment-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 5\n    connected: 6\n  by_consequence:\n    write: 5\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/enrichment/campaigns/\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/enrichment/upload/{slug}/\n  method: get\n  operationId: getUploadRequestSample\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/enrichment/upload/{slug}/\n  method: post\n  operationId: uploadRecordsToCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/enrichment/update/{slug}/\n  method: patch\n  operationId: updateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/enrichment/retrieve/{slug}/\n  method: get\n  operationId: retrieveCampaignRecords\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/enrichment/status/\n  method: get\n  operationId: getApiUsageStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/exclusion/upload/\n  method: post\n  operationId: uploadExclusionRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/enrichment/rapid/\n  method: post\n  operationId: createRapidEnrichmentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/enrichment/rapid/\n  method: get\n  operationId: listEnrichmentRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/enrichment/rapid/{id}/\n  method: get\n  operationId: retrieveEnrichedRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/enrichment/rapid/stats/\n  method: get\n  operationId: getEnrichmentStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadgenius/refs/heads/main/agentic-access/leadgenius-agentic-access.yml
summary_line: 11 operations · 5 acting
tags:
- Company
- Data Enrichment
- Lead Generation
- Sales
- Marketing
- B2B Data
- Contact Data
- Firmographics
- Go To Market
- Account Based Marketing
---
