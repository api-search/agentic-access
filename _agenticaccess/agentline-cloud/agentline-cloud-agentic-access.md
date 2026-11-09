---
acting_count: 44
action_class_counts:
  acting: 44
  connected: 44
api_specs:
- filename: agentline-cloud-agent-integration-api-openapi.yml
  format: yaml
  label: AgentLine Agent Integration API
  slug: agentline-cloud-agent-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-agent-integration-api-openapi.yml
- filename: agentline-cloud-agent-recharge-api-openapi.yml
  format: yaml
  label: AgentLine Agent Recharge API
  slug: agentline-cloud-agent-recharge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-agent-recharge-api-openapi.yml
- filename: agentline-cloud-agents-api-openapi.yml
  format: yaml
  label: AgentLine Agents API
  slug: agentline-cloud-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-agents-api-openapi.yml
- filename: agentline-cloud-auth-api-openapi.yml
  format: yaml
  label: AgentLine Auth API
  slug: agentline-cloud-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-auth-api-openapi.yml
- filename: agentline-cloud-billing-api-openapi.yml
  format: yaml
  label: AgentLine Billing API
  slug: agentline-cloud-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-billing-api-openapi.yml
- filename: agentline-cloud-calls-api-openapi.yml
  format: yaml
  label: AgentLine Calls API
  slug: agentline-cloud-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-calls-api-openapi.yml
- filename: agentline-cloud-contacts-api-openapi.yml
  format: yaml
  label: AgentLine Contacts API
  slug: agentline-cloud-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-contacts-api-openapi.yml
- filename: agentline-cloud-events-api-openapi.yml
  format: yaml
  label: AgentLine Events API
  slug: agentline-cloud-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-events-api-openapi.yml
- filename: agentline-cloud-feedback-api-openapi.yml
  format: yaml
  label: AgentLine Feedback API
  slug: agentline-cloud-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-feedback-api-openapi.yml
- filename: agentline-cloud-health-api-openapi.yml
  format: yaml
  label: AgentLine Health API
  slug: agentline-cloud-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-health-api-openapi.yml
- filename: agentline-cloud-messages-api-openapi.yml
  format: yaml
  label: AgentLine Messages API
  slug: agentline-cloud-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-messages-api-openapi.yml
- filename: agentline-cloud-numbers-api-openapi.yml
  format: yaml
  label: AgentLine Numbers API
  slug: agentline-cloud-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-numbers-api-openapi.yml
- filename: agentline-cloud-usage-api-openapi.yml
  format: yaml
  label: AgentLine Usage API
  slug: agentline-cloud-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-usage-api-openapi.yml
- filename: agentline-cloud-voice-api-openapi.yml
  format: yaml
  label: AgentLine Voice API
  slug: agentline-cloud-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-voice-api-openapi.yml
- filename: agentline-cloud-webhooks-api-openapi.yml
  format: yaml
  label: AgentLine Webhooks API
  slug: agentline-cloud-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-webhooks-api-openapi.yml
- filename: agentline-cloud-x402-discovery-api-openapi.yml
  format: yaml
  label: AgentLine x402 Discovery API
  slug: agentline-cloud-x402-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-x402-discovery-api-openapi.yml
- filename: agentline-cloud-x402-keyless-api-openapi.yml
  format: yaml
  label: AgentLine x402 Keyless API
  slug: agentline-cloud-x402-keyless-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentline-cloud/openapi/agentline-cloud-x402-keyless-api-openapi.yml
