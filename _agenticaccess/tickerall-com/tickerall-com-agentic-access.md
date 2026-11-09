---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 19
api_specs:
- filename: tickerall-com-accounts-api-openapi.yml
  format: yaml
  label: tickerall-com Accounts API
  slug: tickerall-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-accounts-api-openapi.yml
- filename: tickerall-com-bulk-api-openapi.yml
  format: yaml
  label: tickerall-com Bulk API
  slug: tickerall-com-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-bulk-api-openapi.yml
- filename: tickerall-com-candles-history-api-openapi.yml
  format: yaml
  label: tickerall-com Candles & History API
  slug: tickerall-com-candles-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-candles-history-api-openapi.yml
- filename: tickerall-com-copy-trading-api-openapi.yml
  format: yaml
  label: tickerall-com Copy Trading API
  slug: tickerall-com-copy-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-copy-trading-api-openapi.yml
- filename: tickerall-com-orders-api-openapi.yml
  format: yaml
  label: tickerall-com Orders API
  slug: tickerall-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-orders-api-openapi.yml
- filename: tickerall-com-sessions-api-openapi.yml
  format: yaml
  label: tickerall-com Sessions API
  slug: tickerall-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-sessions-api-openapi.yml
- filename: tickerall-com-symbols-api-openapi.yml
  format: yaml
  label: tickerall-com Symbols API
  slug: tickerall-com-symbols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-symbols-api-openapi.yml
- filename: tickerall-com-trade-history-api-openapi.yml
  format: yaml
  label: tickerall-com Trade History API
  slug: tickerall-com-trade-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-trade-history-api-openapi.yml
consequence_counts:
  physical: 6
  read: 19
  safety-critical: 7
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 7
kind: agentic-access
layout: agentic-access
method: generated
name: Tickerall Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/accounts/{id}/orders
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/accounts/{id}/orders/{ticket}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/accounts/{id}/orders/{ticket}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/accounts/{id}/positions/{ticket}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/bulk/orders/cancel
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/bulk/orders/modify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/bulk/positions/modify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounts/{id}/orders/cancel-all
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounts/{id}/positions/close-all
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/accounts/{id}/positions/{ticket}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/bulk/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/copy/sets
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/copy/sets/{setId}/followers/{followerId}
operation_count: 44
overview: 'tickerall-com exposes 44 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 12 write, 6 physical, and 7 safety-critical.


  7 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tickerall-com
provider_slug: tickerall-com
slug: tickerall-com-agentic-access
source_filename: tickerall-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/tickerall-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    acting: 25\n    connected: 19\n  by_consequence:\n    write: 12\n    read: 19\n    safety-critical: 7\n    physical: 6\n  human_in_the_loop_required: 7\noperations:\n- path: /v1/sessions\n  method: post\n  operationId: postV1Sessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{accountId}\n  method: delete\n  operationId: deleteV1SessionsAccountId\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts\n  method: get\n  operationId: getV1Accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{id}\n  method: get\n  operationId: getV1AccountsId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{id}\n  method: delete\n  operationId: deleteV1AccountsId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{id}/positions\n  method: get\n  operationId: getV1AccountsIdPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{id}/migrate\n  method: post\n  operationId: postV1AccountsIdMigrate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{id}/always-hot\n  method: patch\n  operationId: patchV1AccountsIdAlwayshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/always-hot\n  method: patch\n  operationId: patchV1Alwayshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/always-hot/pending\n  method: get\n  operationId: getV1AlwayshotPending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/remember-password\n  method: get\n  operationId: getV1Rememberpassword\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/remember-password\n  method: patch\n  operationId: patchV1Rememberpassword\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{id}/symbols\n  method: get\n  operationId: getV1AccountsIdSymbols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{id}/symbol-specs\n  method: get\n  operationId: getV1AccountsIdSymbolspecs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{id}/candles\n  method: get\n  operationId: getV1AccountsIdCandles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/candles\n  method: get\n  operationId: getV1PublicCandles\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{id}/orders\n  method: post\n  operationId: postV1AccountsIdOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/accounts/{id}/orders\n  method: get\n  operationId: getV1AccountsIdOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{id}/orders/{ticket}\n  method: delete\n  operationId: deleteV1AccountsIdOrdersTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/accounts/{id}/orders/{ticket}\n  method: patch\n  operationId: patchV1AccountsIdOrdersTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/accounts/{id}/orders/cancel-all\n  method: post\n  operationId: postV1AccountsIdOrdersCancelall\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{id}/positions/{ticket}\n  method: delete\n  operationId: deleteV1AccountsIdPositionsTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{id}/positions/{ticket}\n  method: patch\n  operationId: patchV1AccountsIdPositionsTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/accounts/{id}/positions/close-all\n  method: post\n  operationId:\
  \ postV1AccountsIdPositionsCloseall\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{id}/history\n  method: get\n  operationId: getV1AccountsIdHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{id}/deals-history\n  method: get\n  operationId: getV1AccountsIdDealshistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{id}/orders-history\n  method: get\n  operationId: getV1AccountsIdOrdershistory\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{id}/balance-operations\n  method: get\n  operationId: getV1AccountsIdBalanceoperations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bulk/orders\n  method: post\n  operationId: postV1BulkOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bulk/positions/close\n  method: post\n  operationId: postV1BulkPositionsClose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bulk/positions/modify\n  method: post\n  operationId: postV1BulkPositionsModify\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/bulk/orders/cancel\n  method: post\n  operationId: postV1BulkOrdersCancel\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/bulk/orders/modify\n  method: post\n  operationId:\
  \ postV1BulkOrdersModify\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/bulk/accounts\n  method: get\n  operationId: getV1BulkAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/copy/sets\n  method: post\n  operationId: postV1CopySets\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/copy/sets\n  method: get\n\
  \  operationId: getV1CopySets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/copy/sets/{setId}\n  method: get\n  operationId: getV1CopySetsSetId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/copy/sets/{setId}\n  method: patch\n  operationId: patchV1CopySetsSetId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/copy/sets/{setId}\n  method: delete\n  operationId: deleteV1CopySetsSetId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/copy/sets/{setId}/followers\n  method: post\n  operationId: postV1CopySetsSetIdFollowers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/copy/sets/{setId}/followers/{followerId}\n  method: patch\n  operationId: patchV1CopySetsSetIdFollowersFollowerId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/copy/sets/{setId}/followers/{followerId}\n\
  \  method: delete\n  operationId: deleteV1CopySetsSetIdFollowersFollowerId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/copy/sets/{setId}/stats\n  method: get\n  operationId: getV1CopySetsSetIdStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/copy/sets/{setId}/log\n  method: get\n  operationId: getV1CopySetsSetIdLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/tickerall-com/agentic-access/tickerall-com-agentic-access.yml
summary_line: 44 operations · 25 acting · 7 human-in-the-loop
tags:
- Finance
- Trading
- Foreign Exchange
- MT5
- MT4
---
