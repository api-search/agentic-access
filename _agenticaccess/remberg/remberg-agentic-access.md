---
acting_count: 65
action_class_counts:
  acting: 65
  connected: 50
api_specs:
- filename: remberg-assets-openapi.json
  format: json
  label: remberg Assets API
  slug: remberg-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-assets-openapi.json
- filename: remberg-work-orders-openapi.json
  format: json
  label: remberg Work Orders API
  slug: remberg-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-work-orders-openapi.json
- filename: remberg-work-requests-openapi.json
  format: json
  label: remberg Work Requests API
  slug: remberg-work-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-work-requests-openapi.json
- filename: remberg-tickets-openapi.json
  format: json
  label: remberg Tickets API
  slug: remberg-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-tickets-openapi.json
- filename: remberg-parts-openapi.json
  format: json
  label: remberg Parts API
  slug: remberg-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-parts-openapi.json
- filename: remberg-organizations-openapi.json
  format: json
  label: remberg Organizations API
  slug: remberg-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-organizations-openapi.json
- filename: remberg-contacts-openapi.json
  format: json
  label: remberg Contacts API
  slug: remberg-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-contacts-openapi.json
- filename: remberg-users-openapi.json
  format: json
  label: remberg Users API
  slug: remberg-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-users-openapi.json
- filename: remberg-files-openapi.json
  format: json
  label: remberg Files API
  slug: remberg-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-files-openapi.json
- filename: remberg-forms-openapi.json
  format: json
  label: remberg Forms API
  slug: remberg-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-forms-openapi.json
- filename: remberg-procedures-openapi.json
  format: json
  label: remberg Procedures API
  slug: remberg-procedures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-procedures-openapi.json
- filename: remberg-ai-openapi.json
  format: json
  label: remberg AI Copilot API
  slug: remberg-ai-copilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-ai-openapi.json
