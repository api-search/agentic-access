---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 85
api_specs:
- filename: propraven-com-account-api-openapi.yml
  format: yaml
  label: propraven-com Account API
  slug: propraven-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-account-api-openapi.yml
- filename: propraven-com-coverage-api-openapi.yml
  format: yaml
  label: propraven-com Coverage API
  slug: propraven-com-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-coverage-api-openapi.yml
- filename: propraven-com-credits-api-openapi.yml
  format: yaml
  label: propraven-com Credits API
  slug: propraven-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-credits-api-openapi.yml
- filename: propraven-com-deals-api-openapi.yml
  format: yaml
  label: propraven-com Deals API
  slug: propraven-com-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-deals-api-openapi.yml
- filename: propraven-com-distribution-api-openapi.yml
  format: yaml
  label: propraven-com Distribution API
  slug: propraven-com-distribution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-distribution-api-openapi.yml
- filename: propraven-com-leads-api-openapi.yml
  format: yaml
  label: propraven-com Leads API
  slug: propraven-com-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-leads-api-openapi.yml
- filename: propraven-com-market-api-openapi.yml
  format: yaml
  label: propraven-com Market API
  slug: propraven-com-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-market-api-openapi.yml
- filename: propraven-com-owners-api-openapi.yml
  format: yaml
  label: propraven-com Owners API
  slug: propraven-com-owners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-owners-api-openapi.yml
- filename: propraven-com-parcels-api-openapi.yml
  format: yaml
  label: propraven-com Parcels API
  slug: propraven-com-parcels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-parcels-api-openapi.yml
- filename: propraven-com-property-intelligence-api-openapi.yml
  format: yaml
  label: propraven-com Property Intelligence API
  slug: propraven-com-property-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-property-intelligence-api-openapi.yml
- filename: propraven-com-search-api-openapi.yml
  format: yaml
  label: propraven-com Search API
  slug: propraven-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-search-api-openapi.yml
- filename: propraven-com-storefront-api-openapi.yml
  format: yaml
  label: propraven-com Storefront API
  slug: propraven-com-storefront-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-storefront-api-openapi.yml
- filename: propraven-com-verify-api-openapi.yml
  format: yaml
  label: propraven-com Verify API
  slug: propraven-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-verify-api-openapi.yml
- filename: propraven-com-watch-api-openapi.yml
  format: yaml
  label: propraven-com Watch API
  slug: propraven-com-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-watch-api-openapi.yml
- filename: propraven-com-webhooks-api-openapi.yml
  format: yaml
  label: propraven-com Webhooks API
  slug: propraven-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-webhooks-api-openapi.yml
- filename: propraven-com-zoning-api-openapi.yml
  format: yaml
  label: propraven-com Zoning API
  slug: propraven-com-zoning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/propraven-com/openapi/propraven-com-zoning-api-openapi.yml
consequence_counts:
  read: 85
  safety-critical: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Propraven Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/webhooks/{id}
