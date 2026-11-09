---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 92
api_specs:
- filename: aspern-org-account-api-openapi.yml
  format: yaml
  label: ASPERN Account API
  slug: aspern-org-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-account-api-openapi.yml
- filename: aspern-org-agents-api-openapi.yml
  format: yaml
  label: ASPERN Agents API
  slug: aspern-org-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-agents-api-openapi.yml
- filename: aspern-org-alerts-api-openapi.yml
  format: yaml
  label: ASPERN Alerts API
  slug: aspern-org-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-alerts-api-openapi.yml
- filename: aspern-org-attestation-api-openapi.yml
  format: yaml
  label: ASPERN Attestation API
  slug: aspern-org-attestation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-attestation-api-openapi.yml
- filename: aspern-org-capital-api-openapi.yml
  format: yaml
  label: ASPERN Capital API
  slug: aspern-org-capital-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-capital-api-openapi.yml
- filename: aspern-org-commerce-api-openapi.yml
  format: yaml
  label: ASPERN Commerce API
  slug: aspern-org-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-commerce-api-openapi.yml
- filename: aspern-org-crowding-api-openapi.yml
  format: yaml
  label: ASPERN Crowding API
  slug: aspern-org-crowding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-crowding-api-openapi.yml
- filename: aspern-org-history-api-openapi.yml
  format: yaml
  label: ASPERN History API
  slug: aspern-org-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-history-api-openapi.yml
- filename: aspern-org-judgement-api-openapi.yml
  format: yaml
  label: ASPERN Judgement API
  slug: aspern-org-judgement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-judgement-api-openapi.yml
- filename: aspern-org-market-api-openapi.yml
  format: yaml
  label: ASPERN Market API
  slug: aspern-org-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-market-api-openapi.yml
- filename: aspern-org-ratings-api-openapi.yml
  format: yaml
  label: ASPERN Ratings API
  slug: aspern-org-ratings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-ratings-api-openapi.yml
- filename: aspern-org-record-api-openapi.yml
  format: yaml
  label: ASPERN Record API
  slug: aspern-org-record-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-record-api-openapi.yml
- filename: aspern-org-reference-api-openapi.yml
  format: yaml
  label: ASPERN Reference API
  slug: aspern-org-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-reference-api-openapi.yml
- filename: aspern-org-risk-api-openapi.yml
  format: yaml
  label: ASPERN Risk API
  slug: aspern-org-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aspern-org/openapi/aspern-org-risk-api-openapi.yml