consequence_counts:
  physical: 4
  read: 44
  safety-critical: 2
  write: 38
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Agentline Cloud Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/account/voice
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/auth/keys/{key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/auth/otp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/topup/x402/pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/numbers
operation_count: 88
overview: 'AgentLine exposes 88 API operations that an AI agent could call, of which 44 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 44 read, 38 write, 4 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AgentLine
provider_slug: agentline-cloud
slug: agentline-cloud-agentic-access
source_filename: agentline-cloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentline-cloud-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 88\n  by_action_class:\n    connected: 44\n    acting: 44\n  by_consequence:\n    read: 44\n    write: 38\n    physical: 4\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/agents\n  method: get\n  operationId: list_agents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents\n  method: post\n  operationId: create_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{agent_id}\n  method: get\n  operationId: get_agent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{agent_id}\n  method: patch\n  operationId: update_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{agent_id}\n  method: delete\n  operationId: delete_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{agent_id}/contacts\n  method: post\n  operationId: create_contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{agent_id}/contacts\n  method: get\n  operationId: list_contacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{agent_id}/contacts/{contact_id}\n  method: get\n  operationId: get_contact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{agent_id}/contacts/{contact_id}\n  method: patch\n  operationId: update_contact\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{agent_id}/contacts/{contact_id}\n  method: delete\n  operationId: delete_contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/numbers\n  method: get\n  operationId: list_phone_numbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/numbers\n  method: post\n  operationId: buy_phone_number\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/numbers/{number_id}\n  method: get\n  operationId: get_phone_number\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/numbers/attach\n  method: post\n  operationId: attach_existing_number\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/numbers/{number_id}/reassign\n  method: patch\n  operationId: reassign_number\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/numbers/{number_id}/release\n  method: post\n  operationId: release_phone_number\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages\n  method: post\n  operationId: send_sms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages\n\
  \  method: get\n  operationId: list_messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages/conversations\n  method: get\n  operationId: list_conversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calls\n  method: post\n  operationId: make_outbound_call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/calls\n  method: get\n  operationId: list_calls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calls/{call_id}\n\
  \  method: get\n  operationId: get_call_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calls/{call_id}/transcript\n  method: get\n  operationId: get_call_transcript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calls/{call_id}/hangup\n  method: post\n  operationId: hangup_call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/calls/{call_id}/context\n  method: post\n  operationId: push_call_context\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: get_usage_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage/balance\n  method: get\n  operationId: get_usage_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage/transactions\n  method: get\n  operationId: get_billing_transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: get\n  operationId: poll_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/events/peek\n  method: get\n  operationId: peek_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/balance\n  method: get\n  operationId: get_account_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/expenditure\n  method: get\n  operationId: get_expenditure_breakdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/expenditure/calls\n  method: get\n  operationId: get_call_charges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/expenditure/numbers\n  method: get\n  operationId:\
  \ get_number_charges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/verify/{call_id}\n  method: get\n  operationId: verify_call_billing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/summary\n  method: get\n  operationId: get_spending_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/voices\n  method: get\n  operationId: list_available_voices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/voice\n  method: get\n  operationId: get_account_voice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/voice\n  method: delete\n  operationId: reset_account_voice\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/account/voice\n  method: patch\n  operationId: set_account_voice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/feedback\n  method: post\n  operationId: submit_feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/feedback\n  method: get\n  operationId: list_feedback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/otp\n  method: post\n  operationId: auth_send_otp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/verify\n  method: post\n  operationId: auth_verify_otp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/keys\n  method: get\n  operationId: auth_list_api_keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/keys\n  method: post\n  operationId: auth_create_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/keys/{key_id}\n  method: delete\n  operationId: auth_revoke_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n  \
  \    proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/auth/agentid/start\n  method: post\n  operationId: auth_agentid_start\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/agentid/callback\n  method: get\n  operationId: auth_agentid_callback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/agentid/poll\n  method: post\n  operationId: auth_agentid_poll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: get_webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: set_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks\n  method: delete\n  operationId: delete_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/test\n  method: post\n\
  \  operationId: test_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/account\n  method: get\n  operationId: get_account_notification_webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/account\n  method: post\n  operationId: set_account_notification_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/account\n  method: delete\n  operationId: delete_account_notification_webhook\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/account/test\n  method: post\n  operationId: test_account_notification_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/account/deliveries\n  method: get\n  operationId: account_notification_delivery_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/api-key\n  method: get\n  operationId: get_api_key_notification_webhook\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/api-key\n  method: post\n  operationId: set_api_key_notification_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/api-key\n  method: delete\n  operationId: delete_api_key_notification_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/api-key/numbers\n  method: get\n  operationId: list_api_key_notification_numbers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/api-key/numbers/{number_id}\n  method: put\n  operationId: assign_legacy_number_to_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/api-key/test\n  method: post\n  operationId: test_api_key_notification_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/api-key/deliveries\n  method: get\n  operationId: api_key_notification_delivery_status\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/topup/x402/pay\n  method: post\n  operationId: x402_payment_discovery_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/numbers/buy\n  method: post\n  operationId: x402_keyless_buy_number\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/numbers\n  method: get\n  operationId: x402_keyless_list_numbers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/numbers\n  method: post\n  operationId: x402_keyless_list_numbers_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/calls\n  method: post\n  operationId: x402_keyless_make_call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/calls/{call_id}/transcript\n  method: get\n  operationId: x402_keyless_call_transcript\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/calls/{call_id}/transcript\n  method: post\n  operationId: x402_keyless_call_transcript_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/numbers/renew\n  method: post\n  operationId: x402_keyless_renew_number\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/agents\n  method: get\n  operationId: x402_keyless_get_agent\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/agents\n  method: patch\n  operationId: x402_keyless_update_agent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/agents\n  method: post\n  operationId: x402_keyless_update_agent_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/webhooks\n  method: get\n  operationId: x402_keyless_get_webhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v1/x402/webhooks\n  method: post\n  operationId: x402_keyless_set_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/webhooks/test\n  method: post\n  operationId: x402_keyless_test_webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/x402/events\n  method: get\n  operationId: x402_keyless_poll_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/x402/events\n  method: post\n  operationId: x402_keyless_poll_events_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/x402\n  method: get\n  operationId: x402_keyless_discovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-payments.json\n  method: get\n  operationId: agent_payment_integration_discovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agentline.json\n  method: get\n  operationId: agentline_integration_discovery\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: health_check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/x402.json\n  method: get\n  operationId: x402_discovery_manifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agentline-cloud/agentic-access/agentline-cloud-agentic-access.yml
summary_line: 88 operations · 44 acting · 2 human-in-the-loop
tags:
- Artificial Intelligence
- Telephony
- Voice
- SMS
- Agents
---
