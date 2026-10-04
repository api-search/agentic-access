---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 44
api_specs:
- filename: farmdash-account-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Account API
  slug: farmdash-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-account-api-openapi.yml
- filename: farmdash-autopilot-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Autopilot API
  slug: farmdash-autopilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-autopilot-api-openapi.yml
- filename: farmdash-delegation-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Delegation API
  slug: farmdash-delegation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-delegation-api-openapi.yml
- filename: farmdash-execution-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Execution API
  slug: farmdash-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-execution-api-openapi.yml
- filename: farmdash-executionauthority-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Execution Authority API
  slug: farmdash-executionauthority-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-executionauthority-api-openapi.yml
- filename: farmdash-history-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub History API
  slug: farmdash-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-history-api-openapi.yml
- filename: farmdash-intelligence-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Intelligence API
  slug: farmdash-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-intelligence-api-openapi.yml
- filename: farmdash-planning-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Planning API
  slug: farmdash-planning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-planning-api-openapi.yml
- filename: farmdash-proof-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Proof API
  slug: farmdash-proof-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-proof-api-openapi.yml
- filename: farmdash-reputation-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Reputation API
  slug: farmdash-reputation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-reputation-api-openapi.yml
- filename: farmdash-research-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Research API
  slug: farmdash-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-research-api-openapi.yml
- filename: farmdash-risk-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Risk API
  slug: farmdash-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-risk-api-openapi.yml
- filename: farmdash-session-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Session API
  slug: farmdash-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-session-api-openapi.yml
- filename: farmdash-strategy-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Strategy API
  slug: farmdash-strategy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-strategy-api-openapi.yml
- filename: farmdash-swap-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Swap API
  slug: farmdash-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-swap-api-openapi.yml
- filename: farmdash-wallet-api-openapi.yml
  format: yaml
  label: FarmDash Agent Hub Wallet API
  slug: farmdash-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/openapi/farmdash-wallet-api-openapi.yml
