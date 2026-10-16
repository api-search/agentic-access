---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 12
api_specs:
- filename: liquilens-agent-query-api-openapi.yml
  format: yaml
  label: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs Agent Query API
  slug: liquilens-agent-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/openapi/liquilens-agent-query-api-openapi.yml
- filename: liquilens-agent-review-api-openapi.yml
  format: yaml
  label: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs Agent Review API
  slug: liquilens-agent-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/openapi/liquilens-agent-review-api-openapi.yml
- filename: liquilens-applications-api-openapi.yml
  format: yaml
  label: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs Applications API
  slug: liquilens-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/openapi/liquilens-applications-api-openapi.yml
- filename: liquilens-datasets-api-openapi.yml
  format: yaml
  label: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs Datasets API
  slug: liquilens-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/openapi/liquilens-datasets-api-openapi.yml
- filename: liquilens-financial-evidence-for-openbb-api-openapi.yml
  format: yaml
  label: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs Financial Evidence For OpenBB API
  slug: liquilens-financial-evidence-for-openbb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/openapi/liquilens-financial-evidence-for-openbb-api-openapi.yml
- filename: liquilens-funding-review-api-openapi.yml
  format: yaml
  label: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs Funding Review API
  slug: liquilens-funding-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/openapi/liquilens-funding-review-api-openapi.yml
- filename: liquilens-funding-review-csv-api-openapi.yml
  format: yaml
  label: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs Funding Review.csv API
  slug: liquilens-funding-review-csv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/openapi/liquilens-funding-review-csv-api-openapi.yml
- filename: liquilens-guide-api-openapi.yml
  format: yaml
  label: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs Guide API
  slug: liquilens-guide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/openapi/liquilens-guide-api-openapi.yml
- filename: liquilens-healthz-api-openapi.yml
  format: yaml
  label: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs Healthz API
  slug: liquilens-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/openapi/liquilens-healthz-api-openapi.yml
- filename: liquilens-packet-api-openapi.yml
  format: yaml
  label: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs Packet API
  slug: liquilens-packet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/openapi/liquilens-packet-api-openapi.yml
- filename: liquilens-query-api-openapi.yml
  format: yaml
  label: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs Query API
  slug: liquilens-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/openapi/liquilens-query-api-openapi.yml
- filename: liquilens-release-api-openapi.yml
  format: yaml
  label: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs Release API
  slug: liquilens-release-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/openapi/liquilens-release-api-openapi.yml
- filename: liquilens-sources-api-openapi.yml
  format: yaml
  label: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs Sources API
  slug: liquilens-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/openapi/liquilens-sources-api-openapi.yml
consequence_counts:
  read: 12
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Liquilens Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs exposes 14 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LIQUILENS PRIVATE LIMITED -- LiquiLens financial research APIs
provider_slug: liquilens
slug: liquilens-agentic-access
source_filename: liquilens-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: generated\nsource: openapi/liquilens-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 2\n    connected: 12\n  by_consequence:\n    write: 2\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/applications\n  method: post\n  operationId: enroll_api_v1_applications_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/applications/current\n  method: delete\n  operationId: erase_api_v1_applications_current_delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: index__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: get\n  operationId: health_healthz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/release\n  method: get\n  operationId: release_api_v1_release_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funding-review\n  method: get\n  operationId: funding_review_api_v1_funding_review_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funding-review.csv\n  method: get\n  operationId: funding_review_csv_api_v1_funding_review_csv_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /guide\n  method: get\n  operationId: guide_guide_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/datasets\n  method: get\n  operationId: datasets_api_v1_datasets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/query\n  method: get\n  operationId: query_api_v1_query_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sources\n  method: get\n  operationId: sources_api_v1_sources_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packet\n  method: get\n  operationId: packet_api_v1_packet_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent-query\n  method: get\n  operationId: agent_query_api_v1_agent_query_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent-review\n  method: get\n  operationId: agent_review_api_v1_agent_review_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquilens/refs/heads/main/agentic-access/liquilens-agentic-access.yml
summary_line: 14 operations · 2 acting
tags:
- Company
- Finance
- Research
- API
- Data
---
