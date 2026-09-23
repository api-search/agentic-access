---
acting_count: 84
action_class_counts:
  acting: 84
  connected: 67
api_specs:
- filename: algovoi-co-uk-pay-openapi.yml
  format: yaml
  label: AlgoVoi Pay (Payable Core) API
  slug: algovoi-pay-payable-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-pay-openapi.yml
- filename: algovoi-co-uk-gateway-openapi.yml
  format: yaml
  label: AlgoVoi Gateway API
  slug: algovoi-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-gateway-openapi.yml
- filename: algovoi-co-uk-clinic-openapi.yml
  format: yaml
  label: AlgoVoi RFC 9421 Clinic (Verifiable-Comms Agent) API
  slug: algovoi-rfc9421-clinic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-clinic-openapi.yml
- filename: algovoi-co-uk-agent-trust-bench-openapi.yml
  format: yaml
  label: AlgoVoi Agent Trust Bench API
  slug: algovoi-agent-trust-bench-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-agent-trust-bench-openapi.yml
- filename: algovoi-co-uk-audit-verifier-openapi.yml
  format: yaml
  label: AlgoVoi Audit Verifier API
  slug: algovoi-audit-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-audit-verifier-openapi.yml
- filename: algovoi-co-uk-gateway-openapi.yml
  format: yaml
  label: AlgoVoi MCP Server
  slug: algovoi-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/openapi/algovoi-co-uk-gateway-openapi.yml
