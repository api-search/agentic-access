---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 45
api_specs:
- filename: quant-api-keys-api-openapi.yml
  format: yaml
  label: Quant Network API Keys API
  slug: quant-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-api-keys-api-openapi.yml
- filename: quant-contracts-api-openapi.yml
  format: yaml
  label: Quant Network Contracts API
  slug: quant-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-contracts-api-openapi.yml
- filename: quant-deposits-api-openapi.yml
  format: yaml
  label: Quant Network Deposits API
  slug: quant-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-deposits-api-openapi.yml
- filename: quant-flow-query-api-openapi.yml
  format: yaml
  label: Quant Network Flow Query API
  slug: quant-flow-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-flow-query-api-openapi.yml
- filename: quant-flow-registry-api-openapi.yml
  format: yaml
  label: Quant Network Flow Registry API
  slug: quant-flow-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-flow-registry-api-openapi.yml
- filename: quant-flow-sessions-api-openapi.yml
  format: yaml
  label: Quant Network Flow Sessions API
  slug: quant-flow-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-flow-sessions-api-openapi.yml
- filename: quant-flow-webhooks-api-openapi.yml
  format: yaml
  label: Quant Network Flow Webhooks API
  slug: quant-flow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-flow-webhooks-api-openapi.yml
- filename: quant-health-api-openapi.yml
  format: yaml
  label: Quant Network Health API
  slug: quant-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-health-api-openapi.yml
- filename: quant-networks-api-openapi.yml
  format: yaml
  label: Quant Network Networks API
  slug: quant-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-networks-api-openapi.yml
- filename: quant-nodes-api-openapi.yml
  format: yaml
  label: Quant Network Nodes API
  slug: quant-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-nodes-api-openapi.yml
- filename: quant-observability-api-openapi.yml
  format: yaml
  label: Quant Network Observability API
  slug: quant-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-observability-api-openapi.yml
- filename: quant-rpc-api-openapi.yml
  format: yaml
  label: Quant Network RPC API
  slug: quant-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-rpc-api-openapi.yml
- filename: quant-stakes-api-openapi.yml
  format: yaml
  label: Quant Network Stakes API
  slug: quant-stakes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-stakes-api-openapi.yml
- filename: quant-swaps-api-openapi.yml
  format: yaml
  label: Quant Network Swaps API
  slug: quant-swaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-swaps-api-openapi.yml
- filename: quant-tracker-address-api-openapi.yml
  format: yaml
  label: Quant Network Tracker Address API
  slug: quant-tracker-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-tracker-address-api-openapi.yml
- filename: quant-tracker-event-api-openapi.yml
  format: yaml
  label: Quant Network Tracker Event API
  slug: quant-tracker-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-tracker-event-api-openapi.yml
- filename: quant-tracker-transaction-api-openapi.yml
  format: yaml
  label: Quant Network Tracker Transaction API
  slug: quant-tracker-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-tracker-transaction-api-openapi.yml
- filename: quant-user-api-openapi.yml
  format: yaml
  label: Quant Network User API
  slug: quant-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-user-api-openapi.yml
- filename: quant-withdrawals-api-openapi.yml
  format: yaml
  label: Quant Network Withdrawals API
  slug: quant-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/openapi/quant-withdrawals-api-openapi.yml
