---
acting_count: 48
action_class_counts:
  acting: 48
  connected: 49
api_specs:
- filename: lune-accounts-api-openapi.yml
  format: yaml
  label: Lune Accounts API
  slug: lune-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-accounts-api-openapi.yml
- filename: lune-analytics-api-openapi.yml
  format: yaml
  label: Lune Analytics API
  slug: lune-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-analytics-api-openapi.yml
- filename: lune-bundle-portfolios-api-openapi.yml
  format: yaml
  label: Lune Bundle portfolios API
  slug: lune-bundle-portfolios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-bundle-portfolios-api-openapi.yml
- filename: lune-bundle-selections-api-openapi.yml
  format: yaml
  label: Lune Bundle selections API
  slug: lune-bundle-selections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-bundle-selections-api-openapi.yml
- filename: lune-bundles-api-openapi.yml
  format: yaml
  label: Lune Bundles API
  slug: lune-bundles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-bundles-api-openapi.yml
- filename: lune-client-accounts-api-openapi.yml
  format: yaml
  label: Lune Client accounts API
  slug: lune-client-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-client-accounts-api-openapi.yml
- filename: lune-emission-estimates-api-openapi.yml
  format: yaml
  label: Lune Emission estimates API
  slug: lune-emission-estimates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-emission-estimates-api-openapi.yml
- filename: lune-emission-factors-api-openapi.yml
  format: yaml
  label: Lune Emission factors API
  slug: lune-emission-factors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-emission-factors-api-openapi.yml
- filename: lune-orders-api-openapi.yml
  format: yaml
  label: Lune Orders API
  slug: lune-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-orders-api-openapi.yml
- filename: lune-payments-api-openapi.yml
  format: yaml
  label: Lune Payments API
  slug: lune-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-payments-api-openapi.yml
- filename: lune-projects-api-openapi.yml
  format: yaml
  label: Lune Projects API
  slug: lune-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-projects-api-openapi.yml
- filename: lune-shipments-api-openapi.yml
  format: yaml
  label: Lune Shipments API
  slug: lune-shipments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-shipments-api-openapi.yml
- filename: lune-sustainability-page-api-openapi.yml
  format: yaml
  label: Lune Sustainability page API
  slug: lune-sustainability-page-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-sustainability-page-api-openapi.yml
- filename: lune-webhook-request-api-openapi.yml
  format: yaml
  label: Lune Webhook request API
  slug: lune-webhook-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-webhook-request-api-openapi.yml
- filename: lune-webhooks-api-openapi.yml
  format: yaml
  label: Lune Webhooks API
  slug: lune-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lune/openapi/lune-webhooks-api-openapi.yml
