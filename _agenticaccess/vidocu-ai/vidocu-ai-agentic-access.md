---
acting_count: 196
action_class_counts:
  acting: 196
  connected: 124
api_specs:
- filename: vidocu-ai-ai-recorder-api-openapi.yml
  format: yaml
  label: vidocu-ai AI Recorder API
  slug: vidocu-ai-ai-recorder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-ai-recorder-api-openapi.yml
- filename: vidocu-ai-brand-kit-api-openapi.yml
  format: yaml
  label: vidocu-ai Brand Kit API
  slug: vidocu-ai-brand-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-brand-kit-api-openapi.yml
- filename: vidocu-ai-courses-api-openapi.yml
  format: yaml
  label: vidocu-ai Courses API
  slug: vidocu-ai-courses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-courses-api-openapi.yml
- filename: vidocu-ai-governance-api-openapi.yml
  format: yaml
  label: vidocu-ai Governance API
  slug: vidocu-ai-governance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-governance-api-openapi.yml
- filename: vidocu-ai-jobs-api-openapi.yml
  format: yaml
  label: vidocu-ai Jobs API
  slug: vidocu-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-jobs-api-openapi.yml
- filename: vidocu-ai-knowledge-center-api-openapi.yml
  format: yaml
  label: vidocu-ai Knowledge Center API
  slug: vidocu-ai-knowledge-center-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-knowledge-center-api-openapi.yml
- filename: vidocu-ai-operations-api-openapi.yml
  format: yaml
  label: vidocu-ai Operations API
  slug: vidocu-ai-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-operations-api-openapi.yml
- filename: vidocu-ai-projects-api-openapi.yml
  format: yaml
  label: vidocu-ai Projects API
  slug: vidocu-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-projects-api-openapi.yml
- filename: vidocu-ai-reference-api-openapi.yml
  format: yaml
  label: vidocu-ai Reference API
  slug: vidocu-ai-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-reference-api-openapi.yml
- filename: vidocu-ai-remix-api-openapi.yml
  format: yaml
  label: vidocu-ai Remix API
  slug: vidocu-ai-remix-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-remix-api-openapi.yml
- filename: vidocu-ai-studio-api-openapi.yml
  format: yaml
  label: vidocu-ai Studio API
  slug: vidocu-ai-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-studio-api-openapi.yml
- filename: vidocu-ai-tools-api-openapi.yml
  format: yaml
  label: vidocu-ai Tools API
  slug: vidocu-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-tools-api-openapi.yml
- filename: vidocu-ai-training-modules-api-openapi.yml
  format: yaml
  label: vidocu-ai Training Modules API
  slug: vidocu-ai-training-modules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-training-modules-api-openapi.yml
- filename: vidocu-ai-usage-api-openapi.yml
  format: yaml
  label: vidocu-ai Usage API
  slug: vidocu-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-usage-api-openapi.yml
- filename: vidocu-ai-videos-api-openapi.yml
  format: yaml
  label: vidocu-ai Videos API
  slug: vidocu-ai-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-videos-api-openapi.yml
- filename: vidocu-ai-webhooks-api-openapi.yml
  format: yaml
  label: vidocu-ai Webhooks API
  slug: vidocu-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidocu-ai/openapi/vidocu-ai-webhooks-api-openapi.yml
