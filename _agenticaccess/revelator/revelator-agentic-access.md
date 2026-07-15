---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 19
api_specs:
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Distribution API
  slug: revelator-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Catalog API
  slug: revelator-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Analytics API
  slug: revelator-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Royalties & Accounting API
  slug: revelator-royalties-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
- filename: revelator-openapi.yml
  format: yaml
  label: Revelator Payments & Wallet API
  slug: revelator-payments-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/openapi/revelator-openapi.yml
consequence_counts:
  physical: 1
  read: 19
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Revelator Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounting/payee/save
operation_count: 32
overview: 'Revelator exposes 32 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Revelator
provider_slug: revelator
slug: revelator-agentic-access
source_filename: revelator-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/revelator-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    acting: 13\n    connected: 19\n  by_consequence:\n    write: 12\n    read: 19\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /partner/account/signup\n  method: post\n  operationId: partnerAccountSignup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/account/login\n  method: post\n  operationId: partnerAccountLogin\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/account/upgrade\n  method: post\n  operationId: partnerAccountUpgrade\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/login/as\n  method: post\n  operationId: accountLoginAs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/permissions\n\
  \  method: get\n  operationId: getAccountPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enterprise/clients/{enterpriseId}\n  method: get\n  operationId: getEnterpriseClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /distribution/release/{releaseId}/validate\n  method: post\n  operationId: validateRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content/release/retail/save\n  method: post\n  operationId: saveRetailDistributionOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /distribution/release/addtoqueue\n  method: post\n  operationId: addReleaseToQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /distribution/release/all\n  method: get\n  operationId: getAllReleaseDistributionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /distribution/store/all\n  method: get\n  operationId: getStoreDistributionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /distribution/release/takedown\n  method: post\n  operationId: takedownRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/{dataSet}/{aggregationDimension}\n  method: get\n  operationId: getAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/revenue/metricsByDate\n  method: get\n  operationId: getRevenueMetricsByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/{metric}/{aggregation}\n  method: get\n  operationId: getConsumptionAnalytics\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/artificialStreams/{aggregation}\n  method: get\n  operationId: getArtificialStreams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/playlists/byMetadata\n  method: get\n  operationId: getPlaylistAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/contract/save\n  method: post\n  operationId: saveContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounting/contracts\n\
  \  method: get\n  operationId: getContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/contracts/{contractId}\n  method: get\n  operationId: getContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/payee/{payeeId}\n  method: get\n  operationId: getPayee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/payee/save\n  method: post\n  operationId: savePayee\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /integrations/tipalti/generateIframeHashkey\n  method: post\n  operationId: generateTipaltiIframeHashkey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /finance/salereport/all\n  method: get\n  operationId: getSaleReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finance/salereport/{statementId}\n  method: get\n  operationId: getSaleReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finance/salereport/download/summary\n  method: get\n  operationId: downloadStatementSummary\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finance/salereport/download/details\n  method: get\n  operationId: downloadStatementDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finance/salereport/post-download\n  method: post\n  operationId: postDownloadSaleReports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /royaltyTokens\n  method: get\n  operationId: getRoyaltyTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /royaltyTokens\n\
  \  method: post\n  operationId: mintRoyaltyToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /royaltyTokens/{tokenId}\n  method: get\n  operationId: getRoyaltyToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /common/lookup/{type}\n  method: get\n  operationId: getLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revelator/refs/heads/main/agentic-access/revelator-agentic-access.yml
summary_line: 32 operations · 13 acting
tags:
- Music
- Distribution
- Rights
- Royalties
- Payments
- Analytics
---