consequence_counts:
  physical: 15
  read: 49
  write: 33
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lune Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /estimates/shipping
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /estimates/shipping/multi-leg
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /estimates/shipping/multi-leg/by-fuel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /estimates/shipping/multi-leg/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /estimates/shipping/multi-leg/{id}/annotations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /estimates/shipping/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /estimates/shipping/{id}/annotations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /estimates/transaction-documents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /estimates/transaction-documents/async
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/by-estimate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/by-mass
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/by-value
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipments/batches
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shipments/calculate
operation_count: 97
overview: 'Lune exposes 97 API operations that an AI agent could call, of which 48 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 49 read, 33 write, and 15 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lune
provider_slug: lune
slug: lune-agentic-access
source_filename: lune-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/lune-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 97\n  by_action_class:\n    connected: 49\n    acting: 48\n  by_consequence:\n    read: 49\n    write: 33\n    physical: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/me\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/client/me\n  method: get\n  operationId: getClientAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/client\n\
  \  method: post\n  operationId: createClientAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/client\n  method: get\n  operationId: listClientAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/client/{id}\n  method: put\n  operationId: updateClientAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/client/{id}\n  method: patch\n  operationId: partialUpdateClientAccount\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/client/{id}/logo\n  method: post\n  operationId: updateClientAccountLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/client/{id}/logo\n  method: delete\n  operationId: deleteClientAccountLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /accounts\n  method: post\n  operationId: createAccountPair\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{id}\n  method: put\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}\n  method: patch\n  operationId: partialUpdateAccount\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}/logo\n  method: post\n  operationId: updateAccountLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}/logo\n  method: delete\n  operationId: deleteAccountLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /analytics/cumulative-per-bundle\n  method: get\n  operationId: getCumulativeAnalyticsPerBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/metrics\n  method: get\n  operationId: getMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/aggregated-by-property\n  method: get\n  operationId: getAggregatedAnalyticsByProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/emission-calculations\n  method: get\n  operationId: getEmissionCalculationMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/business\n  method:\
  \ get\n  operationId: getBusinessEmissionsAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles\n  method: get\n  operationId: listBundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{id}\n  method: get\n  operationId: getBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{id}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /projects/{id}/perimeter\n  method: get\n  operationId: getProjectPerimeter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/by-slug/{slug}\n  method: get\n  operationId: getProjectBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/by-mass\n  method: post\n  operationId: createOrderByMass\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/by-value\n  method: post\n  operationId: createOrderByValue\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/by-estimate\n  method: post\n  operationId: createOrderByEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}/certificate\n  method: get\n  operationId: getOrderCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/by-idempotency-key/{idempotency_key}\n  method: get\n  operationId: getOrderByIdempotencyKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/by-mass/quote\n  method: post\n  operationId: getOrderQuoteByMass\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/by-value/quote\n  method: post\n  operationId: getOrderQuoteByValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundle-selections\n  method: get\n  operationId: getBundleSelection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundle-selections\n  method: put\n  operationId: updateBundleSelection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundle-portfolios\n  method: get\n  operationId: listAllBundlePortfolios\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundle-portfolios\n  method: put\n  operationId: updateBundlePortfolio\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/electricity\n  method: post\n  operationId: createElectricityEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/electricity/{id}\n  method: get\n  operationId: getElectricityEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates/electricity/{id}\n  method: put\n  operationId: updateElectricityEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/flight\n  method: post\n  operationId: createFlightEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/passenger-transportation\n  method: post\n  operationId: createPassengerTransportationEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/passenger-transportation/{id}\n\
  \  method: get\n  operationId: getPassengerTransportationEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates/passenger-transportation/{id}/annotations\n  method: patch\n  operationId: partialUpdatePassengerTransportationEstimateAnnotations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/shipping/all\n  method: get\n  operationId: listAllShippingEstimates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates/shipping\n  method: post\n  operationId: createShippingEstimate\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/shipping/{id}\n  method: get\n  operationId: getShippingEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates/shipping/{id}\n  method: put\n  operationId: updateShippingEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/shipping/{id}/annotations\n  method: patch\n\
  \  operationId: updateShippingEstimateAnnotations\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/shipping/multi-leg\n  method: post\n  operationId: createMultiLegShippingEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/shipping/multi-leg/{id}\n  method: get\n  operationId: getMultiLegShippingEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates/shipping/multi-leg/{id}\n  method: put\n  operationId: updateMultiLegShippingEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/shipping/multi-leg/{id}/annotations\n  method: patch\n  operationId: updateMultiLegShippingEstimateAnnotations\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/shipping/multi-leg/{id}/pdf\n\
  \  method: get\n  operationId: getMultiLegShippingEstimatePdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates/shipping/multi-leg/by-fuel\n  method: post\n  operationId: createMultiLegShippingEstimateByFuel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/shipping/multi-leg/by-fuel/{id}\n  method: get\n  operationId: getMultiLegShippingEstimateByFuel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates/transaction-documents\n  method: post\n  operationId: createTransactionDocumentEstimate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/transaction-documents/async\n  method: post\n  operationId: createTransactionDocumentEstimateAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/transaction-documents/{id}\n  method: get\n  operationId: getTransactionDocumentEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /estimates/transactions\n  method: post\n  operationId: createTransactionEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/transactions/batch\n  method: post\n  operationId: createBatchTransactionEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/transactions/by-idempotency-key/{idempotency_key}\n  method: get\n  operationId: getTransactionEstimateByIdempotencyKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates/transactions/{id}/annotations\n  method: patch\n  operationId: partialUpdateTransactionsEstimateAnnotations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/transaction-documents/{id}/annotations\n  method: patch\n  operationId: partialUpdateTransactionDocumentsEstimateAnnotations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/transactions/{id}\n  method: get\n  operationId: getTransactionEstimate\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates/transactions/{id}\n  method: put\n  operationId: updateTransactionEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/transactions/multi-match\n  method: post\n  operationId: createMultiMatchTransactionEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/company\n  method: post\n  operationId: createCompanyEstimate\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/company/{id}\n  method: get\n  operationId: getCompanyEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimates/company/{id}\n  method: put\n  operationId: updateCompanyEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/emission-factor\n  method: post\n  operationId: createEmissionFactorEstimate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /estimates/emission-factor/{id}\n  method: get\n  operationId: getEmissionFactorEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emission-factors\n  method: get\n  operationId: listEmissionFactors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emission-factors/regions\n  method: get\n  operationId: listAllEmissionFactorRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listAllWebhooks\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}/rotate-secret\n  method: put\n  operationId: rotateWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /WebhookRequest\n  method: post\n  operationId: webhookRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sustainability-pages\n  method: post\n  operationId: createSustainabilityPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sustainability-pages\n  method: put\n  operationId: updateSustainabilityPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sustainability-pages/current-account\n  method: get\n  operationId: getSustainabilityPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /sustainability-pages/public/{type}/{slug}\n  method: get\n  operationId: getPublicSustainabilityPageBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sustainability-pages/public/{organisation_id}/{type}/{handle}\n  method: get\n  operationId: getPublicSustainabilityPageByHandle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/by-temporary-id/{temporary_id}\n  method: get\n  operationId: getPaymentByTemporaryId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments\n  method: get\n  operationId: listShipments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments\n  method: delete\n  operationId: deleteShipments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipments/calculate\n  method: post\n  operationId: calculateShipments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipments/calculation-batches/{id}\n  method: get\n  operationId: getCalculationBatch\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments/summary\n  method: get\n  operationId: getShipmentSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments/batches\n  method: get\n  operationId: listShipmentBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments/batches\n  method: post\n  operationId: createShipmentBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shipments/batches/{id}\n\
  \  method: get\n  operationId: getShipmentBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shipments/{id}\n  method: get\n  operationId: getShipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/lune/agentic-access/lune-agentic-access.yml
summary_line: 97 operations · 48 acting
tags:
- Logistics
- Emissions
- Carbon
- Supply Chain
- Sustainability
---
