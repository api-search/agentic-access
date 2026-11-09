---
acting_count: 63
action_class_counts:
  acting: 63
  connected: 41
api_specs:
- filename: chatrail-dev-ai-api-openapi.yml
  format: yaml
  label: chatrail-dev AI API
  slug: chatrail-dev-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-ai-api-openapi.yml
- filename: chatrail-dev-auth-api-openapi.yml
  format: yaml
  label: chatrail-dev Auth API
  slug: chatrail-dev-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-auth-api-openapi.yml
- filename: chatrail-dev-billing-api-openapi.yml
  format: yaml
  label: chatrail-dev Billing API
  slug: chatrail-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-billing-api-openapi.yml
- filename: chatrail-dev-connections-api-openapi.yml
  format: yaml
  label: chatrail-dev Connections API
  slug: chatrail-dev-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-connections-api-openapi.yml
- filename: chatrail-dev-groups-api-openapi.yml
  format: yaml
  label: chatrail-dev Groups API
  slug: chatrail-dev-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-groups-api-openapi.yml
- filename: chatrail-dev-internal-api-openapi.yml
  format: yaml
  label: chatrail-dev Internal API
  slug: chatrail-dev-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-internal-api-openapi.yml
- filename: chatrail-dev-mcp-api-openapi.yml
  format: yaml
  label: chatrail-dev MCP API
  slug: chatrail-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-mcp-api-openapi.yml
- filename: chatrail-dev-messages-api-openapi.yml
  format: yaml
  label: chatrail-dev Messages API
  slug: chatrail-dev-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-messages-api-openapi.yml
- filename: chatrail-dev-operational-api-openapi.yml
  format: yaml
  label: chatrail-dev Operational API
  slug: chatrail-dev-operational-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-operational-api-openapi.yml
- filename: chatrail-dev-opt-outs-api-openapi.yml
  format: yaml
  label: chatrail-dev Opt Outs API
  slug: chatrail-dev-opt-outs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-opt-outs-api-openapi.yml
- filename: chatrail-dev-schedules-api-openapi.yml
  format: yaml
  label: chatrail-dev Schedules API
  slug: chatrail-dev-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-schedules-api-openapi.yml
- filename: chatrail-dev-team-api-openapi.yml
  format: yaml
  label: chatrail-dev Team API
  slug: chatrail-dev-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-team-api-openapi.yml
- filename: chatrail-dev-webhooks-api-openapi.yml
  format: yaml
  label: chatrail-dev Webhooks API
  slug: chatrail-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-webhooks-api-openapi.yml
- filename: chatrail-dev-workspace-api-openapi.yml
  format: yaml
  label: chatrail-dev Workspace API
  slug: chatrail-dev-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatrail-dev/openapi/chatrail-dev-workspace-api-openapi.yml
