---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 14
api_specs:
- filename: ucsd-chat-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — chat
  slug: tritonai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-chat-api-openapi.yml
- filename: ucsd-completions-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — completions
  slug: tritonai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-completions-api-openapi.yml
- filename: ucsd-embeddings-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — embeddings
  slug: tritonai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-embeddings-api-openapi.yml
- filename: ucsd-models-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — models
  slug: tritonai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-models-api-openapi.yml
- filename: ucsd-images-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — images
  slug: tritonai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-images-api-openapi.yml
- filename: ucsd-audio-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — audio
  slug: tritonai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-audio-api-openapi.yml
- filename: ucsd-scim-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — SCIM 2.0 provisioning
  slug: tritonai-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-scim-api-openapi.yml
- filename: ucsd-objects-api-openapi.yml
  format: yaml
  label: University of California, San Diego Objects API
  slug: ucsd-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-objects-api-openapi.yml
- filename: ucsd-search-api-openapi.yml
  format: yaml
  label: University of California, San Diego Search API
  slug: ucsd-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-search-api-openapi.yml
consequence_counts:
  read: 14
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ucsd Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'University of California, San Diego exposes 28 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: University of California, San Diego
provider_slug: ucsd
slug: ucsd-agentic-access
source_filename: ucsd-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/ucsd-audio-api-openapi.yml, openapi/ucsd-chat-api-openapi.yml, openapi/ucsd-completions-api-openapi.yml,\n  openapi/ucsd-embeddings-api-openapi.yml, openapi/ucsd-images-api-openapi.yml, openapi/ucsd-models-api-openapi.yml,\n  openapi/ucsd-objects-api-openapi.yml, openapi/ucsd-scim-api-openapi.yml, openapi/ucsd-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 14\n    connected: 14\n  by_consequence:\n    write: 14\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /audio/speech\n  method: post\n  operationId: audio_speech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/transcriptions\n  method: post\n  operationId: audio_transcriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chat/completions\n  method: post\n  operationId: chat_completion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/completions\n  method: post\n  operationId: completion\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/embeddings\n  method: post\n  operationId: embeddings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/images/generations\n  method: post\n  operationId: image_generation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/models\n  method: get\n  operationId: model_list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dc/object/{id}.json\n  method: get\n  operationId: getDigitalObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dc/collection/{id}.json\n  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2\n  method: get\n  operationId: get_scim_base_scim_v2_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Groups\n  method: get\n  operationId: get_groups_scim_v2_Groups_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Groups\n  method: post\n  operationId: create_group_scim_v2_Groups_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Groups/{group_id}\n  method: delete\n  operationId: delete_group_scim_v2_Groups__group_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Groups/{group_id}\n  method: get\n  operationId: get_group_scim_v2_Groups__group_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Groups/{group_id}\n  method: patch\n  operationId: patch_group_scim_v2_Groups__group_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Groups/{group_id}\n  method: put\n  operationId: update_group_scim_v2_Groups__group_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/ResourceTypes\n  method: get\n  operationId: get_resource_types_scim_v2_ResourceTypes_get\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/ResourceTypes/{resource_type_id}\n  method: get\n  operationId: get_resource_type_scim_v2_ResourceTypes__resource_type_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Schemas\n  method: get\n  operationId: get_schemas_scim_v2_Schemas_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Schemas/{schema_id}\n  method: get\n  operationId: get_schema_scim_v2_Schemas__schema_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/ServiceProviderConfig\n  method: get\n  operationId: get_service_provider_config_scim_v2_ServiceProviderConfig_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Users\n  method: get\n  operationId: get_users_scim_v2_Users_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Users\n  method: post\n  operationId: create_user_scim_v2_Users_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Users/{user_id}\n  method: delete\n  operationId: delete_user_scim_v2_Users__user_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Users/{user_id}\n  method: get\n  operationId: get_user_scim_v2_Users__user_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Users/{user_id}\n  method: patch\n  operationId: patch_user_scim_v2_Users__user_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Users/{user_id}\n  method: put\n  operationId: update_user_scim_v2_Users__user_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dc/search.json\n  method: get\n  operationId: searchDigitalCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/agentic-access/ucsd-agentic-access.yml
summary_line: 28 operations · 14 acting
tags:
- Education
- Higher Education
- University
- Public Research University
- UC System
- United States
- California
- Research
- Research Data
- Digital Collections
- Identity Federation
- API Gateway
- Artificial Intelligence
- Research Computing
---
