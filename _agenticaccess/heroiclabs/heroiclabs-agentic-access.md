---
acting_count: 249
action_class_counts:
  acting: 249
  connected: 61
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Nakama API
  slug: nakama-api
  spec_type: OpenAPI
  url: https://heroiclabs.github.io/nakama-docs/
- filename: heroiclabs-hiro-rpc-api-openapi.yml
  format: yaml
  label: Hiro RPC API
  slug: hiro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroiclabs/refs/heads/main/openapi/heroiclabs-hiro-rpc-api-openapi.yml
consequence_counts:
  physical: 18
  read: 61
  safety-critical: 5
  write: 226
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Heroiclabs Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rpc/RPC_ID_PROGRESSIONS_RESET?unwrap
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rpc/RPC_ID_STREAKS_RESET?unwrap
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /rpc/RPC_ID_TUTORIALS_RESET?unwrap
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/console/user/{username}/mfa/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/console/user/{username}/reset/password
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/RPC_ID_ECONOMY_PURCHASE_INTENT?unwrap
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/RPC_ID_ECONOMY_PURCHASE_ITEM?unwrap
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/RPC_ID_ECONOMY_PURCHASE_RESTORE?unwrap
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/RPC_ID_INCENTIVES_SENDER_CLAIM?unwrap
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/RPC_ID_INCENTIVES_SENDER_CREATE?unwrap
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/RPC_ID_INCENTIVES_SENDER_DELETE?unwrap
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/RPC_ID_INCENTIVES_SENDER_LIST?unwrap
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/RPC_ID_PROGRESSIONS_PURCHASE?unwrap
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/RPC_ID_TEAMS_STORE_PURCHASE?unwrap
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/RPC_ID_UNLOCKABLES_PURCHASE_SLOT?unwrap
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rpc/RPC_ID_UNLOCKABLES_PURCHASE_UNLOCK?unwrap
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/console/account/{id}/friend/{friend_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/console/notification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/console/satori/direct-message
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/iap/purchase/apple
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/iap/purchase/facebookinstant
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/iap/purchase/google
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/iap/purchase/huawei
operation_count: 310
overview: 'Heroic Labs exposes 310 API operations that an AI agent could call, of which 249 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 61 read, 226 write, 18 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Heroic Labs
provider_slug: heroiclabs
slug: heroiclabs-agentic-access
source_filename: heroiclabs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/heroiclabs-hiro-rpc-api-openapi.yml, openapi/heroiclabs-nakama-api-openapi.yml,\n  openapi/heroiclabs-nakama-console-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 310\n  by_action_class:\n    acting: 249\n    connected: 61\n  by_consequence:\n    write: 226\n    physical: 18\n    safety-critical: 5\n    read: 61\n  human_in_the_loop_required: 5\noperations:\n- path: /rpc/RPC_ID_INVENTORY_LIST?unwrap\n  method: post\n  operationId: INVENTORY_LIST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_INVENTORY_LIST_INVENTORY?unwrap\n  method: post\n  operationId: INVENTORY_LIST_INVENTORY\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_INVENTORY_CONSUME?unwrap\n  method: post\n  operationId: INVENTORY_CONSUME\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_INVENTORY_GRANT?unwrap\n  method: post\n  operationId: INVENTORY_GRANT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_INVENTORY_UPDATE?unwrap\n  method: post\n  operationId: INVENTORY_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_INVENTORY_DELETE?unwrap\n  method: post\n  operationId: INVENTORY_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ECONOMY_DONATION_CLAIM?unwrap\n  method: post\n  operationId:\
  \ ECONOMY_DONATION_CLAIM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ECONOMY_DONATION_GIVE?unwrap\n  method: post\n  operationId: ECONOMY_DONATION_GIVE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ECONOMY_DONATION_GET?unwrap\n  method: post\n  operationId: ECONOMY_DONATION_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ECONOMY_DONATION_REQUEST?unwrap\n  method: post\n  operationId: ECONOMY_DONATION_REQUEST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ECONOMY_STORE_GET?unwrap\n  method: post\n  operationId: ECONOMY_STORE_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ECONOMY_GRANT?unwrap\n  method: post\n  operationId: ECONOMY_GRANT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ECONOMY_PURCHASE_INTENT?unwrap\n  method: post\n  operationId: ECONOMY_PURCHASE_INTENT\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ECONOMY_PURCHASE_ITEM?unwrap\n  method: post\n  operationId: ECONOMY_PURCHASE_ITEM\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ECONOMY_PURCHASE_RESTORE?unwrap\n  method: post\n  operationId: ECONOMY_PURCHASE_RESTORE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ECONOMY_PLACEMENT_STATUS?unwrap\n  method: post\n  operationId: ECONOMY_PLACEMENT_STATUS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ECONOMY_PLACEMENT_START?unwrap\n  method: post\n  operationId: ECONOMY_PLACEMENT_START\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ACHIEVEMENTS_CLAIM?unwrap\n  method: post\n  operationId: ACHIEVEMENTS_CLAIM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ACHIEVEMENTS_GET?unwrap\n  method: post\n  operationId: ACHIEVEMENTS_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /rpc/RPC_ID_ACHIEVEMENTS_UPDATE?unwrap\n  method: post\n  operationId: ACHIEVEMENTS_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ENERGY_GET?unwrap\n  method: post\n  operationId: ENERGY_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ENERGY_SPEND?unwrap\n  method: post\n  operationId: ENERGY_SPEND\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ENERGY_GRANT?unwrap\n  method: post\n  operationId: ENERGY_GRANT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_ENERGY_SPEND_WITH_REFILL_START_TIME?unwrap\n  method: post\n  operationId: ENERGY_SPEND_WITH_REFILL_START_TIME\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TUTORIALS_GET?unwrap\n  method: post\n  operationId: TUTORIALS_GET\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TUTORIALS_ACCEPT?unwrap\n  method: post\n  operationId: TUTORIALS_ACCEPT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TUTORIALS_DECLINE?unwrap\n  method: post\n  operationId: TUTORIALS_DECLINE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TUTORIALS_ABANDON?unwrap\n\
  \  method: post\n  operationId: TUTORIALS_ABANDON\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TUTORIALS_UPDATE?unwrap\n  method: post\n  operationId: TUTORIALS_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TUTORIALS_RESET?unwrap\n  method: post\n  operationId: TUTORIALS_RESET\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_CREATE?unwrap\n  method: post\n  operationId: TEAMS_CREATE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_UPDATE?unwrap\n  method: post\n  operationId: TEAMS_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_LIST?unwrap\n  method: post\n  operationId: TEAMS_LIST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_SEARCH?unwrap\n  method: post\n  operationId: TEAMS_SEARCH\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_GET?unwrap\n  method: post\n  operationId: TEAMS_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_USER_TEAMS_LIST?unwrap\n  method: post\n  operationId: TEAMS_USER_TEAMS_LIST\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_WRITE_CHAT_MESSAGE?unwrap\n  method: post\n  operationId: TEAMS_WRITE_CHAT_MESSAGE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_STORE_GET?unwrap\n  method: post\n  operationId: TEAMS_STORE_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_STORE_PURCHASE?unwrap\n  method: post\n  operationId: TEAMS_STORE_PURCHASE\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_WALLET_GET?unwrap\n  method: post\n  operationId: TEAMS_WALLET_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_WALLET_GRANT?unwrap\n  method: post\n  operationId: TEAMS_WALLET_GRANT\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_STATS_GET?unwrap\n  method: post\n  operationId: TEAMS_STATS_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_STATS_UPDATE?unwrap\n  method: post\n  operationId: TEAMS_STATS_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_INVENTORY_LIST?unwrap\n\
  \  method: post\n  operationId: TEAMS_INVENTORY_LIST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_INVENTORY_LIST_INVENTORY?unwrap\n  method: post\n  operationId: TEAMS_INVENTORY_LIST_INVENTORY\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_INVENTORY_CONSUME?unwrap\n  method: post\n  operationId: TEAMS_INVENTORY_CONSUME\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_INVENTORY_GRANT?unwrap\n  method: post\n  operationId: TEAMS_INVENTORY_GRANT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_INVENTORY_UPDATE?unwrap\n  method: post\n  operationId: TEAMS_INVENTORY_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_ACHIEVEMENTS_CLAIM?unwrap\n  method: post\n  operationId: TEAMS_ACHIEVEMENTS_CLAIM\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_ACHIEVEMENTS_GET?unwrap\n  method: post\n  operationId: TEAMS_ACHIEVEMENTS_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_ACHIEVEMENTS_UPDATE?unwrap\n  method: post\n  operationId: TEAMS_ACHIEVEMENTS_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /rpc/RPC_ID_TEAMS_EVENT_LEADERBOARD_LIST?unwrap\n  method: post\n  operationId: TEAMS_EVENT_LEADERBOARD_LIST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_EVENT_LEADERBOARD_GET?unwrap\n  method: post\n  operationId: TEAMS_EVENT_LEADERBOARD_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_EVENT_LEADERBOARD_UPDATE?unwrap\n  method: post\n  operationId: TEAMS_EVENT_LEADERBOARD_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_EVENT_LEADERBOARD_CLAIM?unwrap\n  method: post\n  operationId: TEAMS_EVENT_LEADERBOARD_CLAIM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_EVENT_LEADERBOARD_ROLL?unwrap\n  method: post\n  operationId: TEAMS_EVENT_LEADERBOARD_ROLL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /rpc/RPC_ID_TEAMS_EVENT_LEADERBOARD_DEBUG_FILL?unwrap\n  method: post\n  operationId: TEAMS_EVENT_LEADERBOARD_DEBUG_FILL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_EVENT_LEADERBOARD_DEBUG_RANDOM_SCORES?unwrap\n  method: post\n  operationId: TEAMS_EVENT_LEADERBOARD_DEBUG_RANDOM_SCORES\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_REWARD_MAILBOX_LIST?unwrap\n  method: post\n  operationId: TEAMS_REWARD_MAILBOX_LIST\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_REWARD_MAILBOX_CLAIM?unwrap\n  method: post\n  operationId: TEAMS_REWARD_MAILBOX_CLAIM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_REWARD_MAILBOX_DELETE?unwrap\n  method: post\n  operationId: TEAMS_REWARD_MAILBOX_DELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /rpc/RPC_ID_TEAMS_GIFT_LIST?unwrap\n  method: post\n  operationId: TEAMS_GIFT_LIST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_GIFT_CONTRIBUTE?unwrap\n  method: post\n  operationId: TEAMS_GIFT_CONTRIBUTE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_TEAMS_GIFT_CLAIM?unwrap\n  method: post\n  operationId: TEAMS_GIFT_CLAIM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_UNLOCKABLES_CREATE?unwrap\n  method: post\n  operationId: UNLOCKABLES_CREATE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_UNLOCKABLES_GET?unwrap\n  method: post\n  operationId: UNLOCKABLES_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_UNLOCKABLES_UNLOCK_START?unwrap\n  method: post\n  operationId: UNLOCKABLES_UNLOCK_START\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_UNLOCKABLES_PURCHASE_UNLOCK?unwrap\n  method: post\n  operationId: UNLOCKABLES_PURCHASE_UNLOCK\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_UNLOCKABLES_PURCHASE_SLOT?unwrap\n  method: post\n  operationId: UNLOCKABLES_PURCHASE_SLOT\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_UNLOCKABLES_CLAIM?unwrap\n  method: post\n  operationId: UNLOCKABLES_CLAIM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_UNLOCKABLES_QUEUE_ADD?unwrap\n  method: post\n  operationId: UNLOCKABLES_QUEUE_ADD\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_UNLOCKABLES_QUEUE_REMOVE?unwrap\n  method: post\n  operationId: UNLOCKABLES_QUEUE_REMOVE\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_UNLOCKABLES_QUEUE_SET?unwrap\n  method: post\n  operationId: UNLOCKABLES_QUEUE_SET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_BASE_RATE_APP?unwrap\n  method: post\n  operationId: BASE_RATE_APP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /rpc/RPC_ID_BASE_SET_DEVICE_PREFS?unwrap\n  method: post\n  operationId: BASE_SET_DEVICE_PREFS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_BASE_SYNC?unwrap\n  method: post\n  operationId: BASE_SYNC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_LEADERBOARDS_CONFIG_GET?unwrap\n  method: post\n  operationId: LEADERBOARDS_CONFIG_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_LEADERBOARD_LIST?unwrap\n  method: post\n  operationId: LEADERBOARD_LIST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_LEADERBOARD_GET?unwrap\n  method: post\n  operationId: LEADERBOARD_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_LEADERBOARD_UPDATE?unwrap\n  method: post\n  operationId: LEADERBOARD_UPDATE\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_LEADERBOARD_SCORES_LIST?unwrap\n  method: post\n  operationId: LEADERBOARD_SCORES_LIST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_LEADERBOARD_SCORES_LIST_AROUND_OWNER?unwrap\n  method: post\n  operationId: LEADERBOARD_SCORES_LIST_AROUND_OWNER\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /rpc/RPC_ID_EVENT_LEADERBOARD_LIST?unwrap\n  method: post\n  operationId: EVENT_LEADERBOARD_LIST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_EVENT_LEADERBOARD_GET?unwrap\n  method: post\n  operationId: EVENT_LEADERBOARD_GET\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_EVENT_LEADERBOARD_UPDATE?unwrap\n  method: post\n  operationId: EVENT_LEADERBOARD_UPDATE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_EVENT_LEADERBOARD_CLAIM?unwrap\n  method: post\n  operationId: EVENT_LEADERBOARD_CLAIM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_EVENT_LEADERBOARD_ROLL?unwrap\n  method: post\n  operationId: EVENT_LEADERBOARD_ROLL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rpc/RPC_ID_EVENT_LEADERBOARD_DEBUG_FILL?unwrap\n  method:\
  \ post\n  operationId: EVENT_LEADERBOARD_DEBUG_FILL\n  x-ag\n\n# --- truncated at 32 KB (101 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/heroiclabs/refs/heads/main/agentic-access/heroiclabs-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heroiclabs/refs/heads/main/agentic-access/heroiclabs-agentic-access.yml
summary_line: 310 operations · 249 acting · 5 human-in-the-loop
tags:
- Game Backend
- Multiplayer
- Real-Time
- WebSocket
- Matchmaking
- Leaderboards
- Social Gaming
- Open Source
- LiveOps
- gRPC
---
