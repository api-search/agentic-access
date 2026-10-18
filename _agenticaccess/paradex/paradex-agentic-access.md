---
acting_count: 51
action_class_counts:
  acting: 51
  connected: 82
api_specs:
- filename: paradex-websocket-asyncapi.yml
  format: yaml
  label: Paradex WebSocket API
  slug: paradex-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/asyncapi/paradex-websocket-asyncapi.yml
- filename: paradex-account-api-openapi.yml
  format: yaml
  label: Paradex Account API
  slug: paradex-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-account-api-openapi.yml
- filename: paradex-algos-api-openapi.yml
  format: yaml
  label: Paradex Algos API
  slug: paradex-algos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-algos-api-openapi.yml
- filename: paradex-authentication-api-openapi.yml
  format: yaml
  label: Paradex Authentication API
  slug: paradex-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-authentication-api-openapi.yml
- filename: paradex-blocktrades-api-openapi.yml
  format: yaml
  label: Paradex Block Trades API
  slug: paradex-blocktrades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-blocktrades-api-openapi.yml
- filename: paradex-insurance-api-openapi.yml
  format: yaml
  label: Paradex Insurance API
  slug: paradex-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-insurance-api-openapi.yml
- filename: paradex-liquidations-api-openapi.yml
  format: yaml
  label: Paradex Liquidations API
  slug: paradex-liquidations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-liquidations-api-openapi.yml
- filename: paradex-marketmakerprotection-api-openapi.yml
  format: yaml
  label: Paradex Market Maker Protection API
  slug: paradex-marketmakerprotection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-marketmakerprotection-api-openapi.yml
- filename: paradex-markets-api-openapi.yml
  format: yaml
  label: Paradex Markets API
  slug: paradex-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-markets-api-openapi.yml
- filename: paradex-orders-api-openapi.yml
  format: yaml
  label: Paradex Orders API
  slug: paradex-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-orders-api-openapi.yml
- filename: paradex-referrals-api-openapi.yml
  format: yaml
  label: Paradex Referrals API
  slug: paradex-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-referrals-api-openapi.yml
- filename: paradex-rfqs-api-openapi.yml
  format: yaml
  label: Paradex Rfqs API
  slug: paradex-rfqs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-rfqs-api-openapi.yml
- filename: paradex-staking-api-openapi.yml
  format: yaml
  label: Paradex Staking API
  slug: paradex-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-staking-api-openapi.yml
- filename: paradex-subkey-api-openapi.yml
  format: yaml
  label: Paradex Subkey API
  slug: paradex-subkey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-subkey-api-openapi.yml
- filename: paradex-system-api-openapi.yml
  format: yaml
  label: Paradex System API
  slug: paradex-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-system-api-openapi.yml
- filename: paradex-token-api-openapi.yml
  format: yaml
  label: Paradex Token API
  slug: paradex-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-token-api-openapi.yml
- filename: paradex-trades-api-openapi.yml
  format: yaml
  label: Paradex Trades API
  slug: paradex-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-trades-api-openapi.yml
- filename: paradex-transfers-api-openapi.yml
  format: yaml
  label: Paradex Transfers API
  slug: paradex-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-transfers-api-openapi.yml
- filename: paradex-vaults-api-openapi.yml
  format: yaml
  label: Paradex Vaults API
  slug: paradex-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-vaults-api-openapi.yml
- filename: paradex-xptransfersv2-api-openapi.yml
  format: yaml
  label: Paradex XP Transfers V2 API
  slug: paradex-xptransfersv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/openapi/paradex-xptransfersv2-api-openapi.yml
