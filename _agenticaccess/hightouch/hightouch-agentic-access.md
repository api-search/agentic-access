---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 21
api_specs:
- filename: hightouch-api-openapi.json
  format: json
  label: Hightouch API
  slug: hightouch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/_original/hightouch-api-openapi.json
- filename: hightouch-sources-api-openapi.yml
  format: yaml
  label: Hightouch Sources API
  slug: hightouch-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-sources-api-openapi.yml
- filename: hightouch-models-api-openapi.yml
  format: yaml
  label: Hightouch Models API
  slug: hightouch-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-models-api-openapi.yml
- filename: hightouch-destinations-api-openapi.yml
  format: yaml
  label: Hightouch Destinations API
  slug: hightouch-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-destinations-api-openapi.yml
- filename: hightouch-syncs-api-openapi.yml
  format: yaml
  label: Hightouch Syncs API
  slug: hightouch-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-syncs-api-openapi.yml
- filename: hightouch-campaigns-api-openapi.yml
  format: yaml
  label: Hightouch Campaigns API
  slug: hightouch-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-campaigns-api-openapi.yml
- filename: hightouch-ai-decisioning-api-openapi.yml
  format: yaml
  label: Hightouch AI Decisioning API
  slug: hightouch-ai-decisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-ai-decisioning-api-openapi.yml
- filename: hightouch-events-api-openapi.yml
  format: yaml
  label: Hightouch Events API
  slug: hightouch-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-events-api-openapi.yml
- filename: hightouch-identity-resolution-api-openapi.yml
  format: yaml
  label: Hightouch Identity Resolution API
  slug: hightouch-identity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/openapi/hightouch-identity-resolution-api-openapi.yml
consequence_counts:
  physical: 1
  read: 21
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hightouch Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /campaigns/{campaignId}/trigger
operation_count: 43
overview: 'Hightouch exposes 43 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 21 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hightouch
provider_slug: hightouch
slug: hightouch-agentic-access
source_filename: hightouch-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/hightouch-ai-decisioning-api-openapi.yml, openapi/hightouch-campaigns-api-openapi.yml,\n  openapi/hightouch-destinations-api-openapi.yml, openapi/hightouch-events-api-openapi.yml,\n  openapi/hightouch-identity-resolution-api-openapi.yml, openapi/hightouch-models-api-openapi.yml,\n  openapi/hightouch-sources-api-openapi.yml, openapi/hightouch-syncs-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 21\n    acting: 22\n  by_consequence:\n    read: 21\n    write: 21\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /decision-engine/flow/{flowId}\n  method: get\n  operationId: GetFlow\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /decision-engine/flows\n  method: get\n  operationId: ListFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /decision-engine/flow/{flowId}/messages\n  method: get\n  operationId: ListMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /decision-engine/flow/{flowId}/messages\n  method: post\n  operationId: CreateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /decision-engine/flow/{flowId}/messages/{messageId}\n\
  \  method: get\n  operationId: GetMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /decision-engine/flow/{flowId}/messages/{messageId}\n  method: patch\n  operationId: UpdateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /decision-engine/flow/{flowId}/run\n  method: post\n  operationId: RunFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{campaignId}/trigger\n  method: post\n  operationId:\
  \ TriggerCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{campaignId}/sends/{sendId}\n  method: get\n  operationId: GetSendStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destinations/{destinationId}\n  method: get\n  operationId: GetDestination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destinations/{destinationId}\n  method: patch\n  operationId: UpdateDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /destinations\n  method: get\n  operationId: ListDestination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /destinations\n  method: post\n  operationId: CreateDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/contracts/{contractId}\n  method: get\n  operationId: GetContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/contracts/{contractId}\n\
  \  method: patch\n  operationId: UpdateContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/contracts\n  method: get\n  operationId: ListContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/contracts\n  method: post\n  operationId: CreateContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/domains/{domainId}\n  method: get\n  operationId: GetDomain\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/domains/{domainId}\n  method: patch\n  operationId: UpdateDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/domains\n  method: get\n  operationId: ListDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/domains\n  method: post\n  operationId: CreateDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /idr/{graphId}/trigger\n  method: post\n  operationId: TriggerIdrRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /idr/{graphId}/runs\n  method: get\n  operationId: ListIdrRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /idr/{graphId}/queue-for-reprocessing\n  method: post\n  operationId: QueueForReprocessing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /idr/{graphId}/reprocess-status/{requestId}\n\
  \  method: get\n  operationId: ReprocessStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /id_graphs/{graphId}/trigger\n  method: post\n  operationId: TriggerRunIdGraph\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{modelId}\n  method: get\n  operationId: GetModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{modelId}\n  method: patch\n  operationId: UpdateModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models\n  method: get\n  operationId: ListModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models\n  method: post\n  operationId: CreateModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sources/{sourceId}\n  method: get\n  operationId: GetSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources/{sourceId}\n  method: patch\n  operationId: UpdateSource\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sources\n  method: get\n  operationId: ListSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources\n  method: post\n  operationId: CreateSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /syncs/{syncId}\n  method: get\n  operationId: GetSync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /syncs/{syncId}\n  method:\
  \ patch\n  operationId: UpdateSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /syncs\n  method: get\n  operationId: ListSync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /syncs\n  method: post\n  operationId: CreateSync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /syncs/{syncId}/runs\n  method: get\n  operationId: ListSyncRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /syncs/{syncId}/trigger\n  method: post\n  operationId: TriggerRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /syncs/trigger\n  method: post\n  operationId: TriggerRunCustom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sync-sequences/{syncSequenceId}/trigger\n  method: post\n  operationId: TriggerSequenceRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sync-sequences/runs/{syncSequenceRunId}\n  method: get\n  operationId: GetSyncSequenceRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hightouch/refs/heads/main/agentic-access/hightouch-agentic-access.yml
summary_line: 43 operations · 22 acting
tags:
- CDP
- Data Activation
- Reverse ETL
- Audience Management
- Identity Resolution
- Event Collection
- Marketing
- Advertising
- AI Agents
- Data Warehouse
---
