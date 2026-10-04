---
acting_count: 60
action_class_counts:
  acting: 60
  connected: 38
api_specs:
- filename: anchorbrowser-agentic-capabilities-api-openapi.yml
  format: yaml
  label: Anchor Browser Agentic capabilities API
  slug: anchorbrowser-agentic-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-agentic-capabilities-api-openapi.yml
- filename: anchorbrowser-ai-tools-api-openapi.yml
  format: yaml
  label: Anchor Browser AI Tools API
  slug: anchorbrowser-ai-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-ai-tools-api-openapi.yml
- filename: anchorbrowser-applications-api-openapi.yml
  format: yaml
  label: Anchor Browser Applications API
  slug: anchorbrowser-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-applications-api-openapi.yml
- filename: anchorbrowser-batch-sessions-api-openapi.yml
  format: yaml
  label: Anchor Browser Batch Sessions API
  slug: anchorbrowser-batch-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-batch-sessions-api-openapi.yml
- filename: anchorbrowser-billing-api-openapi.yml
  format: yaml
  label: Anchor Browser Billing API
  slug: anchorbrowser-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-billing-api-openapi.yml
- filename: anchorbrowser-browser-sessions-api-openapi.yml
  format: yaml
  label: Anchor Browser Sessions API
  slug: anchorbrowser-browser-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-browser-sessions-api-openapi.yml
- filename: anchorbrowser-certificates-api-openapi.yml
  format: yaml
  label: Anchor Browser Certificates API
  slug: anchorbrowser-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-certificates-api-openapi.yml
- filename: anchorbrowser-event-coordination-api-openapi.yml
  format: yaml
  label: Anchor Browser Event Coordination API
  slug: anchorbrowser-event-coordination-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-event-coordination-api-openapi.yml
- filename: anchorbrowser-extensions-api-openapi.yml
  format: yaml
  label: Anchor Browser Extensions API
  slug: anchorbrowser-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-extensions-api-openapi.yml
- filename: anchorbrowser-identities-api-openapi.yml
  format: yaml
  label: Anchor Browser Identities API
  slug: anchorbrowser-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-identities-api-openapi.yml
- filename: anchorbrowser-integrations-api-openapi.yml
  format: yaml
  label: Anchor Browser Integrations API
  slug: anchorbrowser-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-integrations-api-openapi.yml
- filename: anchorbrowser-os-level-control-api-openapi.yml
  format: yaml
  label: Anchor Browser OS Level Control API
  slug: anchorbrowser-os-level-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-os-level-control-api-openapi.yml
- filename: anchorbrowser-profiles-api-openapi.yml
  format: yaml
  label: Anchor Browser Profiles API
  slug: anchorbrowser-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-profiles-api-openapi.yml
- filename: anchorbrowser-session-recordings-api-openapi.yml
  format: yaml
  label: Anchor Browser Session Recordings API
  slug: anchorbrowser-session-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-session-recordings-api-openapi.yml
- filename: anchorbrowser-tasks-api-openapi.yml
  format: yaml
  label: Anchor Browser Tasks API
  slug: anchorbrowser-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-tasks-api-openapi.yml
- filename: anchorbrowser-tasks-legacy-api-openapi.yml
  format: yaml
  label: Anchor Browser Tasks (Legacy) API
  slug: anchorbrowser-tasks-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-tasks-legacy-api-openapi.yml
- filename: anchorbrowser-tools-api-openapi.yml
  format: yaml
  label: Anchor Browser Tools API
  slug: anchorbrowser-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-tools-api-openapi.yml
consequence_counts:
  physical: 1
  read: 38
  safety-critical: 13
  write: 46
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 13
kind: agentic-access
layout: agentic-access
method: generated
name: Anchorbrowser Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/clipboard
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/copy
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/drag-and-drop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/goto
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/keyboard/shortcut
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/keyboard/type
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/mouse/click
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/mouse/doubleClick
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/mouse/down
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/mouse/move
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/mouse/up
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/paste
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/scroll
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/task/{taskId}/deploy
operation_count: 98
overview: 'Anchor Browser exposes 98 API operations that an AI agent could call, of which 60 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read, 46 write, 1 physical, and 13 safety-critical.


  13 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Anchor Browser
