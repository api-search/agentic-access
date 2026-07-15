---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 8
api_specs:
- filename: looker-studio-api-openapi.yml
  format: yaml
  label: Looker Studio API
  slug: looker-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-api-openapi.yml
- filename: looker-studio-linking-api-openapi.yml
  format: yaml
  label: Looker Studio Linking API
  slug: looker-studio-linking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-linking-api-openapi.yml
- filename: looker-studio-embedding-api-openapi.yml
  format: yaml
  label: Looker Studio Embedding API
  slug: looker-studio-embedding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-embedding-api-openapi.yml
- filename: looker-studio-community-connector-api-openapi.yml
  format: yaml
  label: Looker Studio Community Connector API
  slug: looker-studio-community-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-community-connector-api-openapi.yml
- filename: looker-studio-community-visualization-api-openapi.yml
  format: yaml
  label: Looker Studio Community Visualization API
  slug: looker-studio-community-visualization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-community-visualization-api-openapi.yml
consequence_counts:
  read: 8
  safety-critical: 1
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Looker Studio Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /assets/{assetId}/permissions:revokeAllPermissions
operation_count: 18
overview: 'Looker Studio exposes 18 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 9 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Looker Studio
provider_slug: looker-studio
slug: looker-studio-agentic-access
source_filename: looker-studio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/looker-studio-api-openapi.yml, openapi/looker-studio-community-connector-api-openapi.yml,\n  openapi/looker-studio-community-visualization-api-openapi.yml, openapi/looker-studio-embedding-api-openapi.yml,\n  openapi/looker-studio-linking-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 8\n    acting: 10\n  by_consequence:\n    read: 8\n    write: 9\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /assets:search\n  method: get\n  operationId: searchAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /assets/{assetId}/permissions\n  method: get\n  operationId: getAssetPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{assetId}/permissions\n  method: patch\n  operationId: updateAssetPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{assetId}/permissions:addMembers\n  method: post\n  operationId: addAssetMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{assetId}/permissions:revokeAllPermissions\n\
  \  method: post\n  operationId: revokeAllAssetPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /connector/getAuthType\n  method: post\n  operationId: getAuthType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connector/isAuthValid\n  method: post\n  operationId: isAuthValid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connector/setCredentials\n  method: post\n  operationId: setCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connector/getConfig\n  method: post\n  operationId: getConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connector/getSchema\n  method: post\n  operationId: getSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connector/getData\n  method: post\n  operationId: getData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /visualization\n  method: get\n  operationId: listCommunityVisualizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visualization/load\n  method: post\n  operationId: loadVisualization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /visualization/manifest\n  method: get\n  operationId: getVisualizationManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /embed/reporting/{reportId}/page/{pageId}\n  method: get\n  operationId: getEmbeddedReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /embed/reporting/{reportId}\n  method: get\n  operationId: getEmbeddedReportDefault\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /s/{shortId}\n  method: get\n  operationId: getSharedReportByShortLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /reporting/create\n  method: get\n  operationId: createLinkedReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/agentic-access/looker-studio-agentic-access.yml
summary_line: 18 operations · 10 acting · 1 human-in-the-loop
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Reports
---
