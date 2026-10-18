---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 46
api_specs:
- filename: clearstreet8e71-accounts-api-openapi.yml
  format: yaml
  label: Clearstreet8e71 Accounts API
  slug: clearstreet8e71-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearstreet8e71/refs/heads/main/openapi/clearstreet8e71-accounts-api-openapi.yml
- filename: clearstreet8e71-api-version-api-openapi.yml
  format: yaml
  label: Clearstreet8e71 API version API
  slug: clearstreet8e71-api-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearstreet8e71/refs/heads/main/openapi/clearstreet8e71-api-version-api-openapi.yml
- filename: clearstreet8e71-calendar-api-openapi.yml
  format: yaml
  label: Clearstreet8e71 Calendar API
  slug: clearstreet8e71-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearstreet8e71/refs/heads/main/openapi/clearstreet8e71-calendar-api-openapi.yml
- filename: clearstreet8e71-instrument-data-api-openapi.yml
  format: yaml
  label: Clearstreet8e71 Instrument Data API
  slug: clearstreet8e71-instrument-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearstreet8e71/refs/heads/main/openapi/clearstreet8e71-instrument-data-api-openapi.yml
- filename: clearstreet8e71-instruments-api-openapi.yml
  format: yaml
  label: Clearstreet8e71 Instruments API
  slug: clearstreet8e71-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearstreet8e71/refs/heads/main/openapi/clearstreet8e71-instruments-api-openapi.yml
- filename: clearstreet8e71-omni-ai-api-openapi.yml
  format: yaml
  label: Clearstreet8e71 Omni AI API
  slug: clearstreet8e71-omni-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearstreet8e71/refs/heads/main/openapi/clearstreet8e71-omni-ai-api-openapi.yml
- filename: clearstreet8e71-orders-api-openapi.yml
  format: yaml
  label: Clearstreet8e71 Orders API
  slug: clearstreet8e71-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearstreet8e71/refs/heads/main/openapi/clearstreet8e71-orders-api-openapi.yml
- filename: clearstreet8e71-positions-api-openapi.yml
  format: yaml
  label: Clearstreet8e71 Positions API
  slug: clearstreet8e71-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearstreet8e71/refs/heads/main/openapi/clearstreet8e71-positions-api-openapi.yml
- filename: clearstreet8e71-private-markets-api-openapi.yml
  format: yaml
  label: Clearstreet8e71 Private Markets API
  slug: clearstreet8e71-private-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearstreet8e71/refs/heads/main/openapi/clearstreet8e71-private-markets-api-openapi.yml
- filename: clearstreet8e71-screener-api-openapi.yml
  format: yaml
  label: Clearstreet8e71 Screener API
  slug: clearstreet8e71-screener-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearstreet8e71/refs/heads/main/openapi/clearstreet8e71-screener-api-openapi.yml
- filename: clearstreet8e71-watchlist-api-openapi.yml
  format: yaml
  label: Clearstreet8e71 Watchlist API
  slug: clearstreet8e71-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearstreet8e71/refs/heads/main/openapi/clearstreet8e71-watchlist-api-openapi.yml