consequence_counts:
  physical: 14
  read: 50
  safety-critical: 10
  write: 41
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 10
kind: agentic-access
layout: agentic-access
method: generated
name: Remberg Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/ai/answer
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/ai/feedback/{traceId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/contacts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/contacts/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/contacts/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/organizations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/organizations/number/{organizationNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/organizations/number/{organizationNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/organizations/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/organizations/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/users/{id}/invite
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/work-orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/work-orders/erp/{externalReference}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/work-orders/erp/{externalReference}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/work-orders/erp/{externalReference}/checklist
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/work-orders/erp/{externalReference}/procedures
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/work-orders/erp/{externalReference}/procedures/{procedureInstanceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/work-orders/erp/{externalReference}/stock-changes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/work-orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/work-orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/work-orders/{id}/checklist
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/work-orders/{id}/procedures
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/work-orders/{id}/procedures/{procedureInstanceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/work-orders/{id}/stock-changes
operation_count: 115
overview: 'Remberg exposes 115 API operations that an AI agent could call, of which 65 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 50 read, 41 write, 14 physical, and 10 safety-critical.


  10 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Remberg
provider_slug: remberg
slug: remberg-agentic-access
source_filename: remberg-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/remberg-ai-openapi.json, openapi/remberg-assets-openapi.json, openapi/remberg-contacts-openapi.json,\n  openapi/remberg-files-openapi.json, openapi/remberg-forms-openapi.json, openapi/remberg-organizations-openapi.json,\n  openapi/remberg-parts-openapi.json, openapi/remberg-procedures-openapi.json, openapi/remberg-tickets-openapi.json,\n  openapi/remberg-users-openapi.json, openapi/remberg-work-orders-openapi.json, openapi/remberg-work-requests-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 115\n  by_action_class:\n    acting: 65\n    connected: 50\n  by_consequence:\n    safety-critical: 10\n    read: 50\n    write: 41\n    physical: 14\n  human_in_the_loop_required:\
  \ 10\noperations:\n- path: /v1/ai/answer\n  method: post\n  operationId: AiCopilotCfaController_getAnswer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/ai/feedback/{traceId}\n  method: post\n  operationId: AiCopilotCfaController_provideFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/assets/failure-types\n  method: get\n  operationId: /v2/assets/failure-types_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/failure-types\n  method: post\n  operationId: /v2/assets/failure-types_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/failure-types/{reference}\n  method: patch\n  operationId: /v2/assets/failure-types/{reference}_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/failure-types/{reference}\n  method: delete\n  operationId: /v2/assets/failure-types/{reference}_delete\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/types/{id}\n  method: get\n  operationId: /v2/assets/types/{id}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/types/{id}\n  method: patch\n  operationId: /v2/assets/types/{id}_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/types/{id}\n  method: delete\n  operationId: /v2/assets/types/{id}_delete\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/types/label/{assetTypeLabel}\n  method: get\n  operationId: /v2/assets/types/label/{assetTypeLabel}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/types/label/{assetTypeLabel}\n  method: patch\n  operationId: /v2/assets/types/label/{assetTypeLabel}_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/types/label/{assetTypeLabel}\n  method: delete\n  operationId: /v2/assets/types/label/{assetTypeLabel}_delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/types\n  method: post\n  operationId: /v2/assets/types_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/{id}/status-signals\n  method: post\n  operationId: /v2/assets/{id}/status-signals_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/assets/{id}/status-signals\n  method: get\n  operationId: /v2/assets/{id}/status-signals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/number/{assetNumber}/status-signals\n  method: post\n  operationId: /v2/assets/number/{assetNumber}/status-signals_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/number/{assetNumber}/status-signals\n  method: get\n  operationId: /v2/assets/number/{assetNumber}/status-signals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/{id}/status-signals/resolve\n\
  \  method: patch\n  operationId: /v2/assets/{id}/status-signals/resolve_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/number/{assetNumber}/status-signals/resolve\n  method: patch\n  operationId: /v2/assets/number/{assetNumber}/status-signals/resolve_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/status-signals\n  method: get\n  operationId: /v2/assets/status-signals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /v2/assets\n  method: get\n  operationId: /v2/assets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets\n  method: post\n  operationId: /v2/assets_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/{id}\n  method: get\n  operationId: /v2/assets/{id}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/{id}\n  method: patch\n  operationId: /v2/assets/{id}_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/{id}\n  method: delete\n  operationId: /v2/assets/{id}_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/number/{assetNumber}\n  method: get\n  operationId: /v2/assets/number/{assetNumber}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/number/{assetNumber}\n  method: patch\n  operationId: /v2/assets/number/{assetNumber}_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/number/{assetNumber}\n  method: delete\n  operationId: /v2/assets/number/{assetNumber}_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/assets/number/{assetNumber}/inventories\n  method: get\n  operationId: /v2/assets/number/{assetNumber}/inventories_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/assets/{id}/inventories\n  method: get\n  operationId: /v2/assets/{id}/inventories_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts/{id}\n  method: get\n  operationId: ContactsCfaController_findOne\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts/{id}\n  method: patch\n  operationId: ContactsCfaController_updateOne\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/contacts/{id}\n  method: delete\n  operationId: ContactsCfaController_deleteOne\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/contacts\n  method: get\n  operationId: ContactsCfaController_findMany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/contacts\n  method: post\n  operationId: ContactsCfaController_createOne\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/files\n  method: get\n  operationId: /v1/files_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files\n  method: post\n  operationId:\
  \ /v1/files_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files/resolve\n  method: get\n  operationId: /v1/files/resolve_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{id}\n  method: get\n  operationId: /v1/files/{id}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{id}\n  method: patch\n  operationId: /v1/files/{id}_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files/{id}\n  method: delete\n  operationId: /v1/files/{id}_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files/{id}/download\n  method: get\n  operationId: /v1/files/{id}/download_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/folder\n  method: post\n  operationId: /v1/files/folder_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/files/{id}/content\n  method: patch\n  operationId: /v1/files/{id}/content_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/forms\n  method: get\n  operationId: /v1/forms_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/forms/{id}\n  method: get\n  operationId: /v1/forms/{id}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/number/{organizationNumber}\n  method: get\n  operationId: OrganizationsCfaController_findOneByOrganizationNumber\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/number/{organizationNumber}\n  method: patch\n  operationId: OrganizationsCfaController_updateOneByOrganizationNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/organizations/number/{organizationNumber}\n  method: delete\n  operationId: OrganizationsCfaController_deleteOneByOrganizationNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /v1/organizations/{id}\n  method: get\n  operationId: OrganizationsCfaController_findOneById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{id}\n  method: patch\n  operationId: OrganizationsCfaController_updateOneById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/organizations/{id}\n  method: delete\n  operationId: OrganizationsCfaController_deleteOneById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/organizations\n  method: get\n  operationId: OrganizationsCfaController_findMany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations\n  method: post\n  operationId: OrganizationsCfaController_createOne\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/organizations/{id}/contacts\n  method: get\n  operationId: OrganizationsCfaController_findManyContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/parts/{partTypeId}/inventories/storage/{storageAssetId}\n  method: get\n  operationId: /v2/parts/{partTypeId}/inventories/storage/{storageAssetId}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts/{partTypeId}/inventories/storage/{storageAssetId}\n  method: post\n  operationId: /v2/parts/{partTypeId}/inventories/storage/{storageAssetId}_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/number/{partNumber}/inventories/storage/number/{storageAssetNumber}\n  method: get\n  operationId: /v2/parts/number/{partNumber}/inventories/storage/number/{storageAssetNumber}_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts/number/{partNumber}/inventories/storage/number/{storageAssetNumber}\n  method: post\n  operationId: /v2/parts/number/{partNumber}/inventories/storage/number/{storageAssetNumber}_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/{partTypeId}/inventories\n  method: get\n  operationId: /v2/parts/{partTypeId}/inventories_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts/number/{partNumber}/inventories\n  method: get\n  operationId: /v2/parts/number/{partNumber}/inventories_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts/{partTypeId}/stock-changes\n  method: get\n  operationId: /v2/parts/{partTypeId}/stock-changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts/number/{partNumber}/stock-changes\n  method: get\n  operationId: /v2/parts/number/{partNumber}/stock-changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts\n  method: get\n  operationId: /v2/parts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts\n  method: post\n  operationId: /v2/parts_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/{id}\n  method: get\n  operationId: /v2/parts/{id}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/parts/{id}\n  method: patch\n  operationId: /v2/parts/{id}_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/parts/number/{partNumber}\n  method: get\n  operationId: /v2/parts/number/{partNumber}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v2/parts/number/{partNumber}\n  method: patch\n  operationId: /v2/parts/number/{partNumber}_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/procedures/templates\n  method: get\n  operationId: /v1/procedures/templates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tickets/categories\n  method: get\n  operationId: /v2/tickets/categories_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tickets\n  method: get\n  operationId: /v2/tickets_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tickets\n  method: post\n  operationId: /v2/tickets_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tickets/{id}/conversations\n  method: get\n  operationId: /v2/tickets/{id}/conversations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tickets/{id}\n  method: get\n  operationId: /v2/tickets/{id}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/tickets/{id}\n  method: patch\n  operationId: /v2/tickets/{id}_patch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/tickets/{id}\n  method: delete\n  operationId: /v2/tickets/{id}_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/groups\n  method: get\n  operationId: /v1/users/groups_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/roles\n  method: get\n  operationId: /v1/users/roles_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: get\n  operationId: /v1/users_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users\n  method: post\n  operationId: /v1/users_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{id}\n  method: get\n  operationId: /v1/users/{id}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{id}\n  method: patch\n  operationId: /v1/users/{id}_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{id}/invite\n  method: post\n  operationId: /v1/users/{id}/invite_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/work-orders\n  method: get\n  operationId: /v2/work-orders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/work-orders\n  method: post\n  operationId: /v2/work-orders_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/work-orders/{id}\n  method: get\n  operationId: /v2/work-orders/{id}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/work-orders/{id}\n  method: patch\n  operationId: /v2/work-orders/{id}_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/work-orders/{id}\n  method: delete\n  operationId: /v2/work-orders/{id}_delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/work-orders/erp/{externalReference}\n  method: get\n  operationId: /v2/work-orders/erp/{externalReference}_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/work-orders/erp/{externalReference}\n  method: patch\n  operationId: /v2/work-orders/erp/{externalReference}_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/work-orders/erp/{externalReference}\n  method: delete\n  operationId: /v2/work-orders/erp/{externalReference}_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/work-orders/{id}/checklist\n  method: post\n  operationId: /v2/work-orders/{id}/checklist_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/work-orders/erp/{externalReference}/checklist\n\
  \  method: post\n  operationId: /v2/work-orders/erp/{externalReference}/checklist_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/work-orders/{id}/times\n  method: get\n  operationId: /v2/work-orders/{id}/times_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/work-orders/{id}/stock-changes\n  method: get\n  operationId: /v2/work-orders/{id}/stock-changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/work-orders/{id}/stock-changes\n  method: post\n  operationId: /v2/work-orders/{id}/stock-changes_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/work-orders/erp/{externalReference}/stock-changes\n  method: get\n  operationId: /v2/work-orders/erp/{externalReference}/stock-changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/work-orders/erp/{externalReference}/stock-changes\n  method: post\n  operationId: /v2/work-orders/erp/{externalReference}/stock-changes_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/work-orders/{id}/procedures\n  method: post\n  operationId: /v2/work-orders/{id}/procedures_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/work-orders/erp/{externalReference}/procedures\n  method: post\n  operationId: /v2/work-orders/erp/{externalReference}/procedures_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-\n\n# --- truncated at 32 KB (37 KB total) ---\n# Full source:\
  \ https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/agentic-access/remberg-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/agentic-access/remberg-agentic-access.yml
summary_line: 115 operations · 65 acting · 10 human-in-the-loop
tags:
- Maintenance
- Asset Management
- CMMS
- EAM
- Field Service
- Work Orders
- Industrial
- SaaS
- Germany
---