consequence_counts:
  physical: 6
  read: 45
  safety-critical: 3
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Quant Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /deployed-contracts/{contractAddress}/permissions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /users/me/api-keys/{keyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /users/me/providers/{providerId}/reset-policy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /deployed-contracts/{contractAddress}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployed-contracts/{contractAddress}/permissions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /withdrawals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /withdrawals/{id}/finalize-tx
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /withdrawals/{id}/prove-tx
operation_count: 70
overview: 'Quant Network exposes 70 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 45 read, 16 write, 6 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Quant Network
provider_slug: quant
slug: quant-agentic-access
source_filename: quant-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/quant-overledger-server-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 70\n  by_action_class:\n    acting: 25\n    connected: 45\n  by_consequence:\n    write: 16\n    read: 45\n    physical: 6\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /accounts/subscribe/{address}\n  method: post\n  operationId: subscribeAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/unsubscribe/{subscriptionId}\n\
  \  method: delete\n  operationId: unsubscribeAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{address}/events\n  method: get\n  operationId: listAddressEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployed-contracts/{contractAddress}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployed-contracts/{contractAddress}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployed-contracts/{contractAddress}/permissions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deployed-contracts/{contractAddress}/permissions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployed-contracts/{contractAddress}/permissions\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /deposits\n  method: post\n  operationId: createDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deposits/allowance\n  method: get\n  operationId: getDepositAllowance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deposits/balances\n  method: get\n  operationId: getDepositBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /deposits/{id}\n  method: get\n  operationId: getDeposit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deposits/{id}/status\n  method: get\n  operationId: checkDepositStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/subscribe\n  method: post\n  operationId: subscribeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/subscriptions/{subscriptionId}/events\n  method: get\n  operationId: listEventSubscriptionEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/unsubscribe/{subscriptionId}\n  method: delete\n  operationId: unsubscribeEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flow/apps/{appId}/events\n  method: get\n  operationId: replayEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow/apps/{appId}/query/{queryId}\n  method: get\n  operationId: queryAppState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow/apps/{appId}/subscriptions\n  method: post\n  operationId: createSubscription\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flow/apps/{appId}/subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow/apps/{appId}/subscriptions/{subscriptionId}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flow/registry/apps\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow/registry/apps/components\n  method: get\n  operationId: getAllowedComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow/registry/apps/{appId}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow/sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flow/sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow/sessions/{sessionId}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow/sessions/{sessionId}/steps/{stepId}\n  method: get\n  operationId: getStep\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow/sessions/{sessionId}/steps/{stepId}\n  method: post\n  operationId: submitStep\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networks/fusion\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networks/total\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nodes\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nodes/{nodeId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ready\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rpc/{apiKey}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stakes\n  method:\
  \ post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stakes/address\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swaps\n  method: post\n  operationId: createSwap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /swaps/quote\n  method: post\n  operationId: getSwapQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /swaps/tokens\n  method: get\n  operationId: getSupportedSwapTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swaps/{id}\n  method: get\n  operationId: getSwap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /swaps/{id}/status\n  method: get\n  operationId: checkSwapStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/track\n  method: post\n  operationId: trackTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /transactions/{transactionId}/status\n  method: get\n  operationId: getTransactionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/access-details\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/api-keys\n  method: post\n  operationId: mintApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /users/me/api-keys/{keyId}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users/me/deployed-contracts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/deposits\n  method: get\n  operationId: listUserDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/history\n  method: get\n  operationId: getUserHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/id\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/nodes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/providers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/providers/{providerId}/reactivate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/me/providers/{providerId}/reset-policy\n\
  \  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users/me/stakes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/stakes/total\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/swaps\n  method: get\n  operationId: getUserSwaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/transactions\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/me/withdrawals\n  method: get\n  operationId: getUserWithdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /withdrawals\n  method: post\n  operationId: createWithdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /withdrawals/action-required\n  method: get\n  operationId: getActionableWithdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /withdrawals/{id}\n\
  \  method: get\n  operationId: getWithdrawalById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /withdrawals/{id}/finalize-tx\n  method: post\n  operationId: recordFinalizeTx\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /withdrawals/{id}/prove-tx\n  method: post\n  operationId: recordProveTx\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /withdrawals/{id}/status\n  method: get\n  operationId: checkWithdrawalStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/agentic-access/quant-agentic-access.yml
summary_line: 70 operations · 25 acting · 3 human-in-the-loop
tags:
- Blockchain
- Distributed Ledger
- Interoperability
- Overledger
- Smart Contracts
- Digital Assets
- Web3
---
