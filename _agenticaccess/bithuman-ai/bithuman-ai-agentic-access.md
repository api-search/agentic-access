---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 23
api_specs:
- filename: bithuman-ai-account-api-openapi.yml
  format: yaml
  label: bithuman-ai Account API
  slug: bithuman-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-account-api-openapi.yml
- filename: bithuman-ai-agent-context-api-openapi.yml
  format: yaml
  label: bithuman-ai Agent Context API
  slug: bithuman-ai-agent-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-agent-context-api-openapi.yml
- filename: bithuman-ai-agent-generation-api-openapi.yml
  format: yaml
  label: bithuman-ai Agent Generation API
  slug: bithuman-ai-agent-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-agent-generation-api-openapi.yml
- filename: bithuman-ai-agent-management-api-openapi.yml
  format: yaml
  label: bithuman-ai Agent Management API
  slug: bithuman-ai-agent-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-agent-management-api-openapi.yml
- filename: bithuman-ai-api-secrets-api-openapi.yml
  format: yaml
  label: bithuman-ai API secrets API
  slug: bithuman-ai-api-secrets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-api-secrets-api-openapi.yml
- filename: bithuman-ai-authentication-api-openapi.yml
  format: yaml
  label: bithuman-ai Authentication API
  slug: bithuman-ai-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-authentication-api-openapi.yml
- filename: bithuman-ai-billing-api-openapi.yml
  format: yaml
  label: bithuman-ai Billing API
  slug: bithuman-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-billing-api-openapi.yml
- filename: bithuman-ai-dynamics-api-openapi.yml
  format: yaml
  label: bithuman-ai Dynamics API
  slug: bithuman-ai-dynamics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-dynamics-api-openapi.yml
- filename: bithuman-ai-embedding-api-openapi.yml
  format: yaml
  label: bithuman-ai Embedding API
  slug: bithuman-ai-embedding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-embedding-api-openapi.yml
- filename: bithuman-ai-files-api-openapi.yml
  format: yaml
  label: bithuman-ai Files API
  slug: bithuman-ai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-files-api-openapi.yml
- filename: bithuman-ai-knowledge-api-openapi.yml
  format: yaml
  label: bithuman-ai Knowledge API
  slug: bithuman-ai-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-knowledge-api-openapi.yml
- filename: bithuman-ai-providers-api-openapi.yml
  format: yaml
  label: bithuman-ai Providers API
  slug: bithuman-ai-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-providers-api-openapi.yml
- filename: bithuman-ai-realtime-api-openapi.yml
  format: yaml
  label: bithuman-ai Realtime API
  slug: bithuman-ai-realtime-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-realtime-api-openapi.yml
- filename: bithuman-ai-runtime-sessions-api-openapi.yml
  format: yaml
  label: bithuman-ai Runtime sessions API
  slug: bithuman-ai-runtime-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-runtime-sessions-api-openapi.yml
- filename: bithuman-ai-self-hosting-api-openapi.yml
  format: yaml
  label: bithuman-ai Self Hosting API
  slug: bithuman-ai-self-hosting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-self-hosting-api-openapi.yml
- filename: bithuman-ai-status-api-openapi.yml
  format: yaml
  label: bithuman-ai Status API
  slug: bithuman-ai-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-status-api-openapi.yml
- filename: bithuman-ai-video-api-openapi.yml
  format: yaml
  label: bithuman-ai Video API
  slug: bithuman-ai-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-video-api-openapi.yml
- filename: bithuman-ai-webhooks-api-openapi.yml
  format: yaml
  label: bithuman-ai Webhooks API
  slug: bithuman-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bithuman-ai/openapi/bithuman-ai-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 23
  safety-critical: 2
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Bithuman Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/{user_id}/runtime-sessions/{session_id}/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/{user_id}/runtime/revoke-all
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{webhook_id}/test
operation_count: 52
overview: 'bithuman-ai exposes 52 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read, 26 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: bithuman-ai
provider_slug: bithuman-ai
slug: bithuman-ai-agentic-access
source_filename: bithuman-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/bithuman-ai-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    acting: 29\n    connected: 23\n  by_consequence:\n    write: 26\n    read: 23\n    physical: 1\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/validate\n  method: post\n  operationId: validateApiSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/generate\n  method: post\n  operationId: generateAgent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/status/{agent_id}\n  method: get\n  operationId: getAgentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/{code}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/{code}\n  method: post\n  operationId: updateAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/{code}\n  method: delete\n  operationId: deleteAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/{code}/speak\n  method: post\n  operationId: agentSpeak\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/{code}/sessions\n  method: get\n  operationId: listAgentSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/{code}/add-context\n\
  \  method: post\n  operationId: addContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/{code}/models\n  method: post\n  operationId: addAgentModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/{code}/model/download\n  method: get\n  operationId: downloadAgentModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/upload\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/models/showcase\n  method: get\n  operationId: getShowcaseManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/credit-summaries\n  method: get\n  operationId: getCreditSummaries\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/embed-tokens/request\n  method: post\n  operationId: requestEmbedToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/runtime-tokens/mint\n  method: post\n  operationId: mintScopedRuntimeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/runtime-tokens/request\n  method: post\n  operationId: requestRuntimeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/dynamics/generate\n  method: post\n  operationId: generateDynamics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/dynamics/{agent_id}\n  method: get\n  operationId: getDynamics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dynamics/{agent_id}\n  method: put\n  operationId: updateDynamics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/video/generate\n  method: post\n  operationId: generateTalkingVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/video/{job_id}\n  method: get\n  operationId: getTalkingVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{webhook_id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{webhook_id}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{webhook_id}/deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/validate\n  method: post\n  operationId: validateSelfHostedKey\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/meter/beats\n  method: post\n  operationId: postMeterBeat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{user_id}/api-secrets\n  method: post\n  operationId: createApiSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{user_id}/api-secrets\n\
  \  method: get\n  operationId: listApiSecrets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{user_id}/api-secrets/{alias}/get-value\n  method: get\n  operationId: revealApiSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{user_id}/api-secrets/{alias}\n  method: delete\n  operationId: deleteApiSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{user_id}/providers\n  method: get\n  operationId: getProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /v2/{user_id}/providers\n  method: put\n  operationId: updateProviders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{user_id}/runtime-sessions\n  method: get\n  operationId: listRuntimeSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{user_id}/runtime-sessions/{session_id}/messages\n  method: get\n  operationId: getRuntimeSessionMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{user_id}/runtime-sessions/{session_id}/terminate\n  method: post\n  operationId: terminateRuntimeSession\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/{user_id}/runtime/revoke-all\n  method: post\n  operationId: revokeAllRuntimeKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/runtime-sessions/{session_id}\n  method: get\n  operationId: getCloudAvatarSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/runtime-sessions/{session_id}/end\n\
  \  method: post\n  operationId: endCloudAvatarSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/knowledge/files\n  method: post\n  operationId: ingestKnowledgeFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/knowledge/kbs\n  method: post\n  operationId: createKnowledgeBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/knowledge/kbs\n  method: get\n  operationId: listKnowledgeBases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/knowledge/kbs/{kb_id}/rebuild\n  method: post\n  operationId: rebuildKnowledgeBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/realtime/connect\n  method: post\n  operationId: realtimeConnect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /readyz\n  method: get\n  operationId: getReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bithuman-ai/agentic-access/bithuman-ai-agentic-access.yml
summary_line: 52 operations · 29 acting · 2 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Avatars
- Real-Time
- Platform
---
