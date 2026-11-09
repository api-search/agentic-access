---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 38
api_specs:
- filename: carbonguru-io-analysis-api-openapi.yml
  format: yaml
  label: CarbonGuru Analysis API
  slug: carbonguru-io-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonguru-io/openapi/carbonguru-io-analysis-api-openapi.yml
- filename: carbonguru-io-history-api-openapi.yml
  format: yaml
  label: CarbonGuru History API
  slug: carbonguru-io-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonguru-io/openapi/carbonguru-io-history-api-openapi.yml
- filename: carbonguru-io-offsets-api-openapi.yml
  format: yaml
  label: CarbonGuru Offsets API
  slug: carbonguru-io-offsets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonguru-io/openapi/carbonguru-io-offsets-api-openapi.yml
- filename: carbonguru-io-reference-api-openapi.yml
  format: yaml
  label: CarbonGuru Reference API
  slug: carbonguru-io-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonguru-io/openapi/carbonguru-io-reference-api-openapi.yml
- filename: carbonguru-io-service-api-openapi.yml
  format: yaml
  label: CarbonGuru Service API
  slug: carbonguru-io-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonguru-io/openapi/carbonguru-io-service-api-openapi.yml
- filename: carbonguru-io-store-api-openapi.yml
  format: yaml
  label: CarbonGuru Store API
  slug: carbonguru-io-store-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonguru-io/openapi/carbonguru-io-store-api-openapi.yml
- filename: carbonguru-io-webhooks-api-openapi.yml
  format: yaml
  label: CarbonGuru Webhooks API
  slug: carbonguru-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carbonguru-io/openapi/carbonguru-io-webhooks-api-openapi.yml
consequence_counts:
  physical: 6
  read: 38
  safety-critical: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Carbonguru Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/webhook-endpoints/{endpoint_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/offsets/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/offsets/purchases
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/offsets/subscriptions/{subscription_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhook-deliveries/{delivery_id}/replay
operation_count: 61
overview: 'CarbonGuru exposes 61 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read, 16 write, 6 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CarbonGuru
provider_slug: carbonguru-io
slug: carbonguru-io-agentic-access
source_filename: carbonguru-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/carbonguru-io.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 61\n  by_action_class:\n    acting: 23\n    connected: 38\n  by_consequence:\n    write: 16\n    read: 38\n    safety-critical: 1\n    physical: 6\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/analyses\n  method: post\n  operationId: createAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:analyze\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions\n  method: get\n  operationId:\
  \ listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}/progress\n  method: get\n  operationId: getSessionProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{session_id}/exports\n  method: post\n  operationId: createSessionExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:analyze\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/exports/{job_id}\n  method: get\n  operationId: getExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:analyze\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exports/{job_id}/download\n  method: get\n  operationId: downloadExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:analyze\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/imports/{job_id}\n  method: get\n  operationId: getImport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/imports/{job_id}/download\n  method: get\n  operationId: downloadImport\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/footprints/search\n  method: get\n  operationId: searchFootprints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reference/naics\n  method: get\n  operationId: searchNaics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:reference\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reference/naics/{code}\n  method: get\n  operationId: getNaicsCode\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:reference\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reference/sectors\n  method: get\n  operationId: searchSectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:reference\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reference/sectors/{code}\n  method: get\n  operationId: getSector\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:reference\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reference/emission-factors/{naics_code}\n  method: get\n  operationId: getEmissionFactor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:reference\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reference/countries\n  method: get\n  operationId:\
  \ listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:reference\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook-endpoints\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook-endpoints\n  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-endpoints/{endpoint_id}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    scope:\n    - carbon:read\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/webhook-endpoints/{endpoint_id}/rotate-secret\n  method: post\n  operationId: rotateWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhook-deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook-deliveries/{delivery_id}/replay\n\
  \  method: post\n  operationId: replayWebhookDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - carbon:read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/openapi.json\n  method: get\n  operationId: getOpenapi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/status\n  method: get\n  operationId: getStoreStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - carbon:merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/config\n  method: get\n  operationId: getStoreConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/display-settings\n  method: get\n  operationId: getDisplaySettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/display-settings\n  method: put\n  operationId: updateDisplaySettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:merchant\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/store/products\n  method: get\n  operationId: listStoreProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/products/{product_id}/activate\n  method: post\n  operationId: activateStoreProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:merchant\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/store/products/{product_id}/deactivate\n  method: post\n  operationId: deactivateStoreProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:merchant\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/store/products/{product_id}/reanalyze\n  method: post\n  operationId: reanalyzeStoreProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:merchant\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/store/products/{product_id}\n  method: delete\n  operationId: deleteStoreProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:merchant\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/store/scan\n  method: post\n  operationId: startStoreScan\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:merchant\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/store/scan\n  method: get\n  operationId: getStoreScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog\n  method: post\n  operationId: pushCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:merchant\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pushes/{push_id}\n  method: get\n  operationId: getPush\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pushes/{push_id}/items\n  method: get\n  operationId: getPushItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/footprints\n  method: get\n  operationId: readStoreFootprints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/store/footprints/{identifier}\n  method: get\n  operationId: readStoreFootprint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders\n  method: post\n  operationId:\
  \ createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - carbon:merchant\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders\n  method: get\n  operationId: listOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/quote\n  method: post\n  operationId: quoteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - carbon:merchant\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{order_ref}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:merchant\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offsets/subscriptions\n  method: get\n  operationId: listOffsetSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:commerce\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offsets/subscriptions/{subscription_id}\n  method: get\n  operationId: getOffsetSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:commerce\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offsets/subscriptions/{subscription_id}\n  method: post\n  operationId: manageOffsetSubscription\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - carbon:commerce\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offsets/purchases\n  method: post\n  operationId: purchaseOffsets\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - carbon:commerce\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offsets/purchases/{purchase_id}\n  method: get\n  operationId: getOffsetPurchase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    -\
  \ carbon:commerce\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offsets/quote\n  method: post\n  operationId: quoteOffsets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:commerce\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offsets/cart\n  method: get\n  operationId: getOffsetCart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:commerce\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offsets/cart\n  method: delete\n  operationId: clearOffsetCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:commerce\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offsets/cart/items\n  method: post\n  operationId: addOffsetCartItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:commerce\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offsets/cart/items/{item_key}\n  method: delete\n  operationId: removeOffsetCartItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:commerce\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offsets/checkout\n  method: post\n  operationId: getOffsetCheckoutLink\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - carbon:commerce\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offsets/history\n  method: get\n  operationId: listOffsetPurchases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:commerce\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offsets/impact\n  method: get\n  operationId: getOffsetImpact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:commerce\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offsets/defaults\n  method: get\n  operationId: getOffsetDefaults\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - carbon:commerce\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offsets/defaults\n  method: put\n  operationId: setOffsetDefaults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - carbon:commerce\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offset-products\n  method: get\n  operationId: listOffsetProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - carbon:reference\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/carbonguru-io/agentic-access/carbonguru-io-agentic-access.yml
summary_line: 61 operations · 23 acting · 1 human-in-the-loop
tags:
- Carbon Footprinting
- Automated Offsetting
- E-Commerce
- Marketplace
- B2B
- Consumer
- Sustainability
---