provider_slug: anchorbrowser
slug: anchorbrowser-agentic-access
source_filename: anchorbrowser-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/anchorbrowser-agentic-capabilities-api-openapi.yml, openapi/anchorbrowser-ai-tools-api-openapi.yml,\n  openapi/anchorbrowser-applications-api-openapi.yml, openapi/anchorbrowser-batch-sessions-api-openapi.yml,\n  openapi/anchorbrowser-billing-api-openapi.yml, openapi/anchorbrowser-browser-sessions-api-openapi.yml,\n  openapi/anchorbrowser-certificates-api-openapi.yml, openapi/anchorbrowser-event-coordination-api-openapi.yml,\n  openapi/anchorbrowser-extensions-api-openapi.yml, openapi/anchorbrowser-identities-api-openapi.yml,\n  openapi/anchorbrowser-integrations-api-openapi.yml, openapi/anchorbrowser-os-level-control-api-openapi.yml,\n  openapi/anchorbrowser-profiles-api-openapi.yml, openapi/anchorbrowser-session-recordings-api-openapi.yml,\n  openapi/anchorbrowser-tasks-api-openapi.yml, openapi/anchorbrowser-tasks-legacy-api-openapi.yml,\n  openapi/anchorbrowser-tools-api-openapi.yml\ndescription: Recommended x-agentic-access\
  \ execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 98\n  by_action_class:\n    acting: 60\n    connected: 38\n  by_consequence:\n    write: 46\n    read: 38\n    safety-critical: 13\n    physical: 1\n  human_in_the_loop_required: 13\noperations:\n- path: /v1/sessions/{sessionId}/agent/files\n  method: post\n  operationId: postV1SessionsBySessionIdAgentFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{sessionId}/agent/files\n  method: get\n  operationId: getV1SessionsBySessionIdAgentFiles\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}/agent/pause\n  method: post\n  operationId: postV1SessionsBySessionIdAgentPause\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/agent/resume\n  method: post\n  operationId: postV1SessionsBySessionIdAgentResume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/perform-web-task\n  method: post\n  operationId: postV1ToolsPerformWebTask\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/perform-web-task/{workflowId}/status\n  method: get\n  operationId: getV1ToolsPerformWebTaskByWorkflowIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications\n  method: post\n  operationId: postV1Applications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications\n  method: get\n  operationId: getV1Applications\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/{applicationId}\n  method: get\n  operationId: getV1ApplicationsByApplicationId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/{applicationId}\n  method: delete\n  operationId: deleteV1ApplicationsByApplicationId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications/{applicationId}/identities\n  method: get\n  operationId: getV1ApplicationsByApplicationIdIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/applications/{applicationId}/auth-flows\n  method: get\n  operationId: getV1ApplicationsByApplicationIdAuthFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/{applicationId}/auth-flows\n  method: post\n  operationId: postV1ApplicationsByApplicationIdAuthFlows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications/{applicationId}/auth-flows/{authFlowId}\n  method: patch\n  operationId: patchV1ApplicationsByApplicationIdAuthFlowsByAuthFlowId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications/{applicationId}/auth-flows/{authFlowId}\n  method: delete\n  operationId: deleteV1ApplicationsByApplicationIdAuthFlowsByAuthFlowId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications/{applicationId}/tokens\n  method: post\n  operationId: postV1ApplicationsByApplicationIdTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch-sessions\n  method: get\n  operationId: getV1BatchSessions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch-sessions\n  method: post\n  operationId: postV1BatchSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch-sessions/{batch_id}\n  method: get\n  operationId: getV1BatchSessionsByBatchId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch-sessions/{batch_id}\n  method: patch\n  operationId: patchV1BatchSessionsByBatchId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch-sessions/{batch_id}\n  method: delete\n  operationId: deleteV1BatchSessionsByBatchId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch-sessions/{batch_id}/retry\n  method: post\n  operationId: postV1BatchSessionsByBatchIdRetry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing\n  method: get\n  operationId: getV1Billing\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions\n  method: get\n  operationId: getV1Sessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions\n  method: post\n  operationId: postV1Sessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/async\n  method: post\n  operationId: postV1SessionsAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/sessions/async/{request_id}/status\n  method: get\n  operationId: getV1SessionsAsyncByRequestIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/all\n  method: delete\n  operationId: deleteV1SessionsAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/all/status\n  method: get\n  operationId: getV1SessionsAllStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/history\n  method: get\n  operationId: getV1SessionsHistory\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}\n  method: get\n  operationId: getV1SessionsBySessionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}\n  method: delete\n  operationId: deleteV1SessionsBySessionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/pages\n  method: get\n  operationId: getV1SessionsBySessionIdPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{sessionId}/uploads\n \
  \ method: post\n  operationId: postV1SessionsBySessionIdUploads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/downloads\n  method: get\n  operationId: getV1SessionsBySessionIdDownloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/certificates\n  method: post\n  operationId: postV1Certificates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/certificates\n  method: get\n  operationId:\
  \ getV1Certificates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/certificates/{name}\n  method: delete\n  operationId: deleteV1CertificatesByName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/events/{event_name}/wait\n  method: post\n  operationId: postV1EventsByEventNameWait\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/events/{event_name}\n  method: post\n  operationId: postV1EventsByEventName\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/extensions\n  method: post\n  operationId: postV1Extensions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/extensions\n  method: get\n  operationId: getV1Extensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/extensions/{id}\n  method: get\n  operationId: getV1ExtensionsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/extensions/{id}\n  method: delete\n  operationId: deleteV1ExtensionsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/identities\n  method: post\n  operationId: postV1Identities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/identities/{identityId}\n  method: get\n  operationId: getV1IdentitiesByIdentityId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/identities/{identityId}\n  method: put\n  operationId: putV1IdentitiesByIdentityId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/identities/{identityId}\n  method: delete\n  operationId: deleteV1IdentitiesByIdentityId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations\n  method: post\n  operationId: postV1Integrations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations\n  method: get\n  operationId: getV1Integrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrations/{integrationId}\n  method: delete\n  operationId: deleteV1IntegrationsByIntegrationId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{sessionId}/screenshot\n  method: get\n  operationId: getV1SessionsBySessionIdScreenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/sessions/{sessionId}/mouse/click\n  method: post\n  operationId: postV1SessionsBySessionIdMouseClick\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sessions/{sessionId}/mouse/doubleClick\n  method: post\n  operationId: postV1SessionsBySessionIdMouseDoubleClick\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sessions/{sessionId}/mouse/down\n  method: post\n  operationId: postV1SessionsBySessionIdMouseDown\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sessions/{sessionId}/mouse/up\n  method: post\n  operationId: postV1SessionsBySessionIdMouseUp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sessions/{sessionId}/mouse/move\n  method: post\n  operationId: postV1SessionsBySessionIdMouseMove\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sessions/{sessionId}/drag-and-drop\n  method: post\n  operationId: postV1SessionsBySessionIdDragAndDrop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sessions/{sessionId}/scroll\n  method: post\n  operationId: postV1SessionsBySessionIdScroll\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /v1/sessions/{sessionId}/keyboard/type\n  method: post\n  operationId: postV1SessionsBySessionIdKeyboardType\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sessions/{sessionId}/keyboard/shortcut\n  method: post\n  operationId: postV1SessionsBySessionIdKeyboardShortcut\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sessions/{sessionId}/clipboard\n  method: get\n  operationId: getV1SessionsBySessionIdClipboard\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{sessionId}/clipboard\n  method: post\n  operationId: postV1SessionsBySessionIdClipboard\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sessions/{sessionId}/copy\n  method: post\n  operationId: postV1SessionsBySessionIdCopy\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sessions/{sessionId}/paste\n\
  \  method: post\n  operationId: postV1SessionsBySessionIdPaste\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sessions/{sessionId}/goto\n  method: post\n  operationId: postV1SessionsBySessionIdGoto\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/profiles\n  method: post\n  operationId: postV1Profiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiles\n  method: get\n  operationId: getV1Profiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles/{name}\n  method: get\n  operationId: getV1ProfilesByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles/{name}\n  method: delete\n  operationId: deleteV1ProfilesByName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/recordings/pause\n  method:\
  \ post\n  operationId: postV1SessionsBySessionIdRecordingsPause\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/recordings/resume\n  method: post\n  operationId: postV1SessionsBySessionIdRecordingsResume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{session_id}/recordings\n  method: get\n  operationId: getV1SessionsBySessionIdRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/sessions/{session_id}/recordings/primary/fetch\n  method: get\n  operationId: getV1SessionsBySessionIdRecordingsPrimaryFetch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}/recordings/{recording_id}\n  method: delete\n  operationId: deleteV1SessionsBySessionIdRecordingsByRecordingId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/{taskId}/run\n  method: post\n  operationId: postV2TasksByTaskIdRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tasks/runs/{runId}/status\n  method: get\n  operationId: getV2TasksRunsByRunIdStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/task\n  method: post\n  operationId: postV1Task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/task\n  method: get\n  operationId: getV1Task\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/task/run\n  method: post\n  operationId: postV1TaskRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/task/run/{taskName}\n  method: post\n  operationId: postV1TaskRunByTaskName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/task/{taskId}\n  method: get\n  operationId: getV1TaskByTaskId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/task/{taskId}\n  method: put\n  operationId: putV1TaskByTaskId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/task/{taskId}\n  method: delete\n  operationId: deleteV1TaskByTaskId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/task/{taskId}/versions\n  method: get\n  operationId: getV1TaskByTaskIdVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/task/{taskId}/latest\n  method: get\n  operationId: getV1TaskByTaskIdLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/task/{taskId}/draft\n\
  \  method: get\n  operationId: getV1TaskByTaskIdDraft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/task/{taskId}/draft\n  method: post\n  operationId: postV1TaskByTaskIdDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/task/{taskId}/deploy\n  method: post\n  operationId: postV1TaskByTaskIdDeploy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/task/{taskId}/executions\n\
  \  method: get\n  operationId: getV1TaskByTaskIdExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/task/{taskId}/executions/{executionId}\n  method: get\n  operationId: getV1TaskByTaskIdExecutionsByExecutionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/task/{taskId}/{taskVersion}\n  method: get\n  operationId: getV1TaskByTaskIdByTaskVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/task/{taskId}/{taskVersion}\n  method: post\n  operationId: postV1TaskByTaskIdByTaskVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/task/{taskId}/{taskVersion}\n  method: delete\n  operationId: deleteV1TaskByTaskIdByTaskVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/fetch-webpage\n  method: post\n  operationId: postV1ToolsFetchWebpage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tools/fetch/webpage\n  method: post\n  operationId: postV1ToolsFetchWebpage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/screenshot\n  method: post\n  operationId: postV1ToolsScreenshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tools/page-pdf\n  method: post\n  operationId: postV1ToolsPagePdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/agentic-access/anchorbrowser-agentic-access.yml
summary_line: 98 operations · 60 acting · 13 human-in-the-loop
tags:
- Browser Infrastructure
- AI Agents
- Cloud Browser
- Browser Automation
- Sandbox
- Stealth Browser
- MCP
---
