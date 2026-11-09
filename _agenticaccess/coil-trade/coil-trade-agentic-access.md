---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 49
api_specs:
- filename: coil-trade-access-keys-api-openapi.yml
  format: yaml
  label: Coil Access & Keys API
  slug: coil-trade-access-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-access-keys-api-openapi.yml
- filename: coil-trade-change-detection-api-openapi.yml
  format: yaml
  label: Coil Change Detection API
  slug: coil-trade-change-detection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-change-detection-api-openapi.yml
- filename: coil-trade-coil-live-api-openapi.yml
  format: yaml
  label: Coil Coil Live API
  slug: coil-trade-coil-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-coil-live-api-openapi.yml
- filename: coil-trade-market-data-api-openapi.yml
  format: yaml
  label: Coil Market Data API
  slug: coil-trade-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-market-data-api-openapi.yml
- filename: coil-trade-paid-reads-api-openapi.yml
  format: yaml
  label: Coil Paid reads API
  slug: coil-trade-paid-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-paid-reads-api-openapi.yml
- filename: coil-trade-research-api-openapi.yml
  format: yaml
  label: Coil Research API
  slug: coil-trade-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-research-api-openapi.yml
- filename: coil-trade-verification-api-openapi.yml
  format: yaml
  label: Coil Verification API
  slug: coil-trade-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coil-trade/openapi/coil-trade-verification-api-openapi.yml
consequence_counts:
  read: 49
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Coil Trade Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 52
overview: 'Coil exposes 52 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 49 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Coil
provider_slug: coil-trade
slug: coil-trade-agentic-access
source_filename: coil-trade-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/coil-trade-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 49\n    acting: 3\n  by_consequence:\n    read: 49\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/board/agent\n  method: get\n  operationId: getBoardAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/free\n  method: get\n  operationId: getBoardFree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/regime\n  method:\
  \ get\n  operationId: getBoardRegime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/buylist\n  method: get\n  operationId: getBoardBuylist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/status\n  method: get\n  operationId: getBoardStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/indices\n  method: get\n  operationId: getBoardIndices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/sectors\n  method: get\n  operationId: getBoardSectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/top-volume\n  method: get\n  operationId: getBoardTopVolume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/name\n  method: get\n  operationId: getBoardName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/leaders\n  method: get\n  operationId: getBoardLeaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/movers\n  method: get\n  operationId: getBoardMovers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/sector\n  method: get\n  operationId:\
  \ getBoardSector\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/symbols\n  method: get\n  operationId: getBoardSymbols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/crypto\n  method: get\n  operationId: getBoardCrypto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/brief\n  method: get\n  operationId: getBoardBrief\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/crypto/gate\n  method: get\n  operationId: getCryptoGate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/board/asof\n  method: get\n  operationId: getBoardAsOf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tradfi-risk\n  method: get\n  operationId: getTradfiRisk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/perf\n  method: get\n  operationId: getEngineRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/proof\n  method: get\n  operationId: getProofLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/key\n  method: post\n  operationId: issueFreeKey\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/board/state\n  method: get\n  operationId: getBoardState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/signal-audit\n  method: get\n  operationId: getSignalAudit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/day\n  method: get\n  operationId: getDayStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/hold\n  method: get\n  operationId: getHoldState\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/diff\n  method: get\n  operationId: getBoardDiff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/crypto/day\n  method: get\n  operationId: getCryptoDayBoard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/crypto/night\n  method: get\n  operationId: getCryptoNightRead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/nonce\n  method: get\n  operationId: getWalletAuthNonce\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/verify\n\
  \  method: post\n  operationId: verifyWalletAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/crypto/setup\n  method: get\n  operationId: getCryptoSetupScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/live/feed\n  method: get\n  operationId: getLiveFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/live/setup\n  method: get\n  operationId: getLiveSetup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/live/rules\n\
  \  method: get\n  operationId: getLiveRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/rotation\n  method: get\n  operationId: getRotation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/whynot\n  method: get\n  operationId: getBoardWhyNot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/board/checktrade\n  method: get\n  operationId: getBoardCheckTrade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/live/session\n  method: get\n  operationId: postLiveSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/live/session\n  method: post\n  operationId: postLiveSessionPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/research\n  method: get\n  operationId: listResearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learn/research/is-chasing-a-strong-stock-a-losing-habit/full\n  method: get\n  operationId: getStudyChaseFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learn/research/does-waiting-for-a-30-minute-pivot-candle-improve-a-stock-entry/full\n\
  \  method: get\n  operationId: getStudyPivotCandleFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learn/research/does-buying-the-opening-range-breakout-on-strong-stocks-make-money/full\n  method: get\n  operationId: getStudyOpeningRangeFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learn/research/does-a-trend-template-and-volatility-contraction-breakout-beat-the-market/full\n  method: get\n  operationId: getStudyTrendTemplateFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learn/research/does-weak-breadth-at-a-market-high-predict-a-worse-stock-market/full\n  method: get\n  operationId: getStudyBreadthAtHighFull\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learn/research/does-buying-a-neglected-stock-after-a-big-volume-gap-up-beat-the-market/full\n  method: get\n  operationId: getStudyGapUpTrailFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learn/research/does-buying-the-laggards-of-a-leading-sector-group-beat-the-market/full\n  method: get\n  operationId: getStudySectorLaggardsFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learn/research/does-buying-a-3x-inverse-index-fund-after-a-gap-down-pay/full\n  method: get\n  operationId: getStudyInverseFundGapFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learn/research/does-buying-a-deeply-oversold-high-volatility-stock-the-next-day-pay/full\n\
  \  method: get\n  operationId: getStudyOversoldReboundFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learn/research/does-buying-a-sector-etf-that-money-is-rotating-into-beat-the-market/full\n  method: get\n  operationId: getStudyPairTurnFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stocks/{symbol}/full\n  method: get\n  operationId: getStockFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /board/{date}/full\n  method: get\n  operationId: getBoardDayFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/coil-trade/agentic-access/coil-trade-agentic-access.yml
summary_line: 52 operations · 3 acting
tags:
- Finance
- Artificial Intelligence
- Stock-Scanner
- Real-Time Data
- Trading
---
