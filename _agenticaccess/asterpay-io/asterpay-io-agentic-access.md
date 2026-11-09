---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 57
api_specs:
- filename: asterpay-io-ai-api-openapi.yml
  format: yaml
  label: AsterPay AI API
  slug: asterpay-io-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-ai-api-openapi.yml
- filename: asterpay-io-crypto-api-openapi.yml
  format: yaml
  label: AsterPay Crypto API
  slug: asterpay-io-crypto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-crypto-api-openapi.yml
- filename: asterpay-io-data-api-openapi.yml
  format: yaml
  label: AsterPay Data API
  slug: asterpay-io-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-data-api-openapi.yml
- filename: asterpay-io-discovery-api-openapi.yml
  format: yaml
  label: AsterPay Discovery API
  slug: asterpay-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-discovery-api-openapi.yml
- filename: asterpay-io-market-api-openapi.yml
  format: yaml
  label: AsterPay Market API
  slug: asterpay-io-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-market-api-openapi.yml
- filename: asterpay-io-sessions-api-openapi.yml
  format: yaml
  label: AsterPay Sessions API
  slug: asterpay-io-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-sessions-api-openapi.yml
- filename: asterpay-io-settlement-api-openapi.yml
  format: yaml
  label: AsterPay Settlement API
  slug: asterpay-io-settlement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-settlement-api-openapi.yml
- filename: asterpay-io-trust-api-openapi.yml
  format: yaml
  label: AsterPay Trust API
  slug: asterpay-io-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-trust-api-openapi.yml
- filename: asterpay-io-utility-api-openapi.yml
  format: yaml
  label: AsterPay Utility API
  slug: asterpay-io-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asterpay-io/openapi/asterpay-io-utility-api-openapi.yml
