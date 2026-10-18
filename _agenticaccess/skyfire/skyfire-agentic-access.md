---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 14
api_specs:
- filename: skyfire-agents-api-openapi.yml
  format: yaml
  label: Skyfire Agents API
  slug: skyfire-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyfire/refs/heads/main/openapi/skyfire-agents-api-openapi.yml
- filename: skyfire-auth-api-openapi.yml
  format: yaml
  label: Skyfire Auth API
  slug: skyfire-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyfire/refs/heads/main/openapi/skyfire-auth-api-openapi.yml
- filename: skyfire-directory-api-openapi.yml
  format: yaml
  label: Skyfire Directory API
  slug: skyfire-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyfire/refs/heads/main/openapi/skyfire-directory-api-openapi.yml
- filename: skyfire-organizations-api-openapi.yml
  format: yaml
  label: Skyfire Organizations API
  slug: skyfire-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyfire/refs/heads/main/openapi/skyfire-organizations-api-openapi.yml
- filename: skyfire-tokens-api-openapi.yml
  format: yaml
  label: Skyfire Tokens API
  slug: skyfire-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyfire/refs/heads/main/openapi/skyfire-tokens-api-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Skyfire Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/tokens/charge
operation_count: 31
overview: 'Skyfire exposes 31 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 16 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Skyfire
provider_slug: skyfire
slug: skyfire-agentic-access
source_filename: skyfire-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/skyfire-agent-and-token-apis-openapi.yml, openapi/skyfire-service-directory-apis-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 14\n    acting: 17\n  by_consequence:\n    read: 14\n    write: 16\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/agents/balance\n  method: get\n  operationId: get-agents-wallet-balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/seller-services\n  method: get\n  operationId: get-agents-seller-services-all\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/seller-services\n  method: post\n  operationId: create-agents-service-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/seller-services/{sellerServiceId}\n  method: get\n  operationId: get-agents-service\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/seller-services/{sellerServiceId}\n  method: patch\n  operationId: update-agents-service\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/seller-services/{sellerServiceId}/activate\n  method: post\n  operationId: create-agents-service\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/seller-services/{sellerServiceId}/deactivate\n  method: post\n  operationId: deactivate-agents-service\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/source-ips\n  method: get\n  operationId: get_apiv1agentsbalance-1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agents/source-ips\n  method: put\n  operationId: get_apiv1agentssource-ips-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/auth/skyfire-session-token\n  method: post\n  operationId: create-organization-user-session-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/users\n  method: post\n  operationId: create-enterprise-user\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/users\n  method: get\n  operationId: get_api-v1-organizations-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/users/email/{email}\n  method: get\n  operationId: get_api-v1-organizations-users-email\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/users/{userId}\n  method: get\n  operationId: get_api-v1-organizations-users-userid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/users/{userId}/activate\n  method: patch\n  operationId: patch_api-v1-organizations-users-userid-activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/users/{userId}/agents/seller\n  method: post\n  operationId: create-enterprise-user-2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/users/{userId}/agents/{agentId}/api-keys\n  method: post\n  operationId: post_api-v1-organizations-users-userid-agents-agentid-api-keys\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/users/{userId}/agents/{agentId}/api-keys\n  method: get\n  operationId: get_api-v1-organizations-users-userid-agents-agentid-api-keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/users/{userId}/agents/{agentId}/api-keys/{apiKeyId}/activate\n  method: patch\n  operationId: patch_api-v1-organizations-users-userid-agents-agentid-api-keys-apikeyid-activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/users/{userId}/agents/{agentId}/api-keys/{apiKeyId}/deactivate\n  method: patch\n  operationId: patch_api-v1-organizations-users-userid-agents-agentid-api-keys-apikeyid-deactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/users/{userId}/deactivate\n  method: patch\n  operationId: patch_api-v1-organizations-users-userid-deactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/organizations/users/{userId}/personal-data\n\
  \  method: post\n  operationId: create-enterprise-user-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tokens\n  method: post\n  operationId: create-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tokens/charge\n  method: post\n  operationId: charge-token\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tokens/introspect\n  method: post\n  operationId: introspect-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tokens/{tokenId}/charges\n  method: get\n  operationId: get-token-charges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/directory/agents/{agentId}/services\n  method: get\n  operationId: get-services-by-agent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/directory/services\n  method: get\n  operationId:\
  \ get-all-services\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/directory/services/search\n  method: get\n  operationId: get-services-by-tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/directory/services/{serviceId}\n  method: get\n  operationId: get-service\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/directory/tags\n  method: get\n  operationId: get-all-service-tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyfire/refs/heads/main/agentic-access/skyfire-agentic-access.yml
summary_line: 31 operations · 17 acting
tags:
- Company
- AI Agents
- Agentic Payments
- Identity
- Payments
- Authentication
- Stablecoins
- MCP
- Agentic Commerce
- Know Your Agent
---
