---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 15
api_specs:
- filename: agentspace-com-br-account-api-openapi.yml
  format: yaml
  label: AgentSpace Account API
  slug: agentspace-com-br-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentspace-com-br/openapi/agentspace-com-br-account-api-openapi.yml
- filename: agentspace-com-br-agent-api-openapi.yml
  format: yaml
  label: AgentSpace Agent API
  slug: agentspace-com-br-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentspace-com-br/openapi/agentspace-com-br-agent-api-openapi.yml
- filename: agentspace-com-br-billing-api-openapi.yml
  format: yaml
  label: AgentSpace Billing API
  slug: agentspace-com-br-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentspace-com-br/openapi/agentspace-com-br-billing-api-openapi.yml
- filename: agentspace-com-br-review-api-openapi.yml
  format: yaml
  label: AgentSpace Review API
  slug: agentspace-com-br-review-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentspace-com-br/openapi/agentspace-com-br-review-api-openapi.yml
consequence_counts:
  physical: 4
  read: 15
  safety-critical: 2
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Agentspace Com Br Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/account/keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/review/share/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/connect
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/deployments/{name}
operation_count: 43
overview: 'AgentSpace exposes 43 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 22 write, 4 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AgentSpace
provider_slug: agentspace-com-br
slug: agentspace-com-br-agentic-access
source_filename: agentspace-com-br-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentspace-com-br-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 15\n    acting: 28\n  by_consequence:\n    read: 15\n    write: 22\n    physical: 4\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /api/v1/hello\n  method: get\n  operationId: hello_api_v1_hello_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/whoami\n  method: get\n  operationId: whoami_api_v1_whoami_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/files\n  method: get\n  operationId: list_files_api_v1_files_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/files\n  method: put\n  operationId: write_file_api_v1_files_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/files\n  method: delete\n  operationId: delete_file_api_v1_files_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/files/content\n\
  \  method: get\n  operationId: read_file_api_v1_files_content_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/files/raw\n  method: get\n  operationId: read_file_raw_api_v1_files_raw_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/files/upload\n  method: post\n  operationId: upload_file_api_v1_files_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/files/move\n  method: post\n  operationId: move_file_api_v1_files_move_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/exec\n  method: post\n  operationId: exec_code_api_v1_exec_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tools/{name}\n  method: post\n  operationId: call_tool_api_v1_tools__name__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/deployments\n  method: get\n  operationId: list_deployments_api_v1_deployments_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/deployments\n  method: post\n  operationId: create_deployment_api_v1_deployments_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/deployments/{name}/logs\n  method: get\n  operationId: deployment_logs_api_v1_deployments__name__logs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/deployments/{name}\n  method: delete\n  operationId: delete_deployment_api_v1_deployments__name__delete\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/register\n  method: post\n  operationId: register_api_v1_account_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/login\n  method: post\n  operationId: login_api_v1_account_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/account/logout\n  method: post\n  operationId: logout_api_v1_account_logout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/keys\n  method: get\n  operationId: list_keys_api_v1_account_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/keys\n  method: post\n  operationId: create_key_api_v1_account_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /api/v1/account/keys/{key_id}\n  method: delete\n  operationId: revoke_key_api_v1_account_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/account/connections\n  method: get\n  operationId: list_connections_api_v1_account_connections_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/connections/{grant_id}\n  method: delete\n  operationId: disconnect_api_v1_account_connections__grant_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account\n  method: delete\n  operationId: delete_account_api_v1_account_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/domain\n  method: get\n  operationId: custom_domain_api_v1_account_domain_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/domain\n  method: put\n  operationId: set_custom_domain_api_v1_account_domain_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/domain\n  method: delete\n  operationId: remove_custom_domain_api_v1_account_domain_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account/domain/verify\n  method: post\n  operationId: verify_custom_domain_api_v1_account_domain_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/billing/plans\n  method: get\n  operationId:\
  \ list_plans_api_v1_billing_plans_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/subscription\n  method: get\n  operationId: get_subscription_api_v1_billing_subscription_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/billing/checkout\n  method: post\n  operationId: checkout_api_v1_billing_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/billing/portal\n  method: post\n  operationId: portal_api_v1_billing_portal_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/connect\n  method: post\n  operationId: start_api_v1_connect_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/connect\n  method: get\n  operationId: start_by_link_api_v1_connect_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/connect/poll\n  method: post\n  operationId: poll_api_v1_connect_poll_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/connect/poll\n  method: get\n  operationId: poll_by_link_api_v1_connect_poll_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/review\n  method: get\n  operationId: status_api_v1_review_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/review/settings\n  method: post\n  operationId: settings_api_v1_review_settings_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/review/publish\n  method: post\n  operationId: publish_api_v1_review_publish_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/review/discard\n  method: post\n  operationId: discard_api_v1_review_discard_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/review/rollback\n  method: post\n  operationId: rollback_api_v1_review_rollback_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/review/share\n  method: post\n  operationId: share_api_v1_review_share_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/review/share/revoke\n  method: post\n  operationId: revoke_api_v1_review_share_revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentspace-com-br/agentic-access/agentspace-com-br-agentic-access.yml
summary_line: 43 operations · 28 acting · 2 human-in-the-loop
tags:
- Artificial Intelligence
- Agents
- Workspace
- Sandbox
- Hosting
---
