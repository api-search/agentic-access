---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 35
api_specs:
- filename: audioscrape-com-account-api-openapi.yml
  format: yaml
  label: Audioscrape Account API
  slug: audioscrape-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-account-api-openapi.yml
- filename: audioscrape-com-agent-rail-api-openapi.yml
  format: yaml
  label: Audioscrape Agent rail API
  slug: audioscrape-com-agent-rail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-agent-rail-api-openapi.yml
- filename: audioscrape-com-api-keys-api-openapi.yml
  format: yaml
  label: Audioscrape API Keys API
  slug: audioscrape-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-api-keys-api-openapi.yml
- filename: audioscrape-com-charts-api-openapi.yml
  format: yaml
  label: Audioscrape Charts API
  slug: audioscrape-com-charts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-charts-api-openapi.yml
- filename: audioscrape-com-data-export-api-openapi.yml
  format: yaml
  label: Audioscrape Data Export API
  slug: audioscrape-com-data-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-data-export-api-openapi.yml
- filename: audioscrape-com-episodes-api-openapi.yml
  format: yaml
  label: Audioscrape Episodes API
  slug: audioscrape-com-episodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-episodes-api-openapi.yml
- filename: audioscrape-com-items-api-openapi.yml
  format: yaml
  label: Audioscrape Items API
  slug: audioscrape-com-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-items-api-openapi.yml
- filename: audioscrape-com-knowledge-graph-api-openapi.yml
  format: yaml
  label: Audioscrape Knowledge Graph API
  slug: audioscrape-com-knowledge-graph-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-knowledge-graph-api-openapi.yml
- filename: audioscrape-com-libraries-api-openapi.yml
  format: yaml
  label: Audioscrape Libraries API
  slug: audioscrape-com-libraries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-libraries-api-openapi.yml
- filename: audioscrape-com-persons-api-openapi.yml
  format: yaml
  label: Audioscrape Persons API
  slug: audioscrape-com-persons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-persons-api-openapi.yml
- filename: audioscrape-com-podcasts-api-openapi.yml
  format: yaml
  label: Audioscrape Podcasts API
  slug: audioscrape-com-podcasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-podcasts-api-openapi.yml
- filename: audioscrape-com-search-api-openapi.yml
  format: yaml
  label: Audioscrape Search API
  slug: audioscrape-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-search-api-openapi.yml
- filename: audioscrape-com-system-api-openapi.yml
  format: yaml
  label: Audioscrape System API
  slug: audioscrape-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-system-api-openapi.yml
- filename: audioscrape-com-workspaces-api-openapi.yml
  format: yaml
  label: Audioscrape Workspaces API
  slug: audioscrape-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/audioscrape-com/openapi/audioscrape-com-workspaces-api-openapi.yml
consequence_counts:
  read: 35
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Audioscrape Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 42
overview: 'Audioscrape exposes 42 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Audioscrape
provider_slug: audioscrape-com
slug: audioscrape-com-agentic-access
source_filename: audioscrape-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/audioscrape-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 35\n    acting: 7\n  by_consequence:\n    read: 35\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/agent/v1\n  method: get\n  operationId: manifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/v1/credits\n  method: get\n  operationId: credit_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/v1/credits\n\
  \  method: post\n  operationId: buy_credit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/v1/excerpt\n  method: get\n  operationId: excerpt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/v1/overview\n  method: get\n  operationId: overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/v1/search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/v1/transcribe\n\
  \  method: post\n  operationId: transcribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/v1/transcriptions/{job_id}\n  method: get\n  operationId: transcription_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/charts/podcasts\n  method: get\n  operationId: get_chart_podcasts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/datasets/{id}\n  method: get\n  operationId: get_dataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/datasets/{id}/items\n  method: post\n  operationId: upload_item_external\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/entities\n  method: get\n  operationId: search_entities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/entities/{entity_slug}\n  method: get\n  operationId: get_entity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/episodes\n  method: get\n  operationId: list_recent_episodes_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/episodes/{episode_id}\n  method: get\n  operationId: get_public_episode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/episodes/{episode_id}/transcript\n  method: get\n  operationId: get_episode_transcript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: get_health_openapi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/items\n  method: get\n  operationId: list_items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/items/{item_id}\n  method: get\n  operationId:\
  \ get_item\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/items/{item_id}/transcript\n  method: get\n  operationId: get_item_transcript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys\n  method: get\n  operationId: list_api_keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keys\n  method: post\n  operationId: create_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keys/{id}\n  method: delete\n  operationId:\
  \ delete_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keys/{id}/rotate\n  method: post\n  operationId: rotate_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/keys/{id}/usage\n  method: get\n  operationId: api_key_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/libraries\n  method: get\n  operationId: list_libraries\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/libraries/{slug}\n  method: get\n  operationId: get_library\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me\n  method: get\n  operationId: get_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/me/usage\n  method: get\n  operationId: get_me_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/persons\n  method: get\n  operationId: search_persons_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/persons/{person_slug}\n  method: get\n  operationId: get_person_v1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/podcasts\n  method: get\n  operationId: search_podcasts_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/podcasts/{podcast_id}\n  method: get\n  operationId: get_public_podcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/podcasts/{podcast_id}/episodes\n  method: get\n  operationId: list_podcast_episodes_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/podcasts/{podcast_id}/rankings\n  method: get\n  operationId: get_podcast_ranking_history\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: post\n  operationId: search_api_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/trending\n  method: get\n  operationId: get_real_trending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/workspaces\n  method: get\n  operationId: list_workspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/workspaces/{workspace}\n  method: get\n  operationId: get_workspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/workspaces/{workspace}/datasets\n\
  \  method: get\n  operationId: list_workspace_datasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/workspaces/{workspace}/export\n  method: post\n  operationId: create_workspace_export\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/workspaces/{workspace}/export/{job_id}\n  method: get\n  operationId: get_workspace_export\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/audioscrape-com/agentic-access/audioscrape-com-agentic-access.yml
summary_line: 42 operations · 7 acting
tags:
- Audio
- Artificial Intelligence
- Transcription
- Search
- MCP
---
