---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 17
api_specs:
- filename: bridge-mls-agents-api-openapi.yml
  format: yaml
  label: Bridge Agents API
  slug: bridge-mls-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-agents-api-openapi.yml
- filename: bridge-mls-listings-api-openapi.yml
  format: yaml
  label: Bridge Listings API
  slug: bridge-mls-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-listings-api-openapi.yml
- filename: bridge-mls-media-api-openapi.yml
  format: yaml
  label: Bridge Media API
  slug: bridge-mls-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-media-api-openapi.yml
- filename: bridge-mls-member-api-openapi.yml
  format: yaml
  label: Bridge Member API
  slug: bridge-mls-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-member-api-openapi.yml
- filename: bridge-mls-metadata-api-openapi.yml
  format: yaml
  label: Bridge Metadata API
  slug: bridge-mls-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-metadata-api-openapi.yml
- filename: bridge-mls-office-api-openapi.yml
  format: yaml
  label: Bridge Office API
  slug: bridge-mls-office-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-office-api-openapi.yml
- filename: bridge-mls-offices-api-openapi.yml
  format: yaml
  label: Bridge Offices API
  slug: bridge-mls-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-offices-api-openapi.yml
- filename: bridge-mls-openhouse-api-openapi.yml
  format: yaml
  label: Bridge OpenHouse API
  slug: bridge-mls-openhouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-openhouse-api-openapi.yml
- filename: bridge-mls-openhouses-api-openapi.yml
  format: yaml
  label: Bridge OpenHouses API
  slug: bridge-mls-openhouses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-openhouses-api-openapi.yml
- filename: bridge-mls-property-api-openapi.yml
  format: yaml
  label: Bridge Property API
  slug: bridge-mls-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-property-api-openapi.yml
- filename: bridge-mls-webhooks-api-openapi.yml
  format: yaml
  label: Bridge Webhooks API
  slug: bridge-mls-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/openapi/bridge-mls-webhooks-api-openapi.yml
consequence_counts:
  read: 17
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bridge Mls Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Bridge exposes 21 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bridge
provider_slug: bridge-mls
slug: bridge-mls-agentic-access
source_filename: bridge-mls-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bridge-reso-web-api-openapi.yml, openapi/bridge-web-api-openapi.yml, openapi/bridge-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 17\n    acting: 4\n  by_consequence:\n    read: 17\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /{dataset}\n  method: get\n  operationId: getServiceDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/$metadata\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/Property\n  method: get\n  operationId: listProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/Property('{listingKey}')\n  method: get\n  operationId: getProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/Member\n  method: get\n  operationId: listMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/Member('{memberKey}')\n  method: get\n  operationId: getMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/Office\n  method: get\n  operationId:\
  \ listOffices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/Office('{officeKey}')\n  method: get\n  operationId: getOffice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/OpenHouse\n  method: get\n  operationId: listOpenHouses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/Media\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/listings\n  method: get\n  operationId: listListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /{dataset}/listings/{listingId}\n  method: get\n  operationId: getListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/offices\n  method: get\n  operationId: listOffices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/openhouses\n  method: get\n  operationId: listOpenHouses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{dataset}/webhooks/{webhookId}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{dataset}/webhooks/{webhookId}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{dataset}/webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{dataset}/webhooks/{webhookId}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridge-mls/refs/heads/main/agentic-access/bridge-mls-agentic-access.yml
summary_line: 21 operations · 4 acting
tags:
- Real-Estate
- MLS
- RESO
- Listings
- Property Data
- Brokers
- Data Distribution
---
