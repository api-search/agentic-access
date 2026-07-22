---
acting_count: 52
action_class_counts:
  acting: 52
  connected: 48
api_specs:
- filename: outrival-v1-openapi-original.json
  format: json
  label: OutRival API v1
  slug: outrival-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outrival/refs/heads/main/openapi/outrival-v1-openapi-original.json
- filename: outrival-v2-openapi-original.json
  format: json
  label: OutRival API v2
  slug: outrival-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outrival/refs/heads/main/openapi/outrival-v2-openapi-original.json
consequence_counts:
  read: 48
  safety-critical: 52
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 52
kind: agentic-access
layout: agentic-access
method: generated
name: Outrival Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rest/v1/ai-chats/messages
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rest/v1/assistants
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rest/v1/assistants/duplicate/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /rest/v1/assistants/{assistantId}/chat
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /rest/v1/assistants/{assistantId}/sms
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /rest/v1/assistants/{assistantId}/theme
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /rest/v1/assistants/{assistantId}/voice
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /rest/v1/assistants/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /rest/v1/assistants/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rest/v1/call/phone
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rest/v1/files/upload
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /rest/v1/files/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rest/v1/organization/keys
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rest/v1/organization/keys
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /rest/v1/organization/keys/{keyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /rest/v1/organization/keys/{keyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /rest/v1/organization/keys/{keyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /rest/v1/organization/keys/{keyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rest/v1/organization/token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rest/v1/organization/token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rest/v1/settings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /rest/v1/settings/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /rest/v1/settings/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rest/v1/webhooks/vapi/custom-llm/chat/completions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rest/v1/webhooks/vapi/server-messages
operation_count: 100
overview: 'OutRival exposes 100 API operations that an AI agent could call, of which 52 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 48 read and 52 safety-critical.


  52 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OutRival
provider_slug: outrival
slug: outrival-agentic-access
source_filename: outrival-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/outrival-v1-openapi-original.json, openapi/outrival-v2-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 100\n  by_action_class:\n    acting: 52\n    connected: 48\n  by_consequence:\n    safety-critical: 52\n    read: 48\n  human_in_the_loop_required: 52\noperations:\n- path: /rest/v1/assistants\n  method: post\n  operationId: AssistantsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /rest/v1/assistants\n  method: get\n  operationId: AssistantsController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/assistants/templates\n  method: get\n  operationId: AssistantsController_findAllTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/assistants/{id}\n  method: get\n  operationId: AssistantsController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/assistants/{id}\n  method: patch\n  operationId: AssistantsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/assistants/{id}\n  method: delete\n  operationId: AssistantsController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/assistants/duplicate/{id}\n  method: post\n  operationId: AssistantsController_duplicate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/assistants/{assistantId}/voice\n\
  \  method: patch\n  operationId: VoiceController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/assistants/{assistantId}/voice\n  method: get\n  operationId: VoiceController_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/assistants/{assistantId}/sms\n  method: patch\n  operationId: SmsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /rest/v1/assistants/{assistantId}/sms\n  method: get\n  operationId: SmsController_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/assistants/{assistantId}/chat\n  method: patch\n  operationId: ChatController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/assistants/{assistantId}/chat\n  method: get\n  operationId: ChatController_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/assistants/{assistantId}/theme\n  method:\
  \ patch\n  operationId: ThemeController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/assistants/{assistantId}/theme\n  method: get\n  operationId: ThemeController_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/assistants/{assistantId}/logs\n  method: get\n  operationId: AssistantLogsController_logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/assistants/{assistantId}/log/{logId}\n  method: get\n  operationId: AssistantLogsController_log\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/settings/secret\n  method: get\n  operationId: SettingsController_generateWebhookSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/settings\n  method: get\n  operationId: SettingsController_getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/settings\n  method: post\n  operationId: SettingsController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /rest/v1/settings/{id}\n  method: patch\n  operationId: SettingsController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/settings/{id}\n  method: delete\n  operationId: SettingsController_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/organization\n  method: get\n  operationId: OrganizationController_getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/organization/token\n  method: post\n  operationId: OrganizationController_generateOrganizationToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/organization/keys\n  method: get\n  operationId: OrganizationKeysController_getOrganizationKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/organization/keys\n  method: post\n  operationId: OrganizationKeysController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/organization/keys/public\n  method: get\n  operationId: OrganizationKeysController_getOrganizationPublicKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/organization/keys/{keyId}\n  method: get\n  operationId: OrganizationKeysController_getOrganizationKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/organization/keys/{keyId}\n  method: patch\n  operationId: OrganizationKeysController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/organization/keys/{keyId}\n  method: delete\n  operationId: OrganizationKeysController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/ai-chats/messages\n  method: post\n  operationId: MessagesController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/files/upload\n\
  \  method: post\n  operationId: FilesController_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/files\n  method: get\n  operationId: FilesController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/files/{id}/download\n  method: get\n  operationId: FilesController_getDownloadLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/files/{id}\n  method: delete\n  operationId: FilesController_deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/webhooks/vapi/server-messages\n  method: post\n  operationId: VapiWebhooksController_onServerMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/webhooks/vapi/custom-llm/chat/completions\n  method: post\n  operationId: VapiWebhooksController_onOpenAICustomLLMCall\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/call/phone\n  method: post\n  operationId: VapiController_phoneCallInitiate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/projects\n  method: get\n  operationId: WorkflowProjectController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/projects\n  method: post\n  operationId: WorkflowProjectController_createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/projects/{id}\n  method: get\n  operationId: WorkflowProjectController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/projects/{id}\n  method: patch\n  operationId: WorkflowProjectController_updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/projects/{id}\n  method: delete\n  operationId: WorkflowProjectController_deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/projects/{id}/workflows\n  method: get\n  operationId: WorkflowProjectController_projectWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/projects/{id}/deployments\n  method: get\n  operationId: WorkflowProjectController_projectWorkflowDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/projects/{projectId}/variables\n  method: get\n  operationId: VariableController_getAllVariables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/projects/{projectId}/variables\n  method: post\n  operationId: VariableController_createVariable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/projects/{projectId}/variables/{variableId}\n  method: patch\n  operationId: VariableController_updateVariable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/projects/{projectId}/variables/{variableId}\n  method: delete\n\
  \  operationId: VariableController_deleteVariable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/workflows\n  method: get\n  operationId: WorkflowController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/workflows\n  method: post\n  operationId: WorkflowController_createWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /rest/v2/workflows/{id}\n  method: get\n  operationId: WorkflowController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/workflows/{id}\n  method: patch\n  operationId: WorkflowController_updateWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/workflows/{id}\n  method: delete\n  operationId: WorkflowController_deleteWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/workflows/{id}/nodes\n  method: get\n  operationId: WorkflowController_nodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/workflows/{id}/nodes\n  method: post\n  operationId: WorkflowController_addNode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/workflows/{id}/nodes/config\n  method: get\n  operationId: WorkflowController_nodesWithConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/workflows/{id}/edges\n\
  \  method: get\n  operationId: WorkflowController_edges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/edges\n  method: get\n  operationId: EdgeController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/edges\n  method: post\n  operationId: EdgeController_createEdge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/edges/{id}\n  method: get\n  operationId: EdgeController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/edges/{id}\n  method: patch\n  operationId: EdgeController_updateEdge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/edges/{id}\n  method: delete\n  operationId: EdgeController_deleteEdge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/nodes\n  method: get\n  operationId: NodeController_findAll\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/nodes/{id}\n  method: get\n  operationId: NodeController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/nodes/{id}\n  method: patch\n  operationId: NodeController_update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/nodes/{id}\n  method: delete\n  operationId: NodeController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/nodes/duplicate/{id}\n  method: post\n  operationId: NodeController_duplicate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/nodes/{id}/config\n  method: get\n  operationId: NodeController_nodeWithConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/nodes/{nodeId}/voice\n  method: patch\n  operationId: VoiceConfigController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/nodes/{nodeId}/voice\n  method: get\n  operationId: VoiceConfigController_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/nodes/{nodeId}/sms\n  method: patch\n  operationId: SmsConfigController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/nodes/{nodeId}/sms\n  method: get\n  operationId: SmsConfigController_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/nodes/{nodeId}/chat\n  method: patch\n  operationId: ChatConfigController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/nodes/{nodeId}/chat\n  method: get\n  operationId: ChatConfigController_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/deployments/{id}\n  method: get\n  operationId: WorkflowDeploymentController_projectWorkflowDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /rest/v2/deployments/{id}\n  method: delete\n  operationId: WorkflowDeploymentController_deleteWorkflowDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/deployments/{id}\n  method: post\n  operationId: WorkflowDeploymentController_updateWorkflowDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/deployments\n  method: post\n  operationId: WorkflowDeploymentController_createWorkflowDeployment\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/deployments/{workflowDeploymentId}/theme\n  method: patch\n  operationId: ThemeController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/deployments/{workflowDeploymentId}/theme\n  method: get\n  operationId: ThemeController_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/organization\n\
  \  method: get\n  operationId: OrganizationController_getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/organization/token\n  method: post\n  operationId: OrganizationController_generateOrganizationToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/organization/keys\n  method: get\n  operationId: OrganizationKeysController_getOrganizationKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/organization/keys\n  method: post\n  operationId: OrganizationKeysController_create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/organization/keys/public\n  method: get\n  operationId: OrganizationKeysController_getOrganizationPublicKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/organization/keys/{keyId}\n  method: get\n  operationId: OrganizationKeysController_getOrganizationKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/organization/keys/{keyId}\n  method: patch\n  operationId: OrganizationKeysController_update\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v1/organization/keys/{keyId}\n  method: delete\n  operationId: OrganizationKeysController_remove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/ai-chats/messages\n  method: post\n  operationId: MessagesController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/ai-chats/{aiChatId}/sessions\n  method: get\n  operationId: SessionsController_getByChatId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/ai-chats/project/{projectId}/sessions\n  method: get\n  operationId: SessionsController_getByProjectId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/ai-chats/sessions/{sessionId}/logs\n  method: get\n  operationId: SessionsController_getBySession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/ai-chats/{AiChatId}/logs\n  method: get\n  operationId: SessionsController_getByAiChat\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/ai-chats/user/{userId}/logs\n  method: get\n  operationId: SessionsController_getByUserId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/ai-chats/workflow/{workflowId}/logs\n  method: get\n  operationId: SessionsController_getByWorkflowId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/call/phone\n  method: post\n  operationId: VapiController_phoneCallInitiate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n \
  \     human-in-the-loop: required\n    audit: required\n- path: /rest/v2/call/phone-numbers\n  method: get\n  operationId: VapiController_getActivePhoneNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v2/webhooks/vapi/server-messages\n  method: post\n  operationId: VapiWebhooksController_onServerMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rest/v2/webhooks/vapi/custom-llm/chat/completions\n  method: post\n  operationId: VapiWebhooksController_onOpenAICustomLLMCall\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    aud\n\n# --- truncated\
  \ at 32 KB (32 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/outrival/refs/heads/main/agentic-access/outrival-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outrival/refs/heads/main/agentic-access/outrival-agentic-access.yml
summary_line: 100 operations · 52 acting · 52 human-in-the-loop
tags:
- Company
- Enterprise Saas
- Conversational AI
- AI Agents
- Voice
- SMS
- Customer Engagement
- Chatbots
- Contact Center
- Webhooks
---
