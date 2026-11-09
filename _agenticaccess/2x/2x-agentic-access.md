---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 25
api_specs:
- filename: 2x-alignment-api-openapi.yml
  format: yaml
  label: 2X Alignment API
  slug: 2x-alignment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/2x/openapi/2x-alignment-api-openapi.yml
- filename: 2x-api-keys-api-openapi.yml
  format: yaml
  label: 2X API Keys API
  slug: 2x-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/2x/openapi/2x-api-keys-api-openapi.yml
- filename: 2x-clients-api-openapi.yml
  format: yaml
  label: 2X Clients API
  slug: 2x-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/2x/openapi/2x-clients-api-openapi.yml
- filename: 2x-documentation-api-openapi.yml
  format: yaml
  label: 2X Documentation API
  slug: 2x-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/2x/openapi/2x-documentation-api-openapi.yml
- filename: 2x-health-api-openapi.yml
  format: yaml
  label: 2X Health API
  slug: 2x-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/2x/openapi/2x-health-api-openapi.yml
- filename: 2x-portfolios-api-openapi.yml
  format: yaml
  label: 2X Portfolios API
  slug: 2x-portfolios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/2x/openapi/2x-portfolios-api-openapi.yml
- filename: 2x-root-api-openapi.yml
  format: yaml
  label: 2X Root API
  slug: 2x-root-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/2x/openapi/2x-root-api-openapi.yml
- filename: 2x-status-api-openapi.yml
  format: yaml
  label: 2X Status API
  slug: 2x-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/2x/openapi/2x-status-api-openapi.yml
- filename: 2x-streams-api-openapi.yml
  format: yaml
  label: 2X Streams API
  slug: 2x-streams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/2x/openapi/2x-streams-api-openapi.yml
- filename: 2x-topics-api-openapi.yml
  format: yaml
  label: 2X Topics API
  slug: 2x-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/2x/openapi/2x-topics-api-openapi.yml
consequence_counts:
  read: 25
  safety-critical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: 2X Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/api-keys/{key_id}
operation_count: 27
overview: '2X exposes 27 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 1 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 2X
provider_slug: 2x
slug: 2x-agentic-access
source_filename: 2x-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/2x-alignment-api-openapi.yml, openapi/2x-api-keys-api-openapi.yml, openapi/2x-clients-api-openapi.yml,\n  openapi/2x-documentation-api-openapi.yml, openapi/2x-health-api-openapi.yml, openapi/2x-portfolios-api-openapi.yml,\n  openapi/2x-root-api-openapi.yml, openapi/2x-status-api-openapi.yml, openapi/2x-streams-api-openapi.yml,\n  openapi/2x-topics-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 25\n    acting: 2\n  by_consequence:\n    read: 25\n    write: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/clients/alignment\n  method: get\n  operationId: list_client_alignments_v1_clients_alignment_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{client_id}/alignment\n  method: get\n  operationId: get_client_alignment_v1_clients__client_id__alignment_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys\n  method: post\n  operationId: create_api_key_v1_api_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api-keys\n  method: get\n  operationId: list_api_keys_v1_api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/api-keys/{key_id}\n  method: delete\n  operationId: revoke_api_key_v1_api_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/clients\n  method: get\n  operationId: list_clients_v1_clients_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/portfolio-health\n  method: get\n  operationId: get_portfolio_health_v1_clients_portfolio_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/trending\n  method: get\n  operationId: get_trending_clients_v1_clients_trending_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/search\n  method: get\n  operationId: search_clients_v1_clients_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/statistics/overview\n  method: get\n  operationId: get_statistics_v1_clients_statistics_overview_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/export/csv\n  method: get\n  operationId: export_clients_csv_v1_clients_export_csv_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/by-risk/{risk_level}\n  method: get\n  operationId: get_clients_by_risk_v1_clients_by_risk__risk_level__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{client_id}\n  method: get\n  operationId: get_client_v1_clients__client_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{client_id}/history\n  method: get\n  operationId: get_client_history_v1_clients__client_id__history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{client_id}/priorities\n  method: get\n  operationId: get_client_priorities_v1_clients__client_id__priorities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{client_id}/notes\n  method: get\n\
  \  operationId: get_client_notes_v1_clients__client_id__notes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{client_id}/key-people\n  method: get\n  operationId: get_client_key_people_v1_clients__client_id__key_people_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{client_id}/streams\n  method: get\n  operationId: list_client_streams_v1_clients__client_id__streams_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clients/{client_id}/streams/{stream_id}\n  method: get\n  operationId: get_stream_v1_clients__client_id__streams__stream_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /docs\n  method: get\n  operationId: documentation_docs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/portfolios\n  method: get\n  operationId: list_portfolios_v1_portfolios_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/portfolios/{portfolio_id}\n  method: get\n  operationId: get_portfolio_v1_portfolios__portfolio_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method:\
  \ get\n  operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: status_page_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/streams\n  method: get\n  operationId: list_all_streams_v1_streams_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/topics\n  method: get\n  operationId: list_topics_v1_topics_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/2x/agentic-access/2x-agentic-access.yml
summary_line: 27 operations · 2 acting · 1 human-in-the-loop
tags:
- Company
- Marketing
- Marketing as a Service
- B2B
- MarTech
- Marketing Operations
- Consulting
- Artificial Intelligence
- Go-To-Market
- Revenue Operations
- Commercial Intelligence
- Customer Success
- AI Agents
- Demand Generation
---