consequence_counts:
  physical: 6
  read: 41
  safety-critical: 5
  write: 52
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Chatrail Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/api-keys/{id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/connections/{connection}/groups/{group}/invite/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/members/invitations/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/messages/{id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/profile/sessions/revoke-others
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/ai/runs/{id}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/crypto/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/nowpayments/webhook
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/members/invitations/{id}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/messages/text
operation_count: 104
overview: 'chatrail-dev exposes 104 API operations that an AI agent could call, of which 63 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 41 read, 52 write, 6 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: chatrail-dev
provider_slug: chatrail-dev
slug: chatrail-dev-agentic-access
source_filename: chatrail-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/chatrail-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 104\n  by_action_class:\n    acting: 63\n    connected: 41\n  by_consequence:\n    physical: 6\n    read: 41\n    write: 52\n    safety-critical: 5\n  human_in_the_loop_required: 5\noperations:\n- path: /v1/messages/text\n  method: post\n  operationId: post_v1_messages_text\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - messages:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/messages\n  method: get\n  operationId: get_v1_messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - messages:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/{id}\n  method: get\n  operationId: get_v1_messages__id_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - messages:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/{id}\n  method: patch\n  operationId: patch_v1_messages__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - messages:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/cancel\n  method: post\n  operationId: post_v1_messages__id__cancel\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - messages:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/reactions\n  method: post\n  operationId: post_v1_messages__id__reactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - messages:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/read\n  method: post\n  operationId: post_v1_messages__id__read\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - messages:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/{connection}\n  method: patch\n  operationId: patch_v1_connections__connection_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - connections:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/{connection}\n  method: get\n  operationId: get_v1_connections__connection_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - connections:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{connection}\n  method: delete\n  operationId: delete_v1_connections__connection_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - connections:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/{connection}/groups\n  method: post\n  operationId: post_v1_connections__connection__groups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - connections:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/{connection}/groups\n  method: get\n  operationId: get_v1_connections__connection__groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - connections:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{connection}/groups/{group}\n\
  \  method: get\n  operationId: get_v1_connections__connection__groups__group_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - connections:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{connection}/groups/{group}\n  method: patch\n  operationId: patch_v1_connections__connection__groups__group_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - connections:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/{connection}/groups/{group}/participants\n  method: post\n  operationId: post_v1_connections__connection__groups__group__participants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - connections:write\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/{connection}/groups/{group}/invite\n  method: get\n  operationId: get_v1_connections__connection__groups__group__invite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - connections:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{connection}/groups/{group}/invite/revoke\n  method: post\n  operationId: post_v1_connections__connection__groups__group__invite_revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - connections:write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /v1/connections/{connection}/groups/{group}/leave\n  method: post\n  operationId: post_v1_connections__connection__groups__group__leave\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - connections:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/{connection}/presence\n  method: post\n  operationId: post_v1_connections__connection__presence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - messages:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/revoke\n  method: post\n  operationId: post_v1_messages__id__revoke\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - messages:write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/messages/{id}/reschedule\n  method: post\n  operationId: post_v1_messages__id__reschedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - messages:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/export\n  method: get\n  operationId: get_v1_messages_export\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - messages:read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/numbers/check\n  method: get\n  operationId: get_v1_numbers_check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - messages:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/numbers/check\n  method: post\n  operationId: post_v1_numbers_check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - messages:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections\n  method: post\n  operationId: post_v1_connections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - connections:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections\n  method: get\n  operationId: get_v1_connections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - connections:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{connection}/pair\n  method: post\n  operationId: post_v1_connections__connection__pair\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - connections:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/{connection}/qr/{grantId}\n  method: get\n  operationId: get_v1_connections__connection__qr__grantId_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - connections:write\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{connection}/suspend\n  method: post\n  operationId: post_v1_connections__connection__suspend\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - connections:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connections/{connection}/resume\n  method: post\n  operationId: post_v1_connections__connection__resume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - connections:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schedules\n  method: post\n  operationId: post_v1_schedules\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - schedules:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schedules\n  method: get\n  operationId: get_v1_schedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - schedules:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/schedules/{id}\n  method: get\n  operationId: get_v1_schedules__id_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - schedules:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/schedules/{id}/pause\n  method: post\n  operationId: post_v1_schedules__id__pause\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - schedules:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schedules/{id}/resume\n  method: post\n  operationId: post_v1_schedules__id__resume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - schedules:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schedules/{id}/cancel\n  method: post\n  operationId: post_v1_schedules__id__cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - schedules:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/webhook-endpoints\n  method: post\n  operationId: post_v1_webhook-endpoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-endpoints\n  method: get\n  operationId: get_v1_webhook-endpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook-endpoints/{id}\n  method: delete\n  operationId: delete_v1_webhook-endpoints__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-endpoints/{id}/enable\n  method: post\n  operationId: post_v1_webhook-endpoints__id__enable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/opt-outs\n  method: get\n  operationId: get_v1_opt-outs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - messages:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/opt-outs\n  method: post\n  operationId: post_v1_opt-outs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - messages:write\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/opt-outs/{phone}\n  method: delete\n  operationId: delete_v1_opt-outs__phone_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - messages:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/credentials\n  method: post\n  operationId: post_v1_ai_credentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ai:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/credentials\n  method: get\n  operationId: get_v1_ai_credentials\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ai:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai/credentials/{id}\n  method: delete\n  operationId: delete_v1_ai_credentials__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ai:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/credentials/{id}/test\n  method: post\n  operationId: post_v1_ai_credentials__id__test\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ai:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/policies/{connection}\n\
  \  method: put\n  operationId: put_v1_ai_policies__connection_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ai:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/policies/{connection}\n  method: get\n  operationId: get_v1_ai_policies__connection_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ai:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai/runs\n  method: get\n  operationId: get_v1_ai_runs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ai:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai/runs/{id}/send\n  method: post\n  operationId: post_v1_ai_runs__id__send\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    scope:\n    - ai:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/runs/{id}/dismiss\n  method: post\n  operationId: post_v1_ai_runs__id__dismiss\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ai:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{id}/media\n  method: get\n  operationId: get_v1_messages__id__media\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - messages:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/messages/{id}/correlation\n  method: post\n  operationId: post_v1_messages__id__correlation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - messages:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/quality\n  method: get\n  operationId: get_v1_ai_quality\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ai:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/whoami\n  method: get\n  operationId: get_v1_whoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace\n  method: get\n  operationId: get_v1_workspace\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workspace\n  method: patch\n  operationId: patch_v1_workspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing\n  method: get\n  operationId: get_v1_billing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/regional-price\n  method: get\n  operationId: get_v1_billing_regional-price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/plans\n  method: get\n  operationId: get_v1_billing_plans\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/checkout\n  method: post\n  operationId: post_v1_billing_checkout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/plan-change-check\n  method: post\n  operationId: post_v1_billing_plan-change-check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/portal\n  method: post\n  operationId: post_v1_billing_portal\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/creem/webhook\n  method: post\n  operationId: post_v1_billing_creem_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/crypto\n  method: get\n  operationId: get_v1_billing_crypto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/crypto/checkout\n  method: post\n  operationId: post_v1_billing_crypto_checkout\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/nowpayments/webhook\n  method: post\n  operationId: post_v1_billing_nowpayments_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: get_v1_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - usage:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys\n  method: post\n\
  \  operationId: post_v1_api-keys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/api-keys\n  method: get\n  operationId: get_v1_api-keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys/{id}/revoke\n  method: post\n  operationId: post_v1_api-keys__id__revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/api-keys/{id}/rotate\n  method: post\n  operationId:\
  \ post_v1_api-keys__id__rotate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/members\n  method: get\n  operationId: get_v1_members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/members/invitations\n  method: post\n  operationId: post_v1_members_invitations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/members/invitations/{id}\n  method: delete\n  operationId: delete_v1_members_invitations__id_\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/members/invitations/{id}/resend\n  method: post\n  operationId: post_v1_members_invitations__id__resend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/members/accept\n  method: post\n  operationId: post_v1_members_accept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/members/{id}\n  method: patch\n  operationId: patch_v1_members__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/members/{id}\n  method: delete\n  operationId: delete_v1_members__id_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profile\n  method: get\n  operationId: get_v1_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profile\n  method: patch\n  operationId: patch_v1_profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profile/sessions\n  method: get\n  operationId: get_v1_profile_sessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profile/sessions/revoke-others\n  method: post\n  operationId: post_v1_profile_sessions_revoke-others\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /v1/profile/sessions/{sessionId}\n  method: delete\n  operationId: delete_v1_profile_sessions__sessionId_\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profile/notification-preferences\n  method: get\n  operationId: get_v1_profile_notification-preferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profile/notification-preferences\n  method: patch\n  operationId: patch_v1_profile_notification-preferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profile/heard-from\n  method: put\n  operationId: put_v1_profile_heard-from\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/request-code\n  method: post\n  operationId: post_v1_auth_request-code\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/verify\n  method: post\n  operationId: post_v1_auth_verify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/session\n  method: get\n  operationId: get_v1_auth_session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/logout\n  method: post\n  operationId: post_v1_auth_logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/providers\n  method: get\n  operationId: get_v1_auth_providers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/auth/oauth/{provider}/start\n  method: get\n  operationId: get_v1_auth_oauth__provider__start\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/oauth/{provider}/callback\n  method: get\n  operationId: get_v1_auth_oauth__provider__callback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mcp\n  method: post\n  operationId: post_v1_mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - mcp:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (33 KB total) ---\n# Full source: https://artifacts.apis.io/chatrail-dev/agentic-access/chatrail-dev-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/chatrail-dev/agentic-access/chatrail-dev-agentic-access.yml
summary_line: 104 operations · 63 acting · 5 human-in-the-loop
tags:
- WhatsApp
- Messaging
- Artificial Intelligence
- Developers
---
