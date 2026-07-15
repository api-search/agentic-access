---
acting_count: 146
action_class_counts:
  acting: 146
  connected: 155
api_specs:
- filename: trade.yaml
  format: yaml
  label: Saxo Bank OpenAPI
  slug: saxo-bank-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saxo/refs/heads/main/openapi/trade.yaml
consequence_counts:
  physical: 53
  read: 155
  safety-critical: 3
  write: 90
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Saxo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cm/v1/users/resetpasswordrequest
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /port/v1/accounts/{AccountKey}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /trade/v1/optionschain/subscriptions/{ContextId}/{ReferenceId}/ResetATM
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /at/v3/investments/{InvestmentId}/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /at/v3/tradeFollowers/termsandconditions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /at/v3/tradeFollowers/{ClientKey}/suitabilitystatus
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /at/v3/tradeFollowers/{ClientKey}/termsandconditions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /atr/v1/cashmanagement/withdrawals
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /atr/v1/partner/cashtransfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /atr/v1/partner/prebookedfunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /atr/v1/securitiestransfers/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ca/v2/elections
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /ca/v2/elections/bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cs/v2/cashmanagement/interaccounttransfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /port/v1/orders/subscriptions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /port/v1/orders/subscriptions/{ContextId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /port/v1/orders/subscriptions/{ContextId}/{ReferenceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trade/v1/allocationkeys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /trade/v1/allocationkeys/{AllocationKeyId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trade/v1/infoprices/subscriptions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /trade/v1/infoprices/subscriptions/active
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /trade/v1/infoprices/subscriptions/{ContextId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /trade/v1/infoprices/subscriptions/{ContextId}/{ReferenceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /trade/v1/messages/seen
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /trade/v1/messages/seen/{MessageId}
operation_count: 301
overview: 'Saxo Bank exposes 301 API operations that an AI agent could call, of which 146 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 155 read, 90 write, 53 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Saxo Bank
provider_slug: saxo
slug: saxo-agentic-access
source_filename: saxo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/at.yaml, openapi/atr.yaml, openapi/ca.yaml, openapi/chart.yaml, openapi/cm.yaml,\n  openapi/cr.yaml, openapi/cs.yaml, openapi/developer.yaml, openapi/ens.yaml, openapi/hist.yaml,\n  openapi/mkt.yaml, openapi/partnerintegration.yaml, openapi/port.yaml, openapi/ref.yaml, openapi/root.yaml,\n  openapi/trade.yaml, openapi/vas.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 301\n  by_action_class:\n    acting: 146\n    connected: 155\n  by_consequence:\n    write: 90\n    read: 155\n    physical: 53\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /at/v3/investments/subscriptions/suggestions/{ContextId}/{ReferenceId}\n  method: delete\n  operationId: InvestmentsV3DeleteSuggestionSubscription\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /at/v3/investments/subscriptions/{ContextId}/{ReferenceId}\n  method: delete\n  operationId: InvestmentsV3DeleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /at/v3/investments/subscriptions/suggestions\n  method: post\n  operationId: InvestmentsV3AddSuggestionSubscriptionAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /at/v3/investments/subscriptions\n  method: post\n  operationId: InvestmentsV3AddSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /at/v3/investments/summaries\n  method: get\n  operationId: InvestmentsV3GetInvestmentsummariesAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /at/v3/investments/{InvestmentId}/maxWithdrawalAmount\n  method: get\n  operationId: InvestmentsV3GetMaxWithdrawalAmountAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /at/v3/investments/{InvestmentId}/withdraw\n  method: put\n  operationId: InvestmentsV3PutInvestmentAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /at/v3/investments/{InvestmentId}\n  method: patch\n  operationId: InvestmentsV3PatchInvestmentAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /at/v3/investments\n  method: get\n  operationId: InvestmentsV3GetInvestmentByLeader\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /at/v3/investments\n  method: post\n  operationId: InvestmentsV3PostInvestment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /at/v3/investments/me\n  method: get\n  operationId: InvestmentsV3GetInvestments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /at/v3/tradeLeaders/public/customselection/{SelectionId}\n  method: get\n  operationId: TradeLeadersV3GetTradeLeadersCustomSelectionPublic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /at/v3/tradeLeaders/public/{TradeLeaderId}\n\
  \  method: get\n  operationId: TradeLeadersV3GetTradeLeaderPublic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /at/v3/tradeLeaders/public\n  method: get\n  operationId: TradeLeadersV3GetAllTradeLeadersPublic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /at/v3/tradeLeaders/logo/{LogoKey}\n  method: get\n  operationId: TradeLeadersV3GetTradeLeaderLogoByLogoKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /at/v3/tradeLeaders/{TradeLeaderId}/logo\n  method: get\n  operationId: TradeLeadersV3GetTradeLeaderLogo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /at/v3/tradeLeaders/{TradeLeaderId}\n\
  \  method: get\n  operationId: TradeLeadersV3GetTradeLeader\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /at/v3/tradeLeaders\n  method: get\n  operationId: TradeLeadersV3GetAllTradeLeaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /at/v3/tradeFollowers/termsandconditions\n  method: get\n  operationId: GET_TradeFollowerV3GetTermsAndConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /at/v3/tradeFollowers/termsandconditions\n  method: put\n  operationId: TradeFollowerV3UpdateTermsAndConditions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /at/v3/tradeFollowers/{ClientKey}/termsandconditions\n  method: get\n  operationId: TradeFollowerV3GetTermsAndConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /at/v3/tradeFollowers/{ClientKey}/termsandconditions\n  method: put\n  operationId: TradeFollowerV3PutClientTermsAndConditions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /at/v3/tradeFollowers/{ClientKey}/suitabilitystatus\n  method: get\n  operationId:\
  \ TradeFollowerV3GetSuitabilityStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /at/v3/tradeFollowers/{ClientKey}/suitabilitystatus\n  method: put\n  operationId: TradeFollowerV3PutSuitabilityStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /at/v3/tradeFollowers/me\n  method: get\n  operationId: TradeFollowerV3GetTradeFollowers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atr/v1/partner/prebookedfunds\n  method: post\n  operationId: PartnerPrebookFundPrebookFundDeposit\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /atr/v1/cashmanagement/withdrawals\n  method: post\n  operationId: CashWithdrawalWithdrawl\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /atr/v1/cashmanagement/beneficiaryinstructions\n  method: get\n  operationId: BeneficiaryInstructionsGetBeneficiaryInstructionsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /atr/v1/partner/cashtransferlimits/{AccountKey}\n  method: get\n  operationId: PartnerCashTransferLimitGetCashTransfersLimitsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atr/v1/partner/cashtransferlimits\n  method: get\n  operationId: PartnerCashTransferLimitGetCashTransfersLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atr/v1/securitiestransfers/brokers\n  method: get\n  operationId: SecuritiesTransferGetBrokers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atr/v1/securitiestransfers/transfers\n  method: get\n  operationId: SecuritiesTransferGetTransferDetails\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atr/v1/securitiestransfers/transfers\n  method: post\n  operationId: SecuritiesTransferTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /atr/v1/partner/cashtransfers/{TransactionId}\n  method: get\n  operationId: PartnerCashTransferCashTransfersById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atr/v1/partner/cashtransfers\n  method: get\n  operationId: PartnerCashTransferCashTransfersBySearchParameters\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atr/v1/partner/cashtransfers\n  method: post\n  operationId: PartnerCashTransferCashTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /atr/v1/cashmanagement/withdrawallimits/{AccountKey}\n  method: get\n  operationId: CashWithdrawalLimitGetCashWithdrawalLimitsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atr/v1/cashmanagement/withdrawallimits\n  method: get\n  operationId: CashWithdrawalLimitGetCashWithdrawalLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/v2/holdings\n  method: get\n  operationId: HoldingsGetHoldingsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/v2/events/{EventId}\n  method: get\n  operationId: EventsGetEventAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/v2/events\n  method: get\n  operationId: EventsGetEventsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/v2/events/lookupdata\n  method: get\n  operationId: EventsGetLookupDataAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/v1/proxyvoting/events\n\
  \  method: get\n  operationId: ProxyVotingGetProxyVotingEventsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/v2/standinginstructions\n  method: get\n  operationId: StandingInstructionGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ca/v2/standinginstructions\n  method: post\n  operationId: StandingInstructionPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/v2/standinginstructions\n  method: delete\n  operationId: StandingInstructionDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/v2/elections/bulk\n  method: put\n  operationId: ElectionBulkElectAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ca/v2/elections\n  method: put\n  operationId: ElectionElectAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /chart/chart/ClientConfig\n  method: get\n  operationId: ChartGetClientConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chart/chart/{Symbol}\n  method: get\n  operationId: ChartGetChartData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chart/v1/charts/subscriptions/{ContextId}/{ReferenceId}\n  method: delete\n  operationId: ChartsDeleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chart/v1/charts/subscriptions/{ContextId}\n  method: delete\n  operationId: ChartsDeleteSubscriptions\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chart/v1/charts/subscriptions\n  method: post\n  operationId: ChartsAddSubscriptionAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chart/v1/charts/subscriptions/active\n  method: post\n  operationId: ChartsAddSubscriptionActiveAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /chart/v1/charts\n  method: get\n  operationId: ChartsGetChartDataAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cm/v2/signups/verification/initiate/{ClientKey}\n  method: post\n  operationId: SignUpV2InitiateVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cm/v2/signups/options\n  method: get\n  operationId: SignUpV2GetSignupOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cm/v2/signups/attachments/{SignUpId}\n  method: post\n  operationId: SignUpV2AttachFile\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cm/v1/signups/onboardingpdf/{ClientKey}\n  method: get\n  operationId: SignUpV1GenerateTypedOnboardingPDF\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cm/v1/signups/verification/initiate/{ClientKey}\n  method: post\n  operationId: SignUpV1InitiateVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cm/v1/signups/completeapplication/{SignUpId}\n  method: put\n  operationId: SignUpV1CompleteApplication\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cm/v1/signups/status/{ClientKey}\n  method: get\n  operationId: SignUpV1GetSignUpStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cm/v1/signups\n  method: post\n  operationId: SignUpV1SignUp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cm/v1/signups/options\n  method: get\n  operationId: SignUpV1GetSignupOptions\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cm/v1/signups/attachments/{SignUpId}\n  method: post\n  operationId: SignUpV1AttachFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cm/v1/clientrenewals/pending\n  method: get\n  operationId: ClientRenewalGetRenewalStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cm/v1/clientrenewals/{RenewalEntityId}\n  method: patch\n  operationId: ClientRenewalUpdateClientRenewalData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cm/v1/clientrenewals\n  method: get\n  operationId: ClientRenewalGetClientRenewalData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cm/v1/documents\n  method: post\n  operationId: DocumentsUploadDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cm/v2/accounts\n  method: post\n  operationId: AccountsV2CreateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cm/deephealthcheck/isalive\n  method: get\n  operationId: DeepHealthCheckGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cm/v1/users/resetpasswordrequest\n  method: post\n  operationId: UsersResetPasswordResetPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cr/v1/reports/TradesExecuted/{ClientKey}\n  method: get\n  operationId: TradesExecutedGetAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cr/v1/reports/TradeDetails/{ClientKey}\n\
  \  method: get\n  operationId: TradeDetailsGetAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cr/v1/reports/Portfolio/me/{FromDate}/{ToDate}\n  method: get\n  operationId: PortfolioGetMeAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cr/v1/reports/Portfolio/{ClientKey}/{FromDate}/{ToDate}\n  method: get\n  operationId: PortfolioGetAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cr/v1/reports/AccountStatement/{ClientKey}\n  method: get\n  operationId: AccountStatementGetAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cs/v1/tradingconditions/ContractOptionSpaces/{AccountKey}/{OptionRootId}\n\
  \  method: get\n  operationId: ContractOptionGetForContractOption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cs/v2/cashmanagement/interaccounttransfers\n  method: post\n  operationId: InterAccountTransferTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cs/v1/reports/trades/{ClientKey}\n  method: get\n  operationId: TradesGetDetailsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cs/v1/reports/bookings/{ClientKey}\n  method: get\n  operationId: BookingGet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cs/v1/audit/orderactivities\n  method: get\n  operationId: OrderActivitiesGetOrderStatesAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cs/v1/reports/aggregatedAmounts/{ClientKey}/{FromDate}/{ToDate}\n  method: get\n  operationId: AggregatedAmountGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cs/v1/tradingconditions/instrument/{AccountKey}/{Uic}/{AssetType}\n  method: get\n  operationId: InstrumentGetForInstrument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cs/v2/cashmanagement/wiretransfers/instructions\n  method: get\n\
  \  operationId: WireTransferGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cs/v1/tradingconditions/cost/{AccountKey}/{Uic}/{AssetType}\n  method: get\n  operationId: CostGetTradingConditionCost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cs/v2/clientinfo/clients/search\n  method: post\n  operationId: ClientInfoV2Search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cs/v1/reports/closedPositions/{ClientKey}/{FromDate}/{ToDate}\n  method: get\n  operationId: ClosedPositionGet\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cs/v1/partner/support/cases/{CaseId}/note\n  method: post\n  operationId: PartnerSupportCasesCreateNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cs/v1/partner/support/cases/{CaseId}/internalcomment\n  method: post\n  operationId: PartnerSupportCasesCreateInternalComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cs/v1/partner/support/cases/{CaseId}/caseclose\n  method: put\n  operationId: PartnerSupportCasesCloseCase\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cs/v1/partner/support/cases/{CaseId}\n  method: get\n  operationId: PartnerSupportCasesGetCase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cs/v1/partner/support/cases/{CaseId}\n  method: patch\n  operationId: PartnerSupportCasesUpdateNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cs/v1/partner/support/cases\n  method: get\n  operationId: PartnerSupportCasesGetCases\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cs/v1/partner/support/cases\n  method: post\n  operationId: PartnerSupportCasesCreateCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /developer/apps/resource/{AppKey}\n  method: get\n  operationId: DeveloperAppGetResourceByAppKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /developer/apps/{AppKey}\n  method: get\n  operationId: DeveloperAppGetAppByAppKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /developer/apps/{AppKey}\n  method: delete\n  operationId: DeveloperAppDeactivateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /developer/apps/{AppKey}\n  method: patch\n  operationId: DeveloperAppUpdateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /developer/apps\n  method: get\n  operationId: DeveloperAppGetApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /developer/apps\n\
  \  method: post\n  operationId: DeveloperAppCreateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /developer/featureflags\n  method: get\n  operationId: FeatureFlagsGetFlags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /developer/apps/{AppKey}/redirecturis/{RedirectUriId}\n  method: get\n  operationId: DeveloperRedirectGetRedirectUriFromId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /developer/apps/{AppKey}/redirecturis/{RedirectUriId}\n  method: delete\n  operationId: DeveloperRedirectDeleteRedirectUri\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /developer/apps/{AppKey}/redirecturis/{RedirectUriId}\n  method: patch\n  operationId: DeveloperRedirectUpdateRedirectUri\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /developer/apps/{AppKey}/redirecturis\n  method: get\n  operationId: DeveloperRedirectGetRedirectUris\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\n\n# --- truncated at 32 KB (94 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/saxo/refs/heads/main/agentic-access/saxo-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saxo/refs/heads/main/agentic-access/saxo-agentic-access.yml
summary_line: 301 operations · 146 acting · 3 human-in-the-loop
tags:
- Investment Banking
- Trading
- Equities
- Forex
- Options
- Futures
- Market Data
- Portfolio Management
- Orders
- Financial
---