consequence_counts:
  physical: 2
  read: 92
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aspern Org Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/knock
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payment/inspect
operation_count: 108
overview: 'ASPERN exposes 108 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 92 read, 14 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ASPERN
provider_slug: aspern-org
slug: aspern-org-agentic-access
source_filename: aspern-org-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/aspern-org-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 108\n  by_action_class:\n    connected: 92\n    acting: 16\n  by_consequence:\n    read: 92\n    write: 14\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/vaults\n  method: get\n  operationId: getVaults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/operators/{slug}/check\n  method: get\n  operationId: getOperatorsBySlugCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/vaults/{slug}/check\n  method: get\n  operationId: getVaultsBySlugCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vaults/{slug}\n  method: get\n  operationId: getVaultsBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/operators\n  method: get\n  operationId: getOperators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/operators/{slug}\n  method: get\n  operationId: getOperatorsBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/assets\n  method: get\n  operationId: getAssets\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/index\n  method: get\n  operationId: getIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports/{digest}\n  method: get\n  operationId: getReportsByDigest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/benchmark/{symbol}\n  method: get\n  operationId: getBenchmarkBySymbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dependencies\n  method: get\n  operationId: getDependencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rwa\n  method: get\n  operationId:\
  \ getRwa\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lifecycle\n  method: get\n  operationId: getLifecycle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trading\n  method: get\n  operationId: getTrading\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/revenue\n  method: get\n  operationId: getRevenue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coverage/measures\n  method: get\n  operationId: getCoverageMeasures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /v1/x402/evidence\n  method: get\n  operationId: getX402Evidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/perimeter\n  method: get\n  operationId: getPerimeter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coverage/exit-lifecycle\n  method: get\n  operationId: getCoverageExitLifecycle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/coverage/endpoints\n  method: get\n  operationId: getCoverageEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/freshness\n  method: get\n  operationId: getFreshness\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meta\n  method: get\n  operationId: getMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/platforms\n  method: get\n  operationId: getPlatforms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/risk\n  method: post\n  operationId: postRisk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/stress\n  method: get\n  operationId: getStress\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cascade\n  method: get\n  operationId: getCascade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/correlation\n  method: get\n  operationId: getCorrelation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vaults/{slug}/exits\n  method: get\n  operationId: getVaultsBySlugExits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vaults/{slug}/redemption\n  method: get\n  operationId: getVaultsBySlugRedemption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/changes\n\
  \  method: get\n  operationId: getChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/liquidity\n  method: get\n  operationId: getLiquidity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/liquidity/unmoved\n  method: get\n  operationId: getLiquidityUnmoved\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exposure/netting\n  method: get\n  operationId: getExposureNetting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/operators/{slug}/exposure\n  method: get\n  operationId: getOperatorsBySlugExposure\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vaults/{slug}/waterfall\n  method: get\n  operationId: getVaultsBySlugWaterfall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vaults/{slug}/execution\n  method: get\n  operationId: getVaultsBySlugExecution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vaults/{slug}/trades\n  method: get\n  operationId: getVaultsBySlugTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/forced-exits\n  method: get\n  operationId: getForcedExits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/crowding\n  method: get\n  operationId: getCrowding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/crowding/history\n  method: get\n  operationId: getCrowdingHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/funding\n  method: get\n  operationId: getFunding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/markets\n  method: get\n  operationId: getMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lead-follow\n  method: get\n  operationId: getLeadFollow\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/rails\n  method: get\n  operationId: getAgentsRails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{address}\n  method: get\n  operationId: getAgentsByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{address}/check\n  method: get\n  operationId: getAgentsByAddressCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{address}/profile\n  method: get\n  operationId: getAgentsByAddressProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/service\n  method: get\n  operationId: getService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/identify\n  method: get\n  operationId: getIdentify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/evidence\n  method: get\n  operationId: getEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claim/challenge\n  method: get\n  operationId: getClaimChallenge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claim/verify\n  method: post\n  operationId: postClaimVerify\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/evaluate\n  method: get\n  operationId: getEvaluate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/policies\n  method: get\n  operationId: getPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/dependencies\n  method: post\n  operationId: postAgentsDependencies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/x402/endpoints\n  method: get\n  operationId: getX402Endpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/x402/disagreements\n  method: get\n  operationId: getX402Disagreements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/test-purchase\n  method: get\n  operationId: getTestPurchase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/evidence/regressions\n  method: get\n  operationId: getEvidenceRegressions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/knock\n  method: post\n  operationId: postKnock\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{address}/business\n  method: get\n  operationId: getAgentsByAddressBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exits/screen\n  method: get\n  operationId: getExitsScreen\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vaults/{slug}/exit-confidence\n  method: get\n  operationId: getVaultsBySlugExitConfidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/check-action\n  method: post\n  operationId: postCheckAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/preflight\n  method: get\n  operationId: getPreflight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{address}/history\n  method: get\n  operationId: getAgentsByAddressHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/evaluate/vault-decision\n  method: post\n  operationId: postEvaluateVaultDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/counterparty/bulk\n  method: post\n  operationId: postCounterpartyBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/coverage/capital\n  method: get\n  operationId: getCoverageCapital\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vaults/risk-dimensions\n  method: get\n  operationId: getVaultsRiskDimensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/vaults/earned\n  method: get\n  operationId: getVaultsEarned\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/changes\n  method: get\n  operationId: getAgentsChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/counterparty/agents\n  method: get\n  operationId: getCounterpartyAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/counterparty\n  method: get\n  operationId: getCounterparty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/claims\n  method: get\n  operationId: getAgentsClaims\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/work\n  method: get\n  operationId: getAgentsWork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/delivery\n  method: get\n  operationId: getAgentsDelivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capital/portfolio\n  method: get\n  operationId: getCapitalPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capital/deployment\n  method: get\n  operationId: getCapitalDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/assets/denominations\n  method: get\n  operationId: getAssetsDenominations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/payers\n  method: get\n  operationId: getAgentsPayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resolve\n  method: post\n  operationId: postResolve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vaults/{slug}/due-diligence\n  method: get\n  operationId: getVaultsBySlugDueDiligence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vaults/{slug}/assessment\n  method: get\n  operationId: getVaultsBySlugAssessment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/registry\n  method: post\n  operationId: postRegistry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/registry\n  method: get\n  operationId: getRegistry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/commit\n  method: post\n  operationId: postCommit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reveal\n  method: post\n  operationId: postReveal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/attestation/{digest}\n  method: get\n  operationId: getAttestationByDigest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/openapi.json\n  method: get\n  operationId: getOpenapi.json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/plans\n\
  \  method: get\n  operationId: getPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/populations\n  method: get\n  operationId: getPopulations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lineage\n  method: get\n  operationId: getLineage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/proof\n  method: get\n  operationId: getProof\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/examples\n  method: get\n  operationId: getExamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/checks\n  method: get\n  operationId: getChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/differences\n  method: get\n  operationId: getDifferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/limits\n  method: get\n  operationId: getLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/history/capital\n  method: get\n  operationId: getHistoryCapital\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collateral/{symbol}\n  method: get\n  operationId: getCollateralBySymbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watches\n  method: get\n  operationId: getWatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watches\n  method: put\n  operationId: putWatches\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payment/inspect\n  method: post\n  operationId: postPaymentInspect\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/receipts\n  method: post\n  operationId: postReceipts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/receipts/{id}\n  method: get\n  operationId: getReceiptsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watch/subject\n  method: put\n  operationId: putWatchSubject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watches/{id}\n  method: delete\n  operationId: deleteWatchesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/aspern-org/agentic-access/aspern-org-agentic-access.yml
summary_line: 108 operations · 16 acting
tags:
- Finance
- Blockchain
- Artificial Intelligence
- Data
- Intelligence
---
