---
acting_count: 80
action_class_counts:
  acting: 80
  connected: 59
api_specs:
- filename: opper-account-api-openapi.yml
  format: yaml
  label: Opper AI Account API
  slug: opper-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-account-api-openapi.yml
- filename: opper-artifacts-api-openapi.yml
  format: yaml
  label: Opper AI Artifacts API
  slug: opper-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-artifacts-api-openapi.yml
- filename: opper-audio-api-openapi.yml
  format: yaml
  label: Opper AI Audio API
  slug: opper-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-audio-api-openapi.yml
- filename: opper-compatibility-api-openapi.yml
  format: yaml
  label: Opper AI Compatibility API
  slug: opper-compatibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-compatibility-api-openapi.yml
- filename: opper-files-api-openapi.yml
  format: yaml
  label: Opper AI Files API
  slug: opper-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-files-api-openapi.yml
- filename: opper-functions-api-openapi.yml
  format: yaml
  label: Opper AI Functions API
  slug: opper-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-functions-api-openapi.yml
- filename: opper-generations-api-openapi.yml
  format: yaml
  label: Opper AI Generations API
  slug: opper-generations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-generations-api-openapi.yml
- filename: opper-images-api-openapi.yml
  format: yaml
  label: Opper AI Images API
  slug: opper-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-images-api-openapi.yml
- filename: opper-management-api-openapi.yml
  format: yaml
  label: Opper AI Management API
  slug: opper-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-management-api-openapi.yml
- filename: opper-models-api-openapi.yml
  format: yaml
  label: Opper AI Models API
  slug: opper-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-models-api-openapi.yml
- filename: opper-ocr-api-openapi.yml
  format: yaml
  label: Opper AI OCR API
  slug: opper-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-ocr-api-openapi.yml
- filename: opper-rerank-api-openapi.yml
  format: yaml
  label: Opper AI Rerank API
  slug: opper-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-rerank-api-openapi.yml
- filename: opper-roundtable-api-openapi.yml
  format: yaml
  label: Opper AI Roundtable API
  slug: opper-roundtable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-roundtable-api-openapi.yml
- filename: opper-spans-api-openapi.yml
  format: yaml
  label: Opper AI Spans API
  slug: opper-spans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-spans-api-openapi.yml
- filename: opper-system-api-openapi.yml
  format: yaml
  label: Opper AI System API
  slug: opper-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-system-api-openapi.yml
- filename: opper-tools-api-openapi.yml
  format: yaml
  label: Opper AI Tools API
  slug: opper-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-tools-api-openapi.yml
- filename: opper-traces-api-openapi.yml
  format: yaml
  label: Opper AI Traces API
  slug: opper-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-traces-api-openapi.yml
- filename: opper-user-delegation-api-openapi.yml
  format: yaml
  label: Opper AI User delegation API
  slug: opper-user-delegation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-user-delegation-api-openapi.yml
- filename: opper-videos-api-openapi.yml
  format: yaml
  label: Opper AI Videos API
  slug: opper-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/openapi/opper-videos-api-openapi.yml
