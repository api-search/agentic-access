---
acting_count: 48
action_class_counts:
  acting: 48
  connected: 38
api_specs:
- filename: vapi-assistants-api-openapi.yml
  format: yaml
  label: Vapi Assistants API
  slug: vapi-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-assistants-api-openapi.yml
- filename: vapi-calls-api-openapi.yml
  format: yaml
  label: Vapi Calls API
  slug: vapi-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-calls-api-openapi.yml
- filename: vapi-phone-numbers-api-openapi.yml
  format: yaml
  label: Vapi Phone Numbers API
  slug: vapi-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-phone-numbers-api-openapi.yml
- filename: vapi-squads-api-openapi.yml
  format: yaml
  label: Vapi Squads API
  slug: vapi-squads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-squads-api-openapi.yml
- filename: vapi-tools-api-openapi.yml
  format: yaml
  label: Vapi Tools API
  slug: vapi-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-tools-api-openapi.yml
- filename: vapi-files-api-openapi.yml
  format: yaml
  label: Vapi Files API
  slug: vapi-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-files-api-openapi.yml
- filename: vapi-chats-api-openapi.yml
  format: yaml
  label: Vapi Chats API
  slug: vapi-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-chats-api-openapi.yml
- filename: vapi-sessions-api-openapi.yml
  format: yaml
  label: Vapi Sessions API
  slug: vapi-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-sessions-api-openapi.yml
- filename: vapi-campaigns-api-openapi.yml
  format: yaml
  label: Vapi Campaigns API
  slug: vapi-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-campaigns-api-openapi.yml
- filename: vapi-analytics-api-openapi.yml
  format: yaml
  label: Vapi Analytics API
  slug: vapi-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-analytics-api-openapi.yml
- filename: vapi-insight-api-openapi.yml
  format: yaml
  label: Vapi Insight API
  slug: vapi-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-insight-api-openapi.yml
- filename: vapi-observability-api-openapi.yml
  format: yaml
  label: Vapi Observability Scorecard API
  slug: vapi-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-observability-api-openapi.yml
- filename: vapi-eval-api-openapi.yml
  format: yaml
  label: Vapi Eval API
  slug: vapi-eval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-eval-api-openapi.yml
- filename: vapi-structured-outputs-api-openapi.yml
  format: yaml
  label: Vapi Structured Outputs API
  slug: vapi-structured-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-structured-outputs-api-openapi.yml
- filename: vapi-provider-resources-api-openapi.yml
  format: yaml
  label: Vapi Provider Resources API
  slug: vapi-provider-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-provider-resources-api-openapi.yml
consequence_counts:
  read: 38
  safety-critical: 48
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 48
kind: agentic-access
layout: agentic-access
method: generated
name: Vapi Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /analytics
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /assistant
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /assistant/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /assistant/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /call
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /call/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /call/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /campaign
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /campaign/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /campaign/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /chat
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /chat/responses
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /chat/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /eval
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /eval/run
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /eval/run/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /eval/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /eval/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /file
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /file/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /file/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /observability/scorecard
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /observability/scorecard/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /observability/scorecard/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /phone-number
operation_count: 86
overview: 'Vapi exposes 86 API operations that an AI agent could call, of which 48 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read and 48 safety-critical.


  48 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vapi
