---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 10
api_specs:
- filename: vyond-content-generation-api-openapi.yml
  format: yaml
  label: Vyond Content Generation API
  slug: vyond-content-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-content-generation-api-openapi.yml
- filename: vyond-parameter-api-openapi.yml
  format: yaml
  label: Vyond Parameter API
  slug: vyond-parameter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-parameter-api-openapi.yml
- filename: vyond-scim-api-openapi.yml
  format: yaml
  label: Vyond SCIM API
  slug: vyond-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-scim-api-openapi.yml
- filename: vyond-turbo-api-openapi.yml
  format: yaml
  label: Vyond Turbo API
  slug: vyond-turbo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-turbo-api-openapi.yml
- filename: vyond-user-api-openapi.yml
  format: yaml
  label: Vyond User API
  slug: vyond-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-user-api-openapi.yml
- filename: vyond-video-api-openapi.yml
  format: yaml
  label: Vyond Video API
  slug: vyond-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-video-api-openapi.yml
- filename: vyond-video-export-api-openapi.yml
  format: yaml
  label: Vyond Video Export API
  slug: vyond-video-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-video-export-api-openapi.yml
- filename: vyond-webhook-api-openapi.yml
  format: yaml
  label: Vyond Webhook API
  slug: vyond-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-webhook-api-openapi.yml
consequence_counts:
  physical: 4
  read: 10
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: derived
name: Vyond Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rest/v1/generations/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rest/v1/turbo/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rest/v1/videos/{videoId}/exports
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rest/v2/generations/
operation_count: 20
overview: 'Vyond exposes 20 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 6 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vyond
provider_slug: vyond
slug: vyond-agentic-access
source_filename: vyond-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: openapi/vyond-openapi-original.json (heuristic corrected by hand — see x-correction)\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI.\n  A governance starting point for exposing this API to AI agents — review and bind audience per deployment.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 10\n    connected: 10\n  by_consequence:\n    physical: 4\n    read: 10\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /rest/v1/generations/\n  method: post\n  operationId: ContentGenerationController.createGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    audit: required\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    subject: required\n- path: /rest/v2/generations/\n  method: post\n  operationId: ContentGenerationV2Controller.createGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    audit: required\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    subject: required\n- path: /rest/v2/generations/{id}\n  method: get\n  operationId: ContentGenerationV2Controller.getGeneration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Users\n  method: get\n  operationId: ScimController.getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Users\n  method:\
  \ post\n  operationId: ScimController.createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    audience: null\n    token:\n      max-ttl: 900\n    audit: required\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    subject: required\n- path: /scim/v2/Users/{userId}\n  method: get\n  operationId: ScimController.getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Users/{userId}\n  method: put\n  operationId: ScimController.updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    audience: null\n    token:\n      max-ttl: 900\n    audit: required\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    subject: required\n- path: /scim/v2/Users/{userId}\n  method: patch\n  operationId: ScimController.patchUser\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    audience: null\n    token:\n      max-ttl: 900\n    audit: required\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    subject: required\n- path: /scim/v2/Schemas\n  method: get\n  operationId: ScimController.getSchemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Schemas/{id}\n  method: get\n  operationId: ScimController.getSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/parameters/\n  method: get\n  operationId: ParameterController.getParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/turbo/\n\
  \  method: post\n  operationId: TurboController.createTurbo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    audit: required\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    subject: required\n- path: /rest/v1/turbo/{id}\n  method: get\n  operationId: TurboController.getTurbo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/users/me\n  method: get\n  operationId: UserController.getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/videos/{videoId}/exports\n  method: post\n  operationId: VideoController.exportVideo\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    audit: required\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    subject: required\n- path: /rest/v1/videos/{videoId}/exports/{conversionId}\n  method: get\n  operationId: VideoController.getVideoExportDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/webhooks/\n  method: get\n  operationId: WebhookController.getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/webhooks/\n  method: post\n  operationId: WebhookController.createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    audit: required\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    subject: required\n- path: /rest/v1/webhooks/{webhookId}\n  method: patch\n  operationId: WebhookController.updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    audience: null\n    token:\n      max-ttl: 900\n    audit: required\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    subject: required\n- path: /rest/v1/webhooks/{webhookId}\n  method: delete\n  operationId: WebhookController.deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    audience: null\n    token:\n      max-ttl: 900\n    audit: required\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    subject: required\nx-correction: 'derive-agentic-access.py classified all 10 write operations as\
  \ safety-critical. That was\n  a false positive from its substring keyword match: every Vyond operationId is of the form ''<Name>Controller.<method>'',\n  and ''Controller'' contains the SAFETY_WORDS token ''control''. Reclassified here against the actual\n  semantics — the four credit-consuming operations (content generation v1/v2, Turbo, video export) are\n  ''physical'' because they spend real account credits irreversibly and exportVideo returns 402 Payment\n  Required when exhausted; the remaining six writes (SCIM user create/update/patch, webhook create/update/delete)\n  are ''write''. Nothing in this API is safety-critical. The upstream heuristic needs a word-boundary\n  match; every Controller-named spec in the network is affected.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/agentic-access/vyond-agentic-access.yml
summary_line: 20 operations · 10 acting
tags:
- Video
- Animation
- Video Generation
- Artificial Intelligence
- eLearning
- Learning and Development
- Content Generation
- SCIM
- Identity Provisioning
- Webhooks
- Enterprise
- Media
---