consequence_counts:
  physical: 22
  read: 124
  safety-critical: 6
  write: 168
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Vidocu Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/brand-kit/skills
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/brand-kit/skills
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/brand-kit/skills/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/brand-kit/skills/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/brand-kit/skills/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/brand-kit/skills/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/approvals/{id}/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/approvals/{id}/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/knowledge-base/articles/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/knowledge-base/articles/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/knowledge-base/sections/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/knowledge-base/sections/reorder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/modules/planner/qualification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/modules/planner/qualification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/recorder-sessions/{session}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/recorder-sessions/{session}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/recorder-sessions/{session}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/recorder-sessions/{session}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/recordings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/recordings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/recordings/{jobId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/recordings/{jobId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/recordings/{jobId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/recordings/{jobId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/recordings/{jobId}/input
operation_count: 320
overview: 'vidocu-ai exposes 320 API operations that an AI agent could call, of which 196 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 124 read, 168 write, 22 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: vidocu-ai
provider_slug: vidocu-ai
slug: vidocu-ai-agentic-access
source_filename: vidocu-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/support-vidocu-openapi.json, openapi/vidocu-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 320\n  by_action_class:\n    acting: 196\n    connected: 124\n  by_consequence:\n    write: 168\n    read: 124\n    physical: 22\n    safety-critical: 6\n  human_in_the_loop_required: 6\noperations:\n- path: /v1/videos/upload\n  method: post\n  operationId: postV1VideosUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/from-document\n\
  \  method: post\n  operationId: postV1VideosFrom-document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos\n  method: get\n  operationId: getV1Videos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/{id}\n  method: get\n  operationId: getV1VideosId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/{id}\n  method: patch\n  operationId: patchV1VideosId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}\n  method: delete\n  operationId: deleteV1VideosId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/analyze\n  method: post\n  operationId: postV1VideosIdAnalyze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/export\n  method: post\n  operationId: postV1VideosIdExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/translate\n  method: post\n  operationId: postV1VideosIdTranslate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/subtitles\n  method: get\n  operationId: getV1VideosIdSubtitles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/{id}/voiceover\n  method: post\n  operationId: postV1VideosIdVoiceover\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/article\n  method: post\n  operationId: postV1VideosIdArticle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/article\n  method: get\n  operationId: getV1VideosIdArticle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/process\n  method: post\n  operationId: postV1VideosProcess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/script\n  method: get\n  operationId: getV1VideosIdScript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/videos/{id}/script\n  method: put\n  operationId: putV1VideosIdScript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/download\n  method: get\n  operationId: getV1VideosIdDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: get\n  operationId: getV1Webhooks\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: postV1Webhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}\n  method: patch\n  operationId: patchV1WebhooksId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}\n  method: delete\n  operationId: deleteV1WebhooksId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects\n  method: post\n  operationId: postV1Projects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects\n  method: get\n  operationId: getV1Projects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{id}\n  method: get\n  operationId: getV1ProjectsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{id}\n\
  \  method: patch\n  operationId: patchV1ProjectsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{id}\n  method: delete\n  operationId: deleteV1ProjectsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools\n  method: get\n  operationId: getV1Tools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/{type}\n  method: get\n  operationId: getV1ToolsType\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/{type}/execute\n  method: post\n  operationId: postV1ToolsTypeExecute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/lock\n  method: post\n  operationId: postV1VideosIdLock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/lock\n  method: delete\n  operationId: deleteV1VideosIdLock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/approvals\n  method: post\n  operationId: postV1VideosIdApprovals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/approvals\n  method: get\n  operationId: getV1VideosIdApprovals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/approvals\n  method: get\n  operationId: getV1Approvals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /v1/approvals/{id}/decide\n  method: post\n  operationId: postV1ApprovalsIdDecide\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/approvals/{id}/withdraw\n  method: post\n  operationId: postV1ApprovalsIdWithdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/comments\n  method: get\n  operationId: getV1VideosIdComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/videos/{id}/comments\n  method: post\n  operationId: postV1VideosIdComments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/videos/{id}/comments/{commentId}\n  method: delete\n  operationId: deleteV1VideosIdCommentsCommentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/brand-kit/assets\n  method: get\n  operationId: getV1Brand-kitAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/brand-kit/assets\n  method: post\n  operationId: postV1Brand-kitAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/brand-kit/assets/{id}\n  method: delete\n  operationId: deleteV1Brand-kitAssetsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/studio/templates\n  method: get\n  operationId: getV1StudioTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/studio/templates/{id}/use\n\
  \  method: post\n  operationId: postV1StudioTemplatesIdUse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/studio/projects\n  method: get\n  operationId: getV1StudioProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/studio/projects\n  method: post\n  operationId: postV1StudioProjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/studio/projects/{id}\n  method: get\n  operationId: getV1StudioProjectsId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/studio/projects/{id}\n  method: patch\n  operationId: patchV1StudioProjectsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/studio/projects/{id}\n  method: delete\n  operationId: deleteV1StudioProjectsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/studio/projects/{id}/timeline\n  method: put\n  operationId: putV1StudioProjectsIdTimeline\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/studio/projects/{id}/duplicate\n  method: post\n  operationId: postV1StudioProjectsIdDuplicate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/studio/projects/{id}/export\n  method: post\n  operationId: postV1StudioProjectsIdExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/studio/projects/{id}/share\n  method: post\n  operationId: postV1StudioProjectsIdShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-media\n  method: get\n  operationId: getV1Ai-media\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai-media/shot\n  method: post\n  operationId: postV1Ai-mediaShot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-media/stills\n  method:\
  \ post\n  operationId: postV1Ai-mediaStills\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-media/clips\n  method: post\n  operationId: postV1Ai-mediaClips\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-media/scenes\n  method: post\n  operationId: postV1Ai-mediaScenes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /v1/ai-media/scenes/translate\n  method: post\n  operationId: postV1Ai-mediaScenesTranslate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai-media/{id}\n  method: get\n  operationId: getV1Ai-mediaId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/modules\n  method: get\n  operationId: getV1Modules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/modules/generate\n  method: post\n  operationId: postV1ModulesGenerate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/modules/{id}\n  method: get\n  operationId: getV1ModulesId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/modules/{id}\n  method: patch\n  operationId: patchV1ModulesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/modules/{id}\n  method: delete\n  operationId: deleteV1ModulesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/modules/{id}/lock\n  method: post\n  operationId: postV1ModulesIdLock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/modules/{id}/translate\n  method: post\n  operationId: postV1ModulesIdTranslate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/modules/{id}/translations\n  method: get\n  operationId: getV1ModulesIdTranslations\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/modules/{id}/submit\n  method: post\n  operationId: postV1ModulesIdSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/modules/{id}/results\n  method: get\n  operationId: getV1ModulesIdResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/modules/{id}/passers\n  method: get\n  operationId: getV1ModulesIdPassers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/modules/{id}/qualifications\n  method: get\n  operationId: getV1ModulesIdQualifications\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/modules/{id}/qualifications\n  method: post\n  operationId: postV1ModulesIdQualifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/modules/analytics\n  method: get\n  operationId: getV1ModulesAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/modules/analytics/by-person\n  method: get\n  operationId: getV1ModulesAnalyticsBy-person\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/modules/analytics/signoffs\n  method: get\n  operationId: getV1ModulesAnalyticsSignoffs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/modules/planner\n  method: get\n  operationId: getV1ModulesPlanner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/modules/planner/deadline\n  method: put\n  operationId: putV1ModulesPlannerDeadline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/modules/planner/qualification\n  method: post\n  operationId: postV1ModulesPlannerQualification\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/modules/people\n  method: get\n  operationId: getV1ModulesPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/modules/people\n  method: post\n  operationId: postV1ModulesPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/remixes\n  method: get\n  operationId: getV1Remixes\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/remixes\n  method: post\n  operationId: postV1Remixes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/remixes/{id}\n  method: get\n  operationId: getV1RemixesId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/remixes/{id}\n  method: patch\n  operationId: patchV1RemixesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/remixes/{id}\n  method: delete\n  operationId: deleteV1RemixesId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/remixes/{id}/analyze\n  method: post\n  operationId: postV1RemixesIdAnalyze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/remixes/{id}/export\n  method: post\n  operationId: postV1RemixesIdExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/remixes/{id}/regenerate\n  method: post\n  operationId: postV1RemixesIdRegenerate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/remixes/{id}/moments\n  method: post\n  operationId: postV1RemixesIdMoments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/remixes/{id}/moments/{momentId}\n  method: patch\n  operationId: patchV1RemixesIdMomentsMomentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/remixes/{id}/recap\n  method: put\n  operationId: putV1RemixesIdRecap\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/remixes/{id}/exports\n  method: get\n  operationId: getV1RemixesIdExports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recordings\n  method: get\n  operationId: getV1Recordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recordings\n  method: post\n  operationId: postV1Recordings\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recordings/{jobId}\n  method: get\n  operationId: getV1RecordingsJobId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recordings/{jobId}\n  method: patch\n  operationId: patchV1RecordingsJobId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recordings/{jobId}\n  method: delete\n  operationId: deleteV1RecordingsJobId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recordings/{jobId}/download\n  method: get\n  operationId: getV1RecordingsJobIdDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recordings/{jobId}/input\n  method: post\n  operationId: postV1RecordingsJobIdInput\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recorder-sessions\n  method: get\n  operationId: getV1Recorder-sessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recorder-sessions/{session}\n  method: patch\n  operationId: patchV1Recorder-sessionsSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recorder-sessions/{session}\n  method: delete\n  operationId: deleteV1Recorder-sessionsSession\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/knowledge-base\n  method: get\n  operationId: getV1Knowledge-base\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/knowledge-base\n  method: post\n  operationId: postV1Knowledge-base\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (95 KB total) ---\n# Full source: https://artifacts.apis.io/vidocu-ai/agentic-access/vidocu-ai-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/vidocu-ai/agentic-access/vidocu-ai-agentic-access.yml
summary_line: 320 operations · 196 acting · 6 human-in-the-loop
tags:
- Artificial Intelligence
- Video
- Documentation
- SOP
- Training
- Knowledge Base
---