consequence_counts:
  physical: 5
  read: 46
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clearstreet8E71 Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/accounts/{account_id}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/accounts/{account_id}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/accounts/{account_id}/orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/accounts/{account_id}/orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/private-markets/iois/{ioi_id}
operation_count: 72
overview: 'Clearstreet8e71 exposes 72 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 46 read, 21 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Clearstreet8e71
provider_slug: clearstreet8e71
slug: clearstreet8e71-agentic-access
source_filename: clearstreet8e71-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/clearstreet8e71-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 72\n  by_action_class:\n    connected: 46\n    acting: 26\n  by_consequence:\n    read: 46\n    write: 21\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/accounts\n  method: get\n  operationId: get_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}\n  method: get\n  operationId: get_account_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /v1/accounts/{account_id}\n  method: patch\n  operationId: patch_account_by_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/balances\n  method: get\n  operationId: get_account_balances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/executions\n  method: get\n  operationId: get_executions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/orders\n  method: get\n  operationId: get_orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/orders\n  method: post\n  operationId: submit_orders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/orders\n  method: delete\n  operationId: cancel_all_open_orders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/orders/{order_id}\n  method: get\n  operationId:\
  \ get_order_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/orders/{order_id}\n  method: delete\n  operationId: cancel_open_order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/orders/{order_id}\n  method: patch\n  operationId: replace_order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v1/accounts/{account_id}/portfolio-history\n  method: get\n  operationId: get_portfolio_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/positions\n  method: get\n  operationId: get_positions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/positions\n  method: delete\n  operationId: close_positions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/positions/instructions\n  method: get\n  operationId: get_position_instructions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{account_id}/positions/instructions\n  method: post\n  operationId: submit_position_instructions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/positions/instructions/{instruction_id}\n  method: delete\n  operationId: cancel_position_instruction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/accounts/{account_id}/positions/{instrument_id}\n\
  \  method: delete\n  operationId: close_position\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/calendars/economic-events\n  method: get\n  operationId: get_economic_events_calendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calendars/market-hours\n  method: get\n  operationId: get_market_hours_calendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/clock\n  method: get\n  operationId: get_clock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/instruments\n  method: get\n  operationId: get_instruments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instruments/events\n  method: get\n  operationId: get_all_instrument_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instruments/options/contracts\n  method: get\n  operationId: get_option_contracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instruments/search\n  method: get\n  operationId: search_instruments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instruments/{instrument_id}\n  method: get\n  operationId:\
  \ get_instrument_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instruments/{instrument_id}/analyst-reporting\n  method: get\n  operationId: get_instrument_analyst_consensus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instruments/{instrument_id}/balance-sheets\n  method: get\n  operationId: get_instrument_balance_sheet_statements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instruments/{instrument_id}/cash-flow-statements\n  method: get\n  operationId: get_instrument_cash_flow_statements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instruments/{instrument_id}/events\n\
  \  method: get\n  operationId: get_instrument_events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instruments/{instrument_id}/fundamentals\n  method: get\n  operationId: get_instrument_fundamentals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/instruments/{instrument_id}/income-statements\n  method: get\n  operationId: get_instrument_income_statements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market-data/daily-summary\n  method: get\n  operationId: get_daily_summaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market-data/snapshot\n \
  \ method: get\n  operationId: get_snapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/news\n  method: get\n  operationId: get_news\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/omni-ai/entitlement-agreements\n  method: get\n  operationId: get_entitlement_agreements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/omni-ai/entitlements\n  method: get\n  operationId: get_entitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/omni-ai/entitlements\n  method: post\n  operationId: create_entitlements\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/omni-ai/entitlements/{entitlement_id}\n  method: delete\n  operationId: delete_entitlement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/omni-ai/messages/{message_id}\n  method: get\n  operationId: get_message_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/omni-ai/messages/{message_id}/feedback\n  method: post\n  operationId: submit_feedback\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/omni-ai/responses/{response_id}\n  method: get\n  operationId: get_response_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/omni-ai/responses/{response_id}\n  method: delete\n  operationId: cancel_response\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/omni-ai/threads\n  method: get\n  operationId: get_threads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/omni-ai/threads\n  method: post\n  operationId: create_thread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/omni-ai/threads/{thread_id}\n  method: get\n  operationId: get_thread_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/omni-ai/threads/{thread_id}/messages\n  method: get\n  operationId: get_messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/omni-ai/threads/{thread_id}/messages\n  method: post\n  operationId: create_message\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/omni-ai/threads/{thread_id}/response\n  method: get\n  operationId: get_thread_response\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private-markets/companies/{company_id}\n  method: get\n  operationId: get_company_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private-markets/iois\n  method: get\n  operationId: get_iois\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private-markets/iois\n\
  \  method: post\n  operationId: create_ioi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private-markets/iois/{ioi_id}\n  method: delete\n  operationId: delete_ioi\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private-markets/iois/{ioi_id}\n  method: patch\n  operationId: update_ioi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/private-markets/offerings\n  method: get\n  operationId: get_offerings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private-markets/offerings/{offering_id}\n  method: get\n  operationId: get_offering_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/private-markets/spvs/{spv_id}\n  method: get\n  operationId: get_spv_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/saved-screeners\n  method: get\n  operationId: get_screeners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/saved-screeners\n  method: post\n  operationId: create_screener\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/saved-screeners/{screener_id}\n  method: get\n  operationId: get_screener_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/saved-screeners/{screener_id}\n  method: put\n  operationId: replace_screener\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/saved-screeners/{screener_id}\n\
  \  method: delete\n  operationId: delete_screener\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/saved-screeners/{screener_id}\n  method: patch\n  operationId: patch_screener\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/screener\n  method: post\n  operationId: search_screener\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/screener/catalog\n  method: get\n  operationId: get_screener_catalog\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/version\n  method: get\n  operationId: get_version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watchlists\n  method: get\n  operationId: get_watchlists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watchlists\n  method: post\n  operationId: create_watchlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watchlists/{watchlist_id}\n  method: get\n  operationId: get_watchlist_by_id\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watchlists/{watchlist_id}\n  method: delete\n  operationId: delete_watchlist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watchlists/{watchlist_id}/items\n  method: post\n  operationId: add_watchlist_item\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watchlists/{watchlist_id}/items/{item_id}\n  method: delete\n  operationId: delete_watchlist_item\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearstreet8e71/refs/heads/main/agentic-access/clearstreet8e71-agentic-access.yml
summary_line: 72 operations · 26 acting
tags:
- Company
- Fintech
- Brokerage
- Institutional
---