consequence_counts:
  physical: 1
  read: 57
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Asterpay Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/mpe/merchants/resolve
operation_count: 68
overview: 'AsterPay exposes 68 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 57 read, 10 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AsterPay
provider_slug: asterpay-io
slug: asterpay-io-agentic-access
source_filename: asterpay-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/asterpay-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 68\n  by_action_class:\n    connected: 57\n    acting: 11\n  by_consequence:\n    read: 57\n    write: 10\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/agent/deep-analysis/{address}\n  method: get\n  operationId: getDeepAnalysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/trust-score/{address}\n  method: get\n  operationId: getAgentTrustScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/agent/verify/{address}\n  method: get\n  operationId: verifyAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/tier/{address}\n  method: get\n  operationId: getAgentTier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/settlement/estimate\n  method: get\n  operationId: getSettlementEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/discovery\n  method: get\n  operationId: getAgentDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/x402/market/rates\n  method: get\n  operationId: getMarketRates\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/deep-analysis/batch\n  method: post\n  operationId: batchDeepAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/market/price/{symbol}\n  method: get\n  operationId: getMarketPrice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/ohlcv/{symbol}\n  method: get\n  operationId: getOhlcv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/trending\n  method:\
  \ get\n  operationId: getTrending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/x402/crypto/prices\n  method: get\n  operationId: getCryptoPrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/x402/offramp/estimate\n  method: get\n  operationId: offrampEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/x402/agent-readiness\n  method: get\n  operationId: agentReadinessScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ai/summarize\n  method: post\n  operationId: aiSummarize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/sentiment\n  method: post\n  operationId: aiSentiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/translate\n  method: post\n  operationId: aiTranslate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/code-review\n  method: post\n  operationId: aiCodeReview\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ai/fact-check\n  method: post\n  operationId: aiFactCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/x402/ai/fact-check\n  method: post\n  operationId: aiFactCheckX402\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/x402/ai/fact-check/deep\n  method: post\n \
  \ operationId: aiFactCheckDeep\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/x402/ai/sentiment\n  method: post\n  operationId: aiMarketSentiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/crypto/wallet-score/{address}\n  method: get\n  operationId: getWalletScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/crypto/token-analysis/{address}\n  method: get\n  operationId: getTokenAnalysis\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/crypto/whale-alerts\n  method: get\n  operationId: getWhaleAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/packages\n  method: get\n  operationId: getSessionPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mpe/merchants/resolve\n  method: get\n  operationId: resolveMerchantGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mpe/merchants/resolve\n  method: post\n  operationId: resolveMerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/util/qr-code\n  method: post\n  operationId: generateQrCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/data/fx/ecb\n  method: get\n  operationId: data_fx_ecb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/fx/pair/{base}/{quote}\n  method: get\n  operationId: data_fx_pair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/data/energy/oil\n  method: get\n  operationId: data_energy_oil\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/energy/natgas\n  method: get\n  operationId: data_energy_natgas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/energy/us-grid\n  method: get\n  operationId: data_energy_us_grid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/energy/crude-imports\n  method: get\n  operationId: data_energy_crude_imports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/energy/nuclear-outages\n  method: get\n  operationId:\
  \ data_energy_nuclear_outages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/energy/steo-forecast\n  method: get\n  operationId: data_energy_steo_forecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/energy/us-energy-overview\n  method: get\n  operationId: data_energy_us_energy_overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/energy/electricity-retail/{state}\n  method: get\n  operationId: data_energy_electricity_retail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/macro/us-debt\n  method: get\n  operationId: data_macro_us_debt\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/macro/inflation/{region}\n  method: get\n  operationId: data_macro_inflation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/macro/rates\n  method: get\n  operationId: data_macro_rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/macro/recession\n  method: get\n  operationId: data_macro_recession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/macro/bank-failures\n  method: get\n  operationId: data_macro_bank_failures\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/stablecoins/supply\n  method: get\n  operationId: data_stablecoins_supply\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/stablecoins/peg\n  method: get\n  operationId: data_stablecoins_peg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/crypto/fear-greed\n  method: get\n  operationId: data_crypto_fear_greed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/crypto/hacks\n  method: get\n  operationId: data_crypto_hacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /v1/data/security/cve-critical\n  method: get\n  operationId: data_security_cve_critical\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/security/kev\n  method: get\n  operationId: data_security_kev\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/security/ransomware\n  method: get\n  operationId: data_security_ransomware\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/company/vat/{vatId}\n  method: get\n  operationId: data_company_vat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/company/verify/{vatId}\n \
  \ method: get\n  operationId: data_company_verify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/company/profile/{country}/{id}\n  method: get\n  operationId: data_company_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/company/signals/{country}/{id}\n  method: get\n  operationId: data_company_signals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/company/due-diligence/{vatId}\n  method: get\n  operationId: data_company_due_diligence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/tenders/eu/{country}/{cpv}\n  method: get\n\
  \  operationId: data_tenders_eu\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/risk/agi\n  method: get\n  operationId: data_risk_agi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/risk/ai-extinction\n  method: get\n  operationId: data_risk_ai_extinction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/risk/doomsday-clock\n  method: get\n  operationId: data_risk_doomsday_clock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/risk/asteroids\n  method: get\n  operationId: data_risk_asteroids\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/risk/space-weather\n  method: get\n  operationId: data_risk_space_weather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/risk/earthquakes\n  method: get\n  operationId: data_risk_earthquakes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/risk/outbreaks\n  method: get\n  operationId: data_risk_outbreaks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/risk/climate\n  method: get\n  operationId: data_risk_climate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/data/risk/markets\n  method: get\n  operationId: data_risk_markets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data/risk/board\n  method: get\n  operationId: data_risk_board\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data\n  method: get\n  operationId: data_catalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/asterpay-io/agentic-access/asterpay-io-agentic-access.yml
summary_line: 68 operations · 11 acting
tags:
- Payments
- Fintech
- Artificial Intelligence
- EUR
- Settlement
---