provider_slug: vapi-ai
slug: vapi-ai-agentic-access
source_filename: vapi-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vapi-analytics-api-openapi.yml, openapi/vapi-assistants-api-openapi.yml, openapi/vapi-calls-api-openapi.yml,\n  openapi/vapi-campaigns-api-openapi.yml, openapi/vapi-chats-api-openapi.yml, openapi/vapi-eval-api-openapi.yml,\n  openapi/vapi-files-api-openapi.yml, openapi/vapi-insight-api-openapi.yml, openapi/vapi-observability-api-openapi.yml,\n  openapi/vapi-phone-numbers-api-openapi.yml, openapi/vapi-provider-resources-api-openapi.yml,\n  openapi/vapi-sessions-api-openapi.yml, openapi/vapi-squads-api-openapi.yml, openapi/vapi-structured-outputs-api-openapi.yml,\n  openapi/vapi-tools-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 86\n  by_action_class:\n    acting: 48\n\
  \    connected: 38\n  by_consequence:\n    safety-critical: 48\n    read: 38\n  human_in_the_loop_required: 48\noperations:\n- path: /analytics\n  method: post\n  operationId: AnalyticsController_query\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /assistant\n  method: post\n  operationId: AssistantController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /assistant\n  method: get\n  operationId: AssistantController_findAll\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assistant/{id}\n  method: get\n  operationId: AssistantController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assistant/{id}\n  method: patch\n  operationId: AssistantController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /assistant/{id}\n  method: delete\n  operationId: AssistantController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n  \
  \    exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /call\n  method: post\n  operationId: CallController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /call\n  method: get\n  operationId: CallController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /call/{id}\n  method: get\n  operationId: CallController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /call/{id}\n  method:\
  \ patch\n  operationId: CallController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /call/{id}\n  method: delete\n  operationId: CallController_deleteCallData\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /call/{id}/mono-recording\n  method: get\n  operationId: CallArtifactController_monoRecordingDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /call/{id}/stereo-recording\n  method: get\n  operationId: CallArtifactController_stereoRecordingDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /call/{id}/video-recording\n  method: get\n  operationId: CallArtifactController_videoRecordingDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /call/{id}/customer-recording\n  method: get\n  operationId: CallArtifactController_customerRecordingDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /call/{id}/assistant-recording\n  method: get\n  operationId: CallArtifactController_assistantRecordingDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /call/{id}/pcap\n  method: get\n  operationId: CallArtifactController_pcapDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /call/{id}/call-logs\n  method: get\n  operationId: CallArtifactController_callLogsDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaign\n  method: post\n  operationId: CampaignController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /campaign\n  method: get\n  operationId: CampaignController_findAll\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaign/{id}\n  method: get\n  operationId: CampaignController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaign/{id}\n  method: patch\n  operationId: CampaignController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /campaign/{id}\n  method: delete\n  operationId: CampaignController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /chat\n  method: get\n  operationId: ChatController_listChats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat\n  method: post\n  operationId: ChatController_createChat\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /chat/{id}\n  method: get\n  operationId: ChatController_getChat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/{id}\n\
  \  method: delete\n  operationId: ChatController_deleteChat\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /chat/responses\n  method: post\n  operationId: ChatController_createOpenAIChat\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /eval\n  method: post\n  operationId: EvalController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /eval\n  method: get\n  operationId: EvalController_getPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eval/{id}\n  method: patch\n  operationId: EvalController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /eval/{id}\n  method: delete\n  operationId: EvalController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /eval/{id}\n  method: get\n  operationId: EvalController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eval/run/{id}\n  method: delete\n  operationId: EvalController_removeRun\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /eval/run/{id}\n  method: get\n  operationId: EvalController_getRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /eval/run\n  method: post\n  operationId: EvalController_run\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /eval/run\n  method: get\n  operationId: EvalController_getRunsPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file\n  method: post\n  operationId: FileController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /file\n\
  \  method: get\n  operationId: FileController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file/{id}\n  method: get\n  operationId: FileController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file/{id}\n  method: patch\n  operationId: FileController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /file/{id}\n  method: delete\n  operationId: FileController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reporting/insight\n  method: post\n  operationId: InsightController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reporting/insight\n  method: get\n  operationId: InsightController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/insight/{id}\n  method: patch\n  operationId: InsightController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reporting/insight/{id}\n  method: get\n  operationId: InsightController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/insight/{id}\n  method: delete\n  operationId: InsightController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reporting/insight/{id}/run\n  method: post\n  operationId: InsightController_run\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reporting/insight/preview\n  method: post\n  operationId: InsightController_preview\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /observability/scorecard/{id}\n  method: get\n  operationId: ScorecardController_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /observability/scorecard/{id}\n  method: patch\n  operationId: ScorecardController_update\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /observability/scorecard/{id}\n  method: delete\n  operationId: ScorecardController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /observability/scorecard\n  method: get\n  operationId: ScorecardController_getPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /observability/scorecard\n\
  \  method: post\n  operationId: ScorecardController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /phone-number\n  method: post\n  operationId: PhoneNumberController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /phone-number\n  method: get\n  operationId: PhoneNumberController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v2/phone-number\n  method: get\n  operationId: PhoneNumberController_findAllPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phone-number/{id}\n  method: get\n  operationId: PhoneNumberController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phone-number/{id}\n  method: patch\n  operationId: PhoneNumberController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /phone-number/{id}\n  method: delete\n  operationId: PhoneNumberController_remove\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /provider/{provider}/{resourceName}\n  method: post\n  operationId: ProviderResourceController_createProviderResource\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /provider/{provider}/{resourceName}\n  method: get\n  operationId: ProviderResourceController_getProviderResourcesPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /provider/{provider}/{resourceName}/{id}\n  method: get\n  operationId: ProviderResourceController_getProviderResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/{provider}/{resourceName}/{id}\n  method: delete\n  operationId: ProviderResourceController_deleteProviderResource\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /provider/{provider}/{resourceName}/{id}\n  method: patch\n  operationId: ProviderResourceController_updateProviderResource\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /session\n  method: post\n  operationId: SessionController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /session\n  method: get\n  operationId: SessionController_findAllPaginated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /session/{id}\n  method: get\n  operationId: SessionController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /session/{id}\n  method: patch\n  operationId: SessionController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /session/{id}\n  method: delete\n  operationId: SessionController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /squad\n  method: post\n  operationId: SquadController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /squad\n  method: get\n  operationId: SquadController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /squad/{id}\n  method: get\n  operationId: SquadController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /squad/{id}\n  method: patch\n  operationId: SquadController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /squad/{id}\n  method: delete\n  operationId: SquadController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /structured-output\n  method: get\n  operationId: StructuredOutputController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /structured-output\n  method: post\n  operationId: StructuredOutputController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /structured-output/{id}\n  method: get\n  operationId: StructuredOutputController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /structured-output/{id}\n  method: patch\n  operationId: StructuredOutputController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /structured-output/{id}\n  method: delete\n  operationId: StructuredOutputController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /structured-output/run\n  method: post\n  operationId: StructuredOutputController_run\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tool\n  method: post\n  operationId: ToolController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tool\n  method: get\n  operationId: ToolController_findAll\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tool/{id}\n  method: get\n  operationId: ToolController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tool/{id}\n  method: patch\n  operationId: ToolController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /tool/{id}\n  method: delete\n  operationId: ToolController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/agentic-access/vapi-ai-agentic-access.yml
summary_line: 86 operations · 48 acting · 48 human-in-the-loop
tags:
- AI
- Voice AI
- Voice Agents
- Conversational AI
- Telephony
- Real-Time
- Transcription
- Text-to-Speech
- LLM
- Agents
- MCP
---
