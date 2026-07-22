---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 9
api_specs:
- filename: opusclip-openapi-original.json
  format: json
  label: OpusClip Clip API
  slug: opusclip-clip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/openapi/opusclip-openapi-original.json
consequence_counts:
  read: 9
  safety-critical: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 13
kind: agentic-access
layout: agentic-access
method: generated
name: Opusclip Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/censor-jobs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/clip-projects
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/clip-projects/{projectId}/update-visibility
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/collection-contents
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/collection-contents/delete-collection-contents
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/collections
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/collections/{collectionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/collections/{collectionId}/export
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/generative-jobs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/post-tasks
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/publish-schedules
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/publish-schedules/{scheduleId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/social-copy-jobs
operation_count: 22
overview: 'OpusClip exposes 22 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 13 safety-critical.


  13 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpusClip
provider_slug: opusclip
slug: opusclip-agentic-access
source_filename: opusclip-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/opusclip-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 9\n    acting: 13\n  by_consequence:\n    read: 9\n    safety-critical: 13\n  human_in_the_loop_required: 13\noperations:\n- path: /api/brand-templates\n  method: get\n  operationId: BrandTemplateController_getTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/clip-projects\n  method: post\n  operationId: ClipProjectController_createClipProject\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/clip-projects/{projectId}\n  method: get\n  operationId: ClipProjectController_getClipProjectDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/clip-projects/{projectId}/update-visibility\n  method: post\n  operationId: ClipProjectController_updateClipProjectVisibility\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/exportable-clips\n  method: get\n  operationId: ExportableClipController_queryExportableClips\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/collection-contents/delete-collection-contents\n  method: post\n  operationId: CollectionContentController_deleteCollectionContents\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/collection-contents\n  method: post\n  operationId: CollectionContentController_createCollectionContent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/collections/{collectionId}\n  method: delete\n  operationId: CollectionController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/collections\n  method: post\n  operationId: CollectionController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/collections\n  method: get\n  operationId: CollectionController_list\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/collections/{collectionId}/export\n  method: post\n  operationId: CollectionController_export\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/censor-jobs\n  method: post\n  operationId: CensorJobController_createCensorJob\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/censor-jobs/{jobId}\n  method: get\n  operationId: CensorJobController_getCensorJob\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/social-accounts\n  method: get\n  operationId: SocialAccountController_getSocialAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/social-copy-jobs\n  method: post\n  operationId: SocialCopyJobController_createSocialCopyJob\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/social-copy-jobs/{jobId}\n  method: get\n  operationId: SocialCopyJobController_getSocialCopyJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/post-tasks\n  method: post\n  operationId: PostTaskController_createPostTask\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/publish-schedules\n  method: post\n  operationId: PublishScheduleController_createPublishSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/publish-schedules/{scheduleId}\n  method: delete\n  operationId: PublishScheduleController_cancelPublishSchedule\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/generative-jobs\n  method: post\n  operationId: GenerativeJobController_createGenerativeJob\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/generative-jobs/{jobId}\n  method: get\n  operationId: GenerativeJobController_getGenerativeJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/transcripts\n\
  \  method: get\n  operationId: TranscriptController_getTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opusclip/refs/heads/main/agentic-access/opusclip-agentic-access.yml
summary_line: 22 operations · 13 acting · 13 human-in-the-loop
tags:
- Company
- Consumer
- Video
- AI
- Video Editing
- Short-Form Video
- Social Media
- Content Creation
- MCP
- Developer API
---
