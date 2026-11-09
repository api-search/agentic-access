---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 13
api_specs:
- filename: deepgram-voice-agent-asyncapi.yml
  format: yaml
  label: Deepgram Voice Agent API
  slug: voice-agent-api
  spec_type: AsyncAPI
  url: https://artifacts.apis.io/deepgram/asyncapi/deepgram-voice-agent-asyncapi.yml
- filename: deepgram-balances-api-openapi.yml
  format: yaml
  label: Deepgram Balances API
  slug: deepgram-balances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-balances-api-openapi.yml
- filename: deepgram-keys-api-openapi.yml
  format: yaml
  label: Deepgram Keys API
  slug: deepgram-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-keys-api-openapi.yml
- filename: deepgram-members-api-openapi.yml
  format: yaml
  label: Deepgram Members API
  slug: deepgram-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-members-api-openapi.yml
- filename: deepgram-models-api-openapi.yml
  format: yaml
  label: Deepgram Models API
  slug: deepgram-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-models-api-openapi.yml
- filename: deepgram-projects-api-openapi.yml
  format: yaml
  label: Deepgram Projects API
  slug: deepgram-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-projects-api-openapi.yml
- filename: deepgram-scopes-api-openapi.yml
  format: yaml
  label: Deepgram Scopes API
  slug: deepgram-scopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-scopes-api-openapi.yml
- filename: deepgram-usage-api-openapi.yml
  format: yaml
  label: Deepgram Usage API
  slug: deepgram-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-usage-api-openapi.yml
- filename: deepgram-audio-api-openapi.yml
  format: yaml
  label: Deepgram Audio API
  slug: deepgram-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-audio-api-openapi.yml
- filename: deepgram-breakdown-api-openapi.yml
  format: yaml
  label: Deepgram Breakdown API
  slug: deepgram-breakdown-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-breakdown-api-openapi.yml
- filename: deepgram-configurations-api-openapi.yml
  format: yaml
  label: Deepgram Configurations API
  slug: deepgram-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-configurations-api-openapi.yml
- filename: deepgram-distributioncredentials-api-openapi.yml
  format: yaml
  label: Deepgram Distribution Credentials API
  slug: deepgram-distributioncredentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-distributioncredentials-api-openapi.yml
- filename: deepgram-fields-api-openapi.yml
  format: yaml
  label: Deepgram Fields API
  slug: deepgram-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-fields-api-openapi.yml
- filename: deepgram-invites-api-openapi.yml
  format: yaml
  label: Deepgram Invites API
  slug: deepgram-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-invites-api-openapi.yml
- filename: deepgram-media-api-openapi.yml
  format: yaml
  label: Deepgram Media API
  slug: deepgram-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-media-api-openapi.yml
- filename: deepgram-purchases-api-openapi.yml
  format: yaml
  label: Deepgram Purchases API
  slug: deepgram-purchases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-purchases-api-openapi.yml
- filename: deepgram-requests-api-openapi.yml
  format: yaml
  label: Deepgram Requests API
  slug: deepgram-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-requests-api-openapi.yml
- filename: deepgram-text-api-openapi.yml
  format: yaml
  label: Deepgram Text API
  slug: deepgram-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-text-api-openapi.yml
- filename: deepgram-tokens-api-openapi.yml
  format: yaml
  label: Deepgram Tokens API
  slug: deepgram-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-tokens-api-openapi.yml
- filename: deepgram-variables-api-openapi.yml
  format: yaml
  label: Deepgram Variables API
  slug: deepgram-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepgram/openapi/deepgram-variables-api-openapi.yml
consequence_counts:
  physical: 1
  read: 13
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Deepgram Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/projects/{project_id}/invites
operation_count: 24
overview: 'Deepgram exposes 24 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 10 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Deepgram
provider_slug: deepgram
slug: deepgram-agentic-access
source_filename: deepgram-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/deepgram-management-openapi.yml, openapi/deepgram-speech-to-text-openapi.yml,\n  openapi/deepgram-text-to-speech-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 13\n    acting: 11\n  by_consequence:\n    read: 13\n    write: 10\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project_id}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project_id}\n  method: patch\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{project_id}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{project_id}/keys\n  method: get\n  operationId: listProjectKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project_id}/keys\n  method: post\n  operationId: createProjectKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{project_id}/keys/{key_id}\n  method: get\n  operationId: getProjectKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project_id}/keys/{key_id}\n  method: delete\n  operationId: deleteProjectKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /v1/projects/{project_id}/members\n  method: get\n  operationId: listProjectMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project_id}/members/{member_id}\n  method: delete\n  operationId: removeProjectMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{project_id}/invites\n  method: get\n  operationId: listProjectInvitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project_id}/invites\n  method: post\n  operationId: sendProjectInvitation\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{project_id}/invites/{email}\n  method: delete\n  operationId: deleteProjectInvitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{project_id}/members/{member_id}/scopes\n  method: get\n  operationId: getMemberScopes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project_id}/members/{member_id}/scopes\n\
  \  method: put\n  operationId: updateMemberScopes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{project_id}/usage\n  method: get\n  operationId: getProjectUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project_id}/requests\n  method: get\n  operationId: listProjectRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project_id}/balances\n  method: get\n  operationId: listProjectBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{project_id}/balances/{balance_id}\n  method: get\n  operationId: getProjectBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models/{model_id}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/listen\n  method: post\n  operationId: transcribePreRecordedAudio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/read\n  method: post\n  operationId: analyzeText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/speak\n  method: post\n  operationId: synthesizeSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/deepgram/agentic-access/deepgram-agentic-access.yml
summary_line: 24 operations · 11 acting
tags:
- Artificial Intelligence
- Speech-to-Text
- Text-to-Speech
- Transcription
- Voice AI
- Voice
- Real-Time
---