operation_count: 92
overview: 'propraven-com exposes 92 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 85 read, 6 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: propraven-com
provider_slug: propraven-com
slug: propraven-com-agentic-access
source_filename: propraven-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/propraven-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 92\n  by_action_class:\n    connected: 85\n    acting: 7\n  by_consequence:\n    read: 85\n    write: 6\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/parcels/{id}/assessment-history\n  method: get\n  operationId: getParcelAssessmentHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}\n  method: get\n  operationId: getParcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/parcels/{id}/owner\n  method: get\n  operationId: getParcelOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/permits\n  method: get\n  operationId: getParcelPermits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/deeds\n  method: get\n  operationId: getParcelDeeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/risks\n  method: get\n  operationId: getParcelRisks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/tax-status\n  method: get\n  operationId:\
  \ getParcelTaxStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method: post\n  operationId: searchParcels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coverage\n  method: get\n  operationId: getCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/deals/absentee\n  method: get\n  operationId: getAbsenteeOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/deals/flips\n  method: get\n  operationId: getFlips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/counties\n  method: get\n  operationId: getCountyMarketStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/trends\n  method: get\n  operationId: getMarketTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/owners/search\n  method: get\n  operationId: searchOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/owners/{name}\n  method: get\n  operationId: getOwnerProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/owners/{name}/properties\n  method: get\n  operationId:\
  \ getOwnerProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/owners/{name}/portfolio\n  method: get\n  operationId: getOwnerPortfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/owners/{name}/report\n  method: get\n  operationId: buyOwnerReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/deals/contractors\n  method: get\n  operationId: searchContractors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/deals/entities\n  method: get\n  operationId: searchEntityOwnedParcels\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/deals/high-land-ratio\n  method: get\n  operationId: getHighLandRatioParcels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/deals/lenders\n  method: get\n  operationId: searchLenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/deals/long-hold\n  method: get\n  operationId: getLongHoldParcels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/deals/market\n  method: get\n  operationId: getDealMarketSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/deals/portfolio-owners\n  method: get\n  operationId: getPortfolioOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/webhooks/{id}/deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search/autocomplete\n  method: get\n  operationId: searchAutocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search/export\n  method: get\n  operationId: exportSearchResults\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search/full\n  method: get\n  operationId: fullSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/geojson\n  method: get\n  operationId: getParcelGeoJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/report\n  method: get\n  operationId: getParcelReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/comp-pack\n  method: get\n  operationId: buyCompPack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/parcels/{id}/risk-score\n  method: get\n  operationId: buyRiskScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/traffic-history\n  method: get\n  operationId: getParcelTrafficHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/counties/{fips}\n  method: get\n  operationId: getCountyDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/flips\n  method: get\n  operationId: getMarketFlips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/owners/{name}/transactions\n\
  \  method: get\n  operationId: getOwnerTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/usage\n  method: get\n  operationId: getAccountUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/storefront/catalog\n  method: get\n  operationId: getStorefrontCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/storefront/availability\n  method: get\n  operationId: getStorefrontAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/leads/find\n  method: get\n  operationId: findLeads\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/storefront/credits/topup\n  method: get\n  operationId: fundCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/storefront/credits/balance\n  method: get\n  operationId: creditBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/watch\n  method: get\n  operationId: listWatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/watch\n  method: post\n  operationId: createWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/watch/{id}\n  method: get\n  operationId: pollWatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/watch/{id}\n  method: delete\n  operationId: deleteWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/verify\n  method: post\n  operationId: verifyFactsBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/verify\n  method: get\n  operationId: verifyFactsSingle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/owners/card\n  method: get\n  operationId: getOwnerCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/owners/pierce\n  method: get\n  operationId: getOwnerPierce\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cohorts/{id}/export\n  method: get\n  operationId: exportListMailMerge\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lookup\n  method: get\n  operationId: lookupParcel\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/lookup/batch\n  method: post\n  operationId: lookupBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/batch\n  method: post\n  operationId: getParcelsBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/comps\n  method: get\n  operationId: getParcelComps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/occupants\n  method: get\n  operationId: getParcelOccupants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/violations\n  method: get\n  operationId: getParcelViolations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/poi\n  method: get\n  operationId: getParcelPois\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/snapshot\n  method: get\n  operationId: getMarketSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cmbs/exposure\n  method: get\n  operationId: getCmbsExposure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/freshness\n  method: get\n\
  \  operationId: getFreshness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/freshness/datasets\n  method: get\n  operationId: getFreshnessDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coverage/map\n  method: get\n  operationId: getCoverageMap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/crime/lookup\n  method: get\n  operationId: getCrimeLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/traffic/stations\n  method: get\n  operationId: getTrafficStations\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/{id}/deliveries/{deliveryId}/retry\n  method: post\n  operationId: retryWebhookDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/cohorts\n  method: get\n  operationId: listCohorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/licensees/firms\n  method: get\n  operationId: searchLicenseeFirms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/licensees/individuals\n  method: get\n  operationId: searchLicenseeIndividuals\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/signals\n  method: get\n  operationId: getPropertySignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/intelligence/runs/{runId}\n  method: get\n  operationId: getIntelligenceRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/intelligence/scenarios\n  method: post\n  operationId: createIntelligenceScenario\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/v1/intelligence/runs/{runId}/handoff\n  method: get\n  operationId: getIntelligenceHandoff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/zillow/context\n  method: get\n  operationId: getPropertyZillowContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/zillow/timeseries\n  method: get\n  operationId: getZillowTimeseries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/zillow/compare\n  method: get\n  operationId: compareZillowMarkets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/zoning\n\
  \  method: get\n  operationId: getParcelZoning\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/zoning/search\n  method: get\n  operationId: searchZoning\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/zoning/coverage\n  method: get\n  operationId: getZoningCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/distress\n  method: get\n  operationId: getParcelDistress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/neighborhood/distress\n  method: get\n  operationId: getNeighborhoodDistress\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/r2-credentials\n  method: get\n  operationId: getR2DeliveryInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/data/databricks/grant\n  method: get\n  operationId: getDatabricksShareInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/permits/{permitId}/events\n  method: get\n  operationId: getPermitEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/permits/search\n  method: get\n  operationId: searchPermits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /api/v1/sources/{sourceId}/observations\n  method: get\n  operationId: getSourceObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/parcels/{id}/observations\n  method: get\n  operationId: getParcelObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/propraven-com/agentic-access/propraven-com-agentic-access.yml
summary_line: 92 operations · 7 acting · 1 human-in-the-loop
tags:
- Real Estate
- Data
- Property Intelligence
- US
---