consequence_counts:
  physical: 17
  read: 82
  safety-critical: 3
  write: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Paradex Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /account/keys/subkeys/{public_key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /account/mmp/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /account/tokens/{lookup_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /account/keys/subkeys/{public_key}/block-trade-signing
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /algo/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /algo/orders/{algo_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /block-trades
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /block-trades/{block_trade_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /block-trades/{block_trade_id}/execute
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /block-trades/{block_trade_id}/offers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /block-trades/{block_trade_id}/offers/{offer_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /block-trades/{block_trade_id}/offers/{offer_id}/execute
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/by_client_id/{client_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /xp/transfer
operation_count: 133
overview: 'Paradex exposes 133 API operations that an AI agent could call, of which 51 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 82 read, 31 write, 17 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paradex
provider_slug: paradex
slug: paradex-agentic-access
source_filename: paradex-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/paradex-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 133\n  by_action_class:\n    connected: 82\n    acting: 51\n  by_consequence:\n    read: 82\n    write: 31\n    safety-critical: 3\n    physical: 17\n  human_in_the_loop_required: 3\noperations:\n- path: /account\n  method: get\n  operationId: get-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/compliance\n  method: get\n  operationId: get-compliance-actions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /account/compliance\n  method: post\n  operationId: record-compliance-action\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/history\n  method: get\n  operationId: get-account-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/info\n  method: get\n  operationId: get-accounts-info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/keys/subkeys\n  method: get\n  operationId: list-subkeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /account/keys/subkeys\n  method: post\n  operationId: register-subkey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/keys/subkeys/activate\n  method: post\n  operationId: activate-subkey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/keys/subkeys/{public_key}\n  method: get\n  operationId: get-subkey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/keys/subkeys/{public_key}\n\
  \  method: put\n  operationId: update-subkey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/keys/subkeys/{public_key}\n  method: delete\n  operationId: revoke-subkey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account/keys/subkeys/{public_key}/allowed-cidrs\n  method: put\n  operationId: update-subkey-allowed-cidrs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/keys/subkeys/{public_key}/block-trade-signing\n  method: put\n  operationId: update-subkey-block-trade-signing\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/margin\n  method: get\n  operationId: get-account-margin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/margin/{market}\n  method: post\n  operationId: upsert-account-margin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/mmp\n  method: get\n  operationId: get-account-mmp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/mmp/reset\n  method: post\n  operationId: reset-account-mmp\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account/mmp/{base_asset}\n  method: post\n  operationId: upsert-account-mmp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/mmp/{base_asset}\n  method: delete\n  operationId: delete-account-mmp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/paradigm/enable\n  method: post\n  operationId: rfq-enable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/profile\n  method: get\n  operationId: get-account-profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/profile\n  method: put\n  operationId: update-account-profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/profile/market_max_slippage/{market}\n  method: post\n  operationId: update-account-market-max-slippage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/profile/notifications\n  method: post\n  operationId: update-account-notification-preferences\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/profile/notifications/last_seen\n  method: post\n  operationId: update-last-seen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/profile/referral_code\n  method: post\n  operationId: update-account-profile-referral-code\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/profile/refresh_inventory\n\
  \  method: post\n  operationId: refresh-account-inventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/profile/size_currency_display\n  method: post\n  operationId: update-account-size-currency-display\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/profile/username\n  method: post\n  operationId: update-account-profile-username\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/referrer\n  method: post\n  operationId: update-account-referrer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/settings\n  method: get\n  operationId: get-account-settings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/settings/trading_value_display\n  method: post\n  operationId: update-account-trading-value-display\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/subaccounts\n  method: get\n  operationId: get-sub-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/summary\n  method: get\n  operationId: get-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/terminal-token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/tokens\n  method: get\n  operationId: list-tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/tokens\n  method: post\n  operationId: create-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/tokens/{lookup_id}\n  method: delete\n  operationId: revoke-token\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account/tokens/{lookup_id}/allowed-cidrs\n  method: put\n  operationId: update-token-allowed-cidrs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /algo/orders\n  method: get\n  operationId: get-open-algo-orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /algo/orders\n  method: post\n  operationId: create-algo-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /algo/orders-history\n  method: get\n  operationId: get-algo-orders-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /algo/orders/{algo_id}\n  method: get\n  operationId: get-algo-order-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /algo/orders/{algo_id}\n  method: delete\n  operationId: cancel-algo-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth\n  method: post\n  operationId: auth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balance\n  method: get\n  operationId: get-balance\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bbo/{market}\n  method: get\n  operationId: get-bbo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bbo/{market}/interactive\n  method: get\n  operationId: get-bbo-interactive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block-trades\n  method: get\n  operationId: block-trades-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block-trades\n  method: post\n  operationId: block-trades-create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /block-trades/{block_trade_id}\n  method: get\n  operationId: block-trades-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block-trades/{block_trade_id}\n  method: delete\n  operationId: block-trades-cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /block-trades/{block_trade_id}/execute\n  method: post\n  operationId: block-trades-execute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /block-trades/{block_trade_id}/offers\n  method: get\n  operationId: block-offers-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block-trades/{block_trade_id}/offers\n  method: post\n  operationId: block-offers-create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /block-trades/{block_trade_id}/offers/{offer_id}\n  method: get\n  operationId: block-offers-get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /block-trades/{block_trade_id}/offers/{offer_id}\n  method: delete\n  operationId: block-offers-cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /block-trades/{block_trade_id}/offers/{offer_id}/execute\n  method: post\n  operationId: block-offers-execute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /fills\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funding/data\n  method: get\n  operationId: get-funding-data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funding/payments\n  method: get\n  operationId: get-funding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insurance\n  method: get\n  operationId: get-insurance-fund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jwks.json\n  method: get\n  operationId: jwks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /liquidations\n  method: get\n  operationId: get-liquidations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets\n  method: get\n  operationId: get-markets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/history\n  method: get\n  operationId: get-markets-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/klines\n  method: get\n  operationId: markets-klines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/settlement-price\n  method: get\n  operationId:\
  \ get-market-settlement-price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/summary\n  method: get\n  operationId: get-markets-summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onboarding\n  method: get\n  operationId: getOnboarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onboarding\n  method: post\n  operationId: onboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orderbook/{market}\n  method: get\n  operationId:\
  \ get-orderbook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orderbook/{market}/impact-price\n  method: get\n  operationId: get-impact-price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orderbook/{market}/interactive\n  method: get\n  operationId: get-orderbook-interactive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: get-open-orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: orders-new\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: delete\n  operationId: orders-cancel-all\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders-history\n  method: get\n  operationId: get-orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/batch\n  method: post\n  operationId: orders-new-batch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/batch\n  method: delete\n  operationId: orders-cancel-batch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/by_client_id/{client_id}\n  method: get\n  operationId: orders-get-by-client-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/by_client_id/{client_id}\n  method: delete\n  operationId: orders-cancel-by-client-id\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}\n  method: get\n  operationId: orders-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}\n  method: put\n  operationId: orders-modify\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}\n  method: delete\n\
  \  operationId: orders-cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /positions\n  method: get\n  operationId: get-positions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referrals/qr-code\n  method: get\n  operationId: get-referral-qr-code\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referrals/summary\n  method: get\n  operationId: get-referrals-summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /rfqs\n  method: get\n  operationId: rfq-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rfqs\n  method: post\n  operationId: rfq-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rfqs/drafts\n  method: get\n  operationId: rfq-draft-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rfqs/drafts\n  method: post\n  operationId: rfq-draft-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rfqs/drafts/{draft_id}\n  method: delete\n  operationId: rfq-draft-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rfqs/markets\n  method: get\n  operationId: rfq-markets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rfqs/platform-state\n  method: get\n  operationId: rfq-platform-state\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rfqs/{rfq_id}\n  method: delete\n  operationId: rfq-delete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rfqs/{rfq_id}/bbo\n  method: get\n  operationId: rfq-bbo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rfqs/{rfq_id}/execute\n  method: post\n  operationId: rfq-execute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /staking/balance/history\n  method: get\n  operationId: get-staking-balance-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/balance/history/global\n  method: get\n  operationId: get-global-staking-balance-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/config\n  method: get\n  operationId: get-staking-config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/history\n  method: get\n  operationId: get-staking-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /staking/summary\n  method: get\n  operationId: get-staking-summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/announcements\n\
  \  method: get\n  operationId: get-announcements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/config\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/margin-config\n  method: get\n  operationId: get-margin-config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/portfolio-margin-config\n  method: get\n  operationId: get-portfolio-margin-config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/state\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /system/time\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/volume-tiers\n  method: get\n  operationId: get-volume-tiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tradebusts\n  method: get\n  operationId: tradebusts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trades\n  method: get\n  operationId: trades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers\n  method: get\n  operationId: get-transfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/auth\n  method: post\n  operationId: evmAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/onboarding\n  method: post\n  operationId: evmOnboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (35 KB\
  \ total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/agentic-access/paradex-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paradex/refs/heads/main/agentic-access/paradex-agentic-access.yml
summary_line: 133 operations · 51 acting · 3 human-in-the-loop
tags:
- Company
- Cryptocurrency
- Exchange
- Derivatives
- Trading
- Perpetual Futures
- DeFi
- WebSocket
- MCP
---