consequence_counts:
  physical: 4
  read: 44
  safety-critical: 2
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Farmdash Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/agent/authority
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/agent/receipts/share
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/agent/futures/cancel-order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/agent/futures/cancel-order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/agent/futures/execute-order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/agent/futures/execute-order
operation_count: 73
overview: 'FarmDash Agent Hub exposes 73 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 44 read, 23 write, 4 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FarmDash Agent Hub
provider_slug: farmdash
slug: farmdash-agentic-access
source_filename: farmdash-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: generated\nsource: openapi/farmdash-account-api-openapi.yml, openapi/farmdash-autopilot-api-openapi.yml,\n  openapi/farmdash-delegation-api-openapi.yml, openapi/farmdash-execution-api-openapi.yml, openapi/farmdash-history-api-openapi.yml,\n  openapi/farmdash-intelligence-api-openapi.yml, openapi/farmdash-openapi.yaml, openapi/farmdash-research-api-openapi.yml,\n  openapi/farmdash-risk-api-openapi.yml, openapi/farmdash-session-api-openapi.yml, openapi/farmdash-strategy-api-openapi.yml,\n  openapi/farmdash-swap-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 73\n  by_action_class:\n    connected: 44\n    acting: 29\n  by_consequence:\n    read: 44\n    write: 23\n    physical: 4\n    safety-critical:\
  \ 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/agent/futures/account-state\n  method: get\n  operationId: getAccountState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/autopilot\n  method: get\n  operationId: getRecommendedAutopilotConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/autopilot\n  method: post\n  operationId: manageAutopilot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/delegation\n  method: get\n  operationId: getDelegationStatus\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/delegation\n  method: post\n  operationId: verifyDelegation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/futures/execute-order\n  method: post\n  operationId: executeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/futures/cancel-order\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/history\n  method: get\n  operationId: getSwapHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/status\n  method: get\n  operationId: getAgentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/protocols\n  method: get\n  operationId: getProtocolCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trail-heat\n  method: get\n  operationId:\
  \ getLiveTrailHeat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/prices\n  method: get\n  operationId: getTokenPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/workflows\n  method: get\n  operationId: listAgentWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/chain-breakdown\n  method: get\n  operationId: getChainBreakdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/status\n  method: get\n  operationId: getPublicSystemStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/billing-history\n  method: get\n  operationId: getBillingHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/status\n  method: get\n  operationId: getAgentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/quote\n  method: get\n  operationId: getSwapQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/market-estimate\n  method: get\n  operationId: getMarketEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/quote-intent\n  method: post\n  operationId:\
  \ createQuoteIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/solana-quote\n  method: get\n  operationId: getSolanaQuotePreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/simulate\n  method: post\n  operationId: simulateSwapExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/swap\n  method: post\n  operationId: executeSwap\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/confirm\n  method: post\n  operationId: confirmSwap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/history\n  method: get\n  operationId: getSwapHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/reputation\n  method: get\n  operationId: getAgentReputation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/agent/leaderboard\n  method: get\n  operationId: getLeaderboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/balances\n  method: get\n  operationId: getWalletBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/performance\n  method: get\n  operationId: getAgentPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/sybil-audit\n  method: get\n  operationId: getSybilAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/simulate-points\n  method: post\n  operationId: simulatePoints\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/optimize-portfolio\n  method: post\n  operationId: optimizePortfolio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/protocols\n  method: get\n  operationId: getProtocolCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trail-heat\n  method: get\n  operationId: getLiveTrailHeat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/prices\n  method: get\n  operationId: getTokenPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/workflows\n  method: get\n  operationId: listAgentWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/chain-breakdown\n  method: get\n  operationId: getChainBreakdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/futures/scan-funding\n  method: get\n  operationId: scanFundingRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/futures/market-conditions\n\
  \  method: get\n  operationId: getMarketConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/futures/account-state\n  method: get\n  operationId: getAccountState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/futures/analyze-strategy\n  method: post\n  operationId: analyzeStrategy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/futures/position-sizing\n  method: post\n  operationId: calculatePositionSize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/futures/execute-order\n  method: post\n  operationId: executeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/futures/cancel-order\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/agent/onboard\n  method: get\n  operationId: getOnboardingGuide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/authority\n  method: get\n  operationId: getExecutionAuthority\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/authority\n  method: post\n  operationId: manageExecutionAuthority\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agent/session\n  method: get\n  operationId: findSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/session\n  method: post\n  operationId: manageSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/delegation\n  method: get\n  operationId: getDelegationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/delegation\n  method: post\n  operationId: verifyDelegation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/agent/autopilot\n  method: get\n  operationId: getRecommendedAutopilotConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/autopilot\n  method: post\n  operationId: manageAutopilot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/risk-sentinel\n  method: get\n  operationId: getRiskSentinelInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/risk-sentinel\n  method: post\n  operationId: analyzeRiskSentinel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/receipts/share\n  method: post\n  operationId: createReceiptShare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/receipts/share\n  method: delete\n  operationId: revokeReceiptShare\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /r/{token}\n  method: get\n  operationId: resolveReceiptShare\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/farmdash-receipt-key.json\n  method: get\n  operationId: getReceiptProofKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/futures/scan-funding\n  method: get\n  operationId: scanFundingRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/futures/market-conditions\n  method: get\n  operationId: getMarketConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/simulate\n  method: post\n  operationId: simulateSwapExecution\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/risk-sentinel\n  method: get\n  operationId: getRiskSentinelInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/risk-sentinel\n  method: post\n  operationId: analyzeRiskSentinel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/onboard\n  method: get\n  operationId: getOnboardingGuide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/agent/session\n  method: get\n  operationId: findSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/session\n  method: post\n  operationId: manageSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/futures/analyze-strategy\n  method: post\n  operationId: analyzeStrategy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/futures/position-sizing\n\
  \  method: post\n  operationId: calculatePositionSize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/quote\n  method: get\n  operationId: getSwapQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/simulate\n  method: post\n  operationId: simulateSwapExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/swap\n  method: post\n  operationId: executeSwap\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/confirm\n  method: post\n  operationId: confirmSwap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmdash/refs/heads/main/agentic-access/farmdash-agentic-access.yml
summary_line: 73 operations · 29 acting · 2 human-in-the-loop
tags:
- DeFi
- DeFAI
- AI Agents
- MCP
- OpenAPI
- x402
- Blockchain
- Crypto
- airdrop tracking
- Developer Tools
- Agent Readiness
- Machine Payments
- Hyperliquid
- Wallet Intelligence
- zero custody
- A2A
---
