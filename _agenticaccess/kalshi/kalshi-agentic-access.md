---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 67
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Kalshi Trade API (REST)
  slug: trade-api
  spec_type: OpenAPI
  url: https://docs.kalshi.com/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Kalshi Trade API (external-api host)
  slug: trade-api-external
  spec_type: OpenAPI
  url: https://docs.kalshi.com/openapi.yaml
- filename: asyncapi.yaml
  format: yaml
  label: Kalshi WebSocket Streaming API
  slug: websocket
  spec_type: AsyncAPI
  url: https://docs.kalshi.com/asyncapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Kalshi OpenAPI Specification
  slug: openapi
  spec_type: OpenAPI
  url: https://docs.kalshi.com/openapi.yaml
- filename: asyncapi.yaml
  format: yaml
  label: Kalshi AsyncAPI Specification
  slug: asyncapi
  spec_type: AsyncAPI
  url: https://docs.kalshi.com/asyncapi.yaml
consequence_counts:
  physical: 17
  read: 67
  safety-critical: 1
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Kalshi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /portfolio/order_groups/{order_group_id}/reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portfolio/events/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portfolio/events/orders/batched
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /portfolio/events/orders/batched
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /portfolio/events/orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portfolio/events/orders/{order_id}/amend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portfolio/events/orders/{order_id}/decrease
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portfolio/order_groups/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /portfolio/order_groups/{order_group_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /portfolio/order_groups/{order_group_id}/limit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /portfolio/order_groups/{order_group_id}/trigger
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portfolio/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portfolio/orders/batched
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /portfolio/orders/batched
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /portfolio/orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portfolio/orders/{order_id}/amend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portfolio/orders/{order_id}/decrease
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portfolio/subaccounts/transfer
operation_count: 98
overview: 'Kalshi exposes 98 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 67 read, 13 write, 17 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kalshi
provider_slug: kalshi
slug: kalshi-agentic-access
source_filename: kalshi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kalshi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 98\n  by_action_class:\n    connected: 67\n    acting: 31\n  by_consequence:\n    read: 67\n    physical: 17\n    safety-critical: 1\n    write: 13\n  human_in_the_loop_required: 1\noperations:\n- path: /exchange/status\n  method: get\n  operationId: GetExchangeStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/announcements\n  method: get\n  operationId: GetExchangeAnnouncements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /series/fee_changes\n  method: get\n  operationId: GetSeriesFeeChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/schedule\n  method: get\n  operationId: GetExchangeSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange/user_data_timestamp\n  method: get\n  operationId: GetUserDataTimestamp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /series/{series_ticker}/markets/{ticker}/candlesticks\n  method: get\n  operationId: GetMarketCandlesticks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/trades\n\
  \  method: get\n  operationId: GetTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{ticker}/orderbook\n  method: get\n  operationId: GetMarketOrderbook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/orderbooks\n  method: get\n  operationId: GetMarketOrderbooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /series/{series_ticker}\n  method: get\n  operationId: GetSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /series\n  method: get\n  operationId: GetSeriesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets\n  method: get\n  operationId: GetMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/{ticker}\n  method: get\n  operationId: GetMarket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /markets/candlesticks\n  method: get\n  operationId: BatchGetMarketCandlesticks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /series/{series_ticker}/events/{ticker}/candlesticks\n  method: get\n  operationId: GetMarketCandlesticksByEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /events\n  method: get\n  operationId: GetEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/multivariate\n  method: get\n  operationId: GetMultivariateEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_ticker}\n  method: get\n  operationId: GetEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_ticker}/metadata\n  method: get\n  operationId: GetEventMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /series/{series_ticker}/events/{ticker}/forecast_percentile_history\n  method: get\n  operationId: GetEventForecastPercentilesHistory\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/orders\n  method: get\n  operationId: GetOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/orders\n  method: post\n  operationId: CreateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/orders/{order_id}\n  method: get\n  operationId: GetOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/orders/{order_id}\n\
  \  method: delete\n  operationId: CancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/orders/batched\n  method: post\n  operationId: BatchCreateOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/orders/batched\n  method: delete\n  operationId: BatchCancelOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/orders/{order_id}/amend\n  method: post\n  operationId: AmendOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/orders/{order_id}/decrease\n  method: post\n  operationId: DecreaseOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/orders/queue_positions\n  method: get\n  operationId: GetOrderQueuePositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/orders/{order_id}/queue_position\n  method: get\n  operationId: GetOrderQueuePosition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/events/orders\n  method: post\n  operationId: CreateOrderV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/events/orders/batched\n\
  \  method: post\n  operationId: BatchCreateOrdersV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/events/orders/batched\n  method: delete\n  operationId: BatchCancelOrdersV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/events/orders/{order_id}\n  method: delete\n  operationId: CancelOrderV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/events/orders/{order_id}/amend\n  method: post\n  operationId: AmendOrderV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/events/orders/{order_id}/decrease\n  method: post\n  operationId: DecreaseOrderV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/order_groups\n  method: get\n  operationId: GetOrderGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/order_groups/create\n  method: post\n  operationId: CreateOrderGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/order_groups/{order_group_id}\n  method: get\n  operationId: GetOrderGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/order_groups/{order_group_id}\n\
  \  method: delete\n  operationId: DeleteOrderGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/order_groups/{order_group_id}/reset\n  method: put\n  operationId: ResetOrderGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /portfolio/order_groups/{order_group_id}/trigger\n  method: put\n  operationId: TriggerOrderGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/order_groups/{order_group_id}/limit\n  method: put\n  operationId: UpdateOrderGroupLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/balance\n  method: get\n  operationId: GetBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/subaccounts\n  method: post\n  operationId: CreateSubaccount\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/subaccounts/transfer\n  method: post\n  operationId: ApplySubaccountTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/subaccounts/balances\n  method: get\n  operationId: GetSubaccountBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/subaccounts/transfers\n  method: get\n  operationId: GetSubaccountTransfers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/subaccounts/netting\n  method: put\n  operationId: UpdateSubaccountNetting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portfolio/subaccounts/netting\n  method: get\n  operationId: GetSubaccountNetting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/positions\n  method: get\n  operationId: GetPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/settlements\n\
  \  method: get\n  operationId: GetSettlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/deposits\n  method: get\n  operationId: GetDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/withdrawals\n  method: get\n  operationId: GetWithdrawals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/summary/total_resting_order_value\n  method: get\n  operationId: GetPortfolioRestingOrderTotalValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portfolio/fills\n  method: get\n  operationId: GetFills\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /communications/id\n  method: get\n  operationId: GetCommunicationsID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /communications/rfqs\n  method: get\n  operationId: GetRFQs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /communications/rfqs\n  method: post\n  operationId: CreateRFQ\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /communications/rfqs/{rfq_id}\n  method: get\n  operationId: GetRFQ\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /communications/rfqs/{rfq_id}\n  method: delete\n  operationId: DeleteRFQ\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /communications/quotes\n  method: get\n  operationId: GetQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /communications/quotes\n  method: post\n  operationId: CreateQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /communications/quotes/{quote_id}\n  method: get\n  operationId: GetQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /communications/quotes/{quote_id}\n  method: delete\n  operationId: DeleteQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /communications/quotes/{quote_id}/accept\n  method: put\n  operationId: AcceptQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /communications/quotes/{quote_id}/confirm\n  method: put\n  operationId: ConfirmQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_keys\n  method: get\n  operationId: GetApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api_keys\n  method: post\n  operationId: CreateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_keys/generate\n  method: post\n  operationId:\
  \ GenerateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api_keys/{api_key}\n  method: delete\n  operationId: DeleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/limits\n  method: get\n  operationId: GetAccountApiLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/endpoint_costs\n  method: get\n  operationId: GetAccountEndpointCosts\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/tags_by_categories\n  method: get\n  operationId: GetTagsForSeriesCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/filters_by_sport\n  method: get\n  operationId: GetFiltersForSports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live_data/milestone/{milestone_id}\n  method: get\n  operationId: GetLiveDataByMilestone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live_data/{type}/milestone/{milestone_id}\n  method: get\n  operationId: GetLiveData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /live_data/batch\n  method: get\n  operationId: GetLiveDatas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live_data/milestone/{milestone_id}/game_stats\n  method: get\n  operationId: GetGameStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /structured_targets\n  method: get\n  operationId: GetStructuredTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /structured_targets/{structured_target_id}\n  method: get\n  operationId: GetStructuredTarget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /milestones/{milestone_id}\n\
  \  method: get\n  operationId: GetMilestone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /milestones\n  method: get\n  operationId: GetMilestones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /multivariate_event_collections/{collection_ticker}\n  method: get\n  operationId: GetMultivariateEventCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /multivariate_event_collections/{collection_ticker}\n  method: post\n  operationId: CreateMarketInMultivariateEventCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /multivariate_event_collections\n  method: get\n  operationId: GetMultivariateEventCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /multivariate_event_collections/{collection_ticker}/lookup\n  method: put\n  operationId: LookupTickersForMarketInMultivariateEventCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /multivariate_event_collections/{collection_ticker}/lookup\n  method: get\n  operationId: GetMultivariateEventCollectionLookupHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /incentive_programs\n  method: get\n  operationId: GetIncentivePrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fcm/orders\n  method: get\n  operationId: GetFCMOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fcm/positions\n  method: get\n  operationId: GetFCMPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical/cutoff\n  method: get\n  operationId: GetHistoricalCutoff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical/markets/{ticker}/candlesticks\n  method: get\n  operationId:\
  \ GetMarketCandlesticksHistorical\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical/fills\n  method: get\n  operationId: GetFillsHistorical\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical/orders\n  method: get\n  operationId: GetHistoricalOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical/trades\n  method: get\n  operationId: GetTradesHistorical\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical/markets\n  method: get\n  operationId: GetHistoricalMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /historical/markets/{ticker}\n  method: get\n  operationId: GetHistoricalMarket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/agentic-access/kalshi-agentic-access.yml
summary_line: 98 operations · 31 acting · 1 human-in-the-loop
tags:
- Prediction Markets
- Event Contracts
- Exchange
- CFTC
- Trading
- Markets
---