consequence_counts:
  physical: 2
  read: 59
  safety-critical: 8
  write: 70
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 8
kind: agentic-access
layout: agentic-access
method: generated
name: Opper Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /management/v1/controls/rules
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /management/v1/controls/rules/{uuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /management/v1/controls/rules/{uuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /management/v1/invites/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /management/v1/management-keys/_self/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /user/v1/controls/rules
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /user/v1/controls/rules/{uuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /user/v1/controls/rules/{uuid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /management/v1/dynamic-routes/{name}/deploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /user/v1/dynamic-routes/{name}/deploy
operation_count: 139
overview: 'Opper AI exposes 139 API operations that an AI agent could call, of which 80 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 59 read, 70 write, 2 physical, and 8 safety-critical.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Opper AI
provider_slug: opper
slug: opper-agentic-access
source_filename: opper-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: generated\nsource: openapi/opper-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 139\n  by_action_class:\n    connected: 59\n    acting: 80\n  by_consequence:\n    read: 59\n    write: 70\n    safety-critical: 8\n    physical: 2\n  human_in_the_loop_required: 8\noperations:\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/mcp\n  method: post\n  operationId: callManagementMCP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/controls/rules\n  method: get\n  operationId: listManagementControlRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/v1/controls/rules\n  method: post\n  operationId: createManagementControlRule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /management/v1/controls/rules/{uuid}\n  method: delete\n  operationId: deleteManagementControlRule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /management/v1/controls/rules/{uuid}\n  method: patch\n  operationId: updateManagementControlRule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /management/v1/dynamic-routes\n  method: get\n  operationId: listManagementDynamicRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/v1/dynamic-routes\n  method: post\n  operationId: createManagementDynamicRoute\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/dynamic-routes/{name}\n  method: delete\n  operationId: deleteManagementDynamicRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/dynamic-routes/{name}\n  method: get\n  operationId: getManagementDynamicRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/v1/dynamic-routes/{name}\n  method: patch\n  operationId: updateManagementDynamicRouteMetadata\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/dynamic-routes/{name}/deploy\n  method: post\n  operationId: deployManagementDynamicRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/dynamic-routes/{name}/draft\n  method: put\n  operationId: updateManagementDynamicRouteDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/dynamic-routes/{name}/simulate\n  method: post\n  operationId: simulateManagementDynamicRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/dynamic-routes/{name}/versions\n  method: get\n  operationId: listManagementDynamicRouteVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/v1/dynamic-routes/{name}/versions/{version_number}\n  method: get\n  operationId: getManagementDynamicRouteVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/v1/dynamic-routes/{name}/versions/{version_number}/restore-to-draft\n  method: post\n  operationId: restoreManagementDynamicRouteVersionToDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/dynamic-routes/{name}/versions/{version_number}/rollback\n  method: post\n  operationId: rollbackManagementDynamicRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/invites\n  method: get\n  operationId: listManagementInvites\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/v1/invites\n  method: post\n  operationId: createManagementInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/invites/{id}\n  method: delete\n  operationId: revokeManagementInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /management/v1/management-keys/_self/disable\n  method: post\n  operationId:\
  \ disableCallingManagementKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /management/v1/members\n  method: get\n  operationId: listManagementMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/v1/members/{user_uuid}\n  method: delete\n  operationId: removeManagementMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/projects\n  method: get\n\
  \  operationId: listManagementProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/v1/projects\n  method: post\n  operationId: createManagementProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/projects/{uuid}\n  method: delete\n  operationId: deleteManagementProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/projects/{uuid}\n  method: get\n  operationId: getManagementProject\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/v1/projects/{uuid}\n  method: patch\n  operationId: updateManagementProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/projects/{uuid}/api-keys\n  method: get\n  operationId: listManagementAPIKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /management/v1/projects/{uuid}/api-keys\n  method: post\n  operationId: createManagementAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/projects/{uuid}/api-keys/{id}\n  method: delete\n  operationId: deleteManagementAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /management/v1/usage\n  method: get\n  operationId: getManagementUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: callUserMCP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/api-keys\n  method: get\n  operationId: userListOrganizationPersonalKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/api-keys\n  method: post\n  operationId: userCreateOrganizationPersonalKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/api-keys/{id}\n  method: delete\n  operationId: userDeleteOrganizationPersonalKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/api-keys/{id}/chat/completions\n  method: post\n  operationId: userCallModelWithOrgKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/api-keys/{id}/traces/{trace_id}\n  method: get\n  operationId: userGetTraceWithOrgKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/context\n  method: get\n  operationId: userGetContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/controls/allowed-models\n  method: get\n  operationId: userGetAllowedModels\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/controls/rules\n  method: get\n  operationId: userListManagementControlRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/controls/rules\n  method: post\n  operationId: userCreateManagementControlRule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/v1/controls/rules/{uuid}\n  method: delete\n  operationId: userDeleteManagementControlRule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/v1/controls/rules/{uuid}\n  method: patch\n  operationId: userUpdateManagementControlRule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /user/v1/controls/vocabulary\n  method: get\n  operationId: userGetControlVocabulary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/dynamic-routes\n  method: get\n  operationId: userListManagementDynamicRoutes\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/dynamic-routes\n  method: post\n  operationId: userCreateManagementDynamicRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/dynamic-routes/{name}\n  method: delete\n  operationId: userDeleteManagementDynamicRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/dynamic-routes/{name}\n  method: get\n  operationId: userGetManagementDynamicRoute\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/dynamic-routes/{name}\n  method: patch\n  operationId: userUpdateManagementDynamicRouteMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/dynamic-routes/{name}/deploy\n  method: post\n  operationId: userDeployManagementDynamicRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/dynamic-routes/{name}/draft\n  method:\
  \ put\n  operationId: userUpdateManagementDynamicRouteDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/dynamic-routes/{name}/simulate\n  method: post\n  operationId: userSimulateManagementDynamicRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/dynamic-routes/{name}/versions\n  method: get\n  operationId: userListManagementDynamicRouteVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /user/v1/dynamic-routes/{name}/versions/{version_number}\n  method: get\n  operationId: userGetManagementDynamicRouteVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/dynamic-routes/{name}/versions/{version_number}/restore-to-draft\n  method: post\n  operationId: userRestoreManagementDynamicRouteVersionToDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/dynamic-routes/{name}/versions/{version_number}/rollback\n  method: post\n  operationId: userRollbackManagementDynamicRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/guides/{topic}\n  method: get\n  operationId: userGetGuide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/models\n  method: get\n  operationId: userListModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/models/access\n  method: get\n  operationId: userCheckModelAccess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/projects\n  method: get\n  operationId: userListManagementProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /user/v1/projects\n  method: post\n  operationId: userCreateManagementProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/projects/{uuid}\n  method: delete\n  operationId: userDeleteManagementProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/projects/{uuid}\n  method: get\n  operationId: userGetManagementProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /user/v1/projects/{uuid}\n  method: patch\n  operationId: userUpdateManagementProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/projects/{uuid}/api-keys\n  method: get\n  operationId: userListManagementAPIKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/projects/{uuid}/api-keys\n  method: post\n  operationId: userCreateManagementAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /user/v1/projects/{uuid}/api-keys/{id}\n  method: delete\n  operationId: userDeleteManagementAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/projects/{uuid}/api-keys/{id}/chat/completions\n  method: post\n  operationId: userCallModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/v1/projects/{uuid}/api-keys/{id}/traces/{trace_id}\n  method: get\n  operationId: userGetTrace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /user/v1/traces\n  method: get\n  operationId: userListTraces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/v1/usage\n  method: get\n  operationId: userGetUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/artifacts/{id}\n  method: delete\n  operationId: deleteArtifact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/artifacts/{id}/status\n  method: get\n  operationId: getArtifactStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v3/audio/generations\n  method: post\n  operationId: createAudioGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/audio/models\n  method: get\n  operationId: listAudioModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/audio/music\n  method: post\n  operationId: createMusic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/audio/speech\n  method:\
  \ post\n  operationId: createSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/audio/transcriptions\n  method: post\n  operationId: createTranscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/audio/voices\n  method: get\n  operationId: listVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/audio/voices\n  method: post\n  operationId: createVoice\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/audio/voices/{id}\n  method: delete\n  operationId: deleteVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/audio/voices/{id}\n  method: get\n  operationId: getVoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/compat/audio/speech\n  method: post\n  operationId: createSpeechOpenAICompat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/compat/chat/completions\n  method: post\n  operationId: chatCompletions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/compat/decisions\n  method: post\n  operationId: createDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/compat/embeddings\n  method: post\n  operationId: createEmbeddings\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/compat/models\n  method: get\n  operationId: listOpenAICompatModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/compat/openresponses\n  method: post\n  operationId: createOpenResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/compat/responses\n  method: post\n  operationId: createResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/compat/v1/messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/compat/v1/messages/count_tokens\n  method: post\n  operationId: countMessageTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/compat/v1/models\n  method: get\n  operationId: listAnthropicCompatModels\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/compat/v1/systemone\n  method: post\n  operationId: evaluateSystemOne\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/compat/v1beta/interactions\n  method: post\n  operationId: createInteraction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/compat/v1beta/models/{model}:countTokens\n  method: post\n  operationId: countTokens\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/compat/v1beta/models/{model}:generateContent\n  method: post\n  operationId: generateContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/compat/v1beta/models/{model}:streamGenerateContent\n  method: post\n  operationId: streamGenerateContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /v3/files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/files/usage\n  method: get\n  operationId: getFilesUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (41 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/agentic-access/opper-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opper/refs/heads/main/agentic-access/opper-agentic-access.yml
summary_line: 139 operations · 80 acting · 8 human-in-the-loop
tags:
- Artificial Intelligence
- Gateways
- European
- OpenAI-Compatible
- GDPR
---