consequence_counts:
  physical: 20
  read: 67
  safety-critical: 1
  write: 63
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Algovoi Co Uk Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/recurring/authorities/{authority_id}/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ap2/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ap2/pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/{token}/abandon
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/{token}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/{token}/submit-sponsored
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/{token}/submit-txn
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/{token}/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/{token}/xchain/bridge-send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/{token}/xchain/optin-submit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/{token}/xchain/prepare
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/{token}/xchain/prepare-optin
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/{token}/xchain/source-tx-recorded
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/{token}/xchain/submit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /message:send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /suite-store/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /suite-store/mesh-fed/provision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /suite-store/order/{token}/activate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payment-links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/verify
operation_count: 151
overview: 'AlgoVoi exposes 151 API operations that an AI agent could call, of which 84 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 67 read, 63 write, 20 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AlgoVoi
provider_slug: algovoi-co-uk
slug: algovoi-co-uk-agentic-access
source_filename: algovoi-co-uk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/algovoi-co-uk-agent-trust-bench-openapi.yml, openapi/algovoi-co-uk-audit-verifier-openapi.yml,\n  openapi/algovoi-co-uk-clinic-openapi.yml, openapi/algovoi-co-uk-gateway-openapi.yml, openapi/algovoi-co-uk-pay-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 151\n  by_action_class:\n    connected: 67\n    acting: 84\n  by_consequence:\n    read: 67\n    write: 63\n    physical: 20\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /{profile_id}\n  method: get\n  operationId: get_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery/resources\n\
  \  method: get\n  operationId: list_resources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/x402.json\n  method: get\n  operationId: well_known_x402\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /freebie\n  method: get\n  operationId: get_freebie\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats.json\n  method: get\n  operationId: get_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: openapi_schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: root__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify\n  method: post\n  operationId: verify_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /.well-known/agent-card.json\n  method: get\n  operationId: agent_card__well_known_agent_card_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent.json\n  method: get\n  operationId: agent_card_legacy__well_known_agent_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/rfc9421\n  method: post\n  operationId: verify_verify_rfc9421_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/rfc9421/explain\n  method: post\n  operationId: explain_verify_rfc9421_explain_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/rfc9421/sign\n  method: post\n  operationId: sign_demo_verify_rfc9421_sign_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a\n  method: get\n  operationId: a2a_hint_a2a_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /a2a\n  method: post\n  operationId: a2a_a2a_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: landing__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/token\n  method: post\n  operationId: exchange_atb_cert_auth_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/token/status\n  method: get\n  operationId: session_status_auth_token_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verify\n  method: post\n  operationId: mpp_verify_v1_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ap2/verify\n  method: post\n  operationId: ap2_verify_v1_ap2_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payouts\n  method: post\n  operationId: create_payout_v1_payouts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpp/challenge\n  method: post\n  operationId: mpp_challenge_mpp_challenge_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpp/probe\n  method: get\n  operationId: mpp_probe_mpp_probe_delete\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mpp/probe\n  method: put\n  operationId: mpp_probe_mpp_probe_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpp/probe\n  method: post\n  operationId: mpp_probe_mpp_probe_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpp/probe\n  method: delete\n  operationId: mpp_probe_mpp_probe_delete\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpp/probe\n  method: options\n  operationId: mpp_probe_mpp_probe_delete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mpp/probe\n  method: head\n  operationId: mpp_probe_mpp_probe_delete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mpp/probe\n  method: patch\n  operationId: mpp_probe_mpp_probe_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /mpp/{resource_id}\n  method: get\n  operationId: mpp_resource_mpp__resource_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mpp/sub/{resource_id}\n  method: post\n  operationId: mpp_subscription_resource_mpp_sub__resource_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mpp/sub/{resource_id}\n  method: get\n  operationId: mpp_subscription_resource_mpp_sub__resource_id__post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ap2/intent\n  method: post\n  operationId: submit_intent_ap2_intent_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap2/cart\n  method: post\n  operationId: submit_cart_ap2_cart_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap2/pay\n  method: post\n  operationId: initiate_payment_ap2_pay_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /ap2/confirm\n  method: post\n  operationId: confirm_payment_ap2_confirm_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ap2/status/{cart_id}\n  method: get\n  operationId: get_status_ap2_status__cart_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ap2/extensions\n  method: get\n  operationId: list_extensions_ap2_extensions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/scoped-authorization-receipts/v1\n  method: get\n\
  \  operationId: _scoped_auth_receipts_profile_ext_scoped_authorization_receipts_v1_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ext/scoped-authorization-receipts/v1\n  method: head\n  operationId: _scoped_auth_receipts_profile_ext_scoped_authorization_receipts_v1_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /extendedAgentCard\n  method: get\n  operationId: extended_agent_card_extendedAgentCard_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /message:send\n  method: post\n  operationId: send_message_message_send_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /message:stream\n  method: post\n  operationId: message_stream_message_stream_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/pushNotificationConfigs/{config_id}\n  method: get\n  operationId: push_notification_config_tasks__task_id__pushNotificationConfigs__config_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/pushNotificationConfigs/{config_id}\n  method: delete\n  operationId: push_notification_config_tasks__task_id__pushNotificationConfigs__config_id__get\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/pushNotificationConfigs\n  method: post\n  operationId: push_notification_config_tasks__task_id__pushNotificationConfigs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}/pushNotificationConfigs\n  method: get\n  operationId: push_notification_config_tasks__task_id__pushNotificationConfigs_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /tasks/{task_id}\n  method: get\n  operationId: get_task_tasks__task_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}:cancel\n  method: post\n  operationId: cancel_task_tasks__task_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks\n  method: get\n  operationId: list_tasks_tasks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a/jsonrpc\n  method: post\n  operationId: a2a_jsonrpc_a2a_jsonrpc_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a/gibberlink\n  method: post\n  operationId: a2a_gibberlink_a2a_gibberlink_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payment-links\n  method: post\n  operationId: create_dynamic_payment_link_v1_payment_links_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/customers\n  method: post\n  operationId: create_customer_endpoint_v1_customers_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers\n  method: get\n  operationId: list_customers_endpoint_v1_customers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subscriptions\n  method: post\n  operationId: create_subscription_endpoint_v1_subscriptions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/subscriptions\n  method: get\n  operationId: list_subscriptions_endpoint_v1_subscriptions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subscriptions/{subscription_id}\n  method: get\n  operationId: get_subscription_endpoint_v1_subscriptions__subscription_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subscriptions/{subscription_id}\n  method: patch\n  operationId: update_subscription_endpoint_v1_subscriptions__subscription_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subscriptions/{subscription_id}/cancel\n\
  \  method: post\n  operationId: cancel_subscription_endpoint_v1_subscriptions__subscription_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subscriptions/{subscription_id}/pause\n  method: post\n  operationId: pause_subscription_endpoint_v1_subscriptions__subscription_id__pause_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subscriptions/{subscription_id}/resume\n  method: post\n  operationId: resume_subscription_endpoint_v1_subscriptions__subscription_id__resume_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subscriptions/{subscription_id}/invoices\n  method: get\n  operationId: list_subscription_invoices_endpoint_v1_subscriptions__subscription_id__invoices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscription/{cancel_secret}/cancel\n  method: get\n  operationId: public_cancel_page_subscription__cancel_secret__cancel_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscription/{cancel_secret}/cancel\n  method: post\n  operationId: public_cancel_commit_subscription__cancel_secret__cancel_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recurr/auth/challenge\n  method: post\n  operationId: challenge_endpoint_v1_recurr_auth_challenge_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recurr/auth/verify\n  method: post\n  operationId: verify_endpoint_v1_recurr_auth_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v1/recurr/me/subscriptions\n  method: get\n  operationId: my_subscriptions_v1_recurr_me_subscriptions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recurr/me/subscriptions/{subscription_id}\n  method: get\n  operationId: my_subscription_detail_v1_recurr_me_subscriptions__subscription_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recurr/me/subscriptions/{subscription_id}/cancel\n  method: post\n  operationId: my_subscription_cancel_v1_recurr_me_subscriptions__subscription_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v1/recurr/me/invoices\n  method: get\n  operationId: my_invoices_v1_recurr_me_invoices_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurr/portal\n  method: get\n  operationId: portal_page_recurr_portal_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurr/cancel/{cancel_secret}\n  method: get\n  operationId: public_cancel_page_recurr_cancel__cancel_secret__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurr/cancel/{cancel_secret}\n  method: post\n  operationId: public_cancel_commit_recurr_cancel__cancel_secret__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recurring/authorities\n  method: post\n  operationId: create_authority_endpoint_v1_recurring_authorities_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recurring/authorities\n  method: get\n  operationId: list_authorities_endpoint_v1_recurring_authorities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recurring/authorities/{authority_id}\n  method: get\n  operationId: get_authority_endpoint_v1_recurring_authorities__authority_id__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recurring/authorities/{authority_id}/confirm\n  method: post\n  operationId: confirm_authority_endpoint_v1_recurring_authorities__authority_id__confirm_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recurring/authorities/{authority_id}/revoke\n  method: post\n  operationId: revoke_authority_endpoint_v1_recurring_authorities__authority_id__revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/recurring/authorities/{authority_id}/pause\n  method: post\n  operationId: pause_authority_endpoint_v1_recurring_authorities__authority_id__pause_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recurring/authorities/{authority_id}/resume\n  method: post\n  operationId: resume_authority_endpoint_v1_recurring_authorities__authority_id__resume_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recurring/pulls\n  method: post\n\
  \  operationId: manual_pull_endpoint_v1_recurring_pulls_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recurring/auth/{token}\n  method: get\n  operationId: resolve_token_v1_recurring_auth__token__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recurring/auth/{token}/confirm\n  method: post\n  operationId: confirm_token_v1_recurring_auth__token__confirm_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/recurring/contracts/algorand/spending_cap_vault_v1\n  method: get\n  operationId: get_algorand_spending_cap_vault_v1_v1_recurring_contracts_algorand_spending_cap_vault_v1_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /protected/{resource_id}\n  method: get\n  operationId: get_protected_resource_protected__resource_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/{resource_id}\n  method: get\n  operationId: get_resource_resources__resource_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/challenge\n  method: post\n  operationId: challenge_x402_challenge_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /x402/verify\n  method: post\n  operationId: verify_x402_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/{token}/verify\n  method: post\n  operationId: verify_checkout_checkout__token__verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /checkout/{token}/qr\n  method: get\n  operationId: checkout_qr_checkout__token__qr_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout/{token}/build-txn\n  method: get\n  operationId: checkout_build_txn_checkout__token__build_txn_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout/{token}/submit-txn\n  method: post\n  operationId: checkout_submit_txn_checkout__token__submit_txn_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/{token}/detect\n  method:\
  \ get\n  operationId: detect_payment_checkout__token__detect_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkout/{token}/submit-sponsored\n  method: post\n  operationId: submit_sponsored_checkout__token__submit_sponsored_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/{token}/abandon\n  method: post\n  operationId: abandon_checkout_checkout__token__abandon_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/{token}/cancel\n  method: post\n  operationId: cancel_checkout_checkout__token__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/{token}/xchain/bridge-info\n  method: get\n  operationId: xchain_bridge_info_checkout__token__xchain_bridge_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (48 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/agentic-access/algovoi-co-uk-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algovoi-co-uk/refs/heads/main/agentic-access/algovoi-co-uk-agentic-access.yml
summary_line: 151 operations · 84 acting · 1 human-in-the-loop
tags:
- Payments
- Agentic Commerce
- x402
- A2A
- MCP
- Stablecoins
- Cryptocurrency
- Blockchain
- Compliance
- Digital Signature
- Post-Quantum Cryptography
- Verification
- Fintech
- agent-native
- Algorand
- United Kingdom
---
