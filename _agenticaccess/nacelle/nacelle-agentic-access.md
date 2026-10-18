---
acting_count: 51
action_class_counts:
  acting: 51
  connected: 4
api_specs:
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Products API
  slug: nacelle-storefront-products-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Product Collections API
  slug: nacelle-storefront-product-collections-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Content API
  slug: nacelle-storefront-content-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Navigation and Spaces API
  slug: nacelle-storefront-navigation-spaces-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Admin Indexing and Ingestion API
  slug: nacelle-admin-indexing-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle-addresses-api-openapi.yml
  format: yaml
  label: Nacelle Addresses API
  slug: nacelle-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-addresses-api-openapi.yml
- filename: nacelle-checkout-api-openapi.yml
  format: yaml
  label: Nacelle Checkout API
  slug: nacelle-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-checkout-api-openapi.yml
- filename: nacelle-credentials-api-openapi.yml
  format: yaml
  label: Nacelle Credentials API
  slug: nacelle-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-credentials-api-openapi.yml
- filename: nacelle-customers-api-openapi.yml
  format: yaml
  label: Nacelle Customers API
  slug: nacelle-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-customers-api-openapi.yml
- filename: nacelle-entries-alpha-api-openapi.yml
  format: yaml
  label: Nacelle entries (ALPHA) API
  slug: nacelle-entries-alpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-entries-alpha-api-openapi.yml
- filename: nacelle-entries-api-openapi.yml
  format: yaml
  label: Nacelle Entries API
  slug: nacelle-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-entries-api-openapi.yml
- filename: nacelle-entries-beta-api-openapi.yml
  format: yaml
  label: Nacelle entries (BETA) API
  slug: nacelle-entries-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-entries-beta-api-openapi.yml
- filename: nacelle-fulfillments-api-openapi.yml
  format: yaml
  label: Nacelle Fulfillments API
  slug: nacelle-fulfillments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-fulfillments-api-openapi.yml
- filename: nacelle-index-api-openapi.yml
  format: yaml
  label: Nacelle Index API
  slug: nacelle-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-index-api-openapi.yml
- filename: nacelle-multiorders-api-openapi.yml
  format: yaml
  label: Nacelle Multiorders API
  slug: nacelle-multiorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-multiorders-api-openapi.yml
- filename: nacelle-orderitems-api-openapi.yml
  format: yaml
  label: Nacelle Orderitems API
  slug: nacelle-orderitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-orderitems-api-openapi.yml
- filename: nacelle-payment-api-openapi.yml
  format: yaml
  label: Nacelle Payment API
  slug: nacelle-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-payment-api-openapi.yml
- filename: nacelle-paymentintent-api-openapi.yml
  format: yaml
  label: Nacelle Paymentintent API
  slug: nacelle-paymentintent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-paymentintent-api-openapi.yml
- filename: nacelle-token-api-openapi.yml
  format: yaml
  label: Nacelle Token API
  slug: nacelle-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-token-api-openapi.yml
consequence_counts:
  physical: 13
  read: 4
  write: 38
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nacelle Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fulfillments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /fulfillments/{nacelle-fulfillment-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /multicart/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /multiorders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /multiorders/{nacelle-multi-order-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /multiordersasync
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /orderitems/{nacelle-order-item-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentintent/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /paymentintent/{payment-intent-id}/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /paymentintent/{payment-intent-id}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /paymentintent/{payment-intent-id}/update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payments/{nacelle-payment-id}
operation_count: 55
overview: 'Nacelle exposes 55 API operations that an AI agent could call, of which 51 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 38 write, and 13 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nacelle
provider_slug: nacelle
slug: nacelle-agentic-access
source_filename: nacelle-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/nacelle-auth-api-openapi.yml, openapi/nacelle-ingest-api-openapi.yml, openapi/nacelle-order-management-api-experimental-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 55\n  by_action_class:\n    acting: 51\n    connected: 4\n  by_consequence:\n    write: 38\n    read: 4\n    physical: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /credential\n  method: post\n  operationId: createCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /credential/list/available\n  method: get\n  operationId: listCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credential/token\n  method: post\n  operationId: createPrivateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credential/{client-id}\n  method: delete\n  operationId: deleteCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credential/{client-id}\n  method: get\n  operationId:\
  \ readCredential\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credential/{client-id}/refresh\n  method: post\n  operationId: rotateCredentialSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issue\n  method: post\n  operationId: issuePublicToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collection\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collection\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collection-content\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collection-content\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom-schema\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /index\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /index\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /index/cancel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /index/clear\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /index/{indexId}/finish\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory-item\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory-item\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory-level\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory-level\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory-location\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inventory-location\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /price-book\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /price-book\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /pricing\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pricing\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /product\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product-content\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /product-content\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /variant\n  method: put\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /variant\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /variant-content\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /variant-content\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/{nacelle-address-id}\n  method: patch\n  operationId: updateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /checkout/validate\n  method: post\n  operationId: validateCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n\
  \  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{nacelle-customer-id}\n  method: patch\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{nacelle-customer-id}/addresses\n  method: post\n  operationId: addCustomerAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillments\n  method: post\n  operationId: createFulfillment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fulfillments/{nacelle-fulfillment-id}\n  method: patch\n  operationId: updateFulfillment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /multicart/validate\n  method: post\n  operationId: multiCartValidate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /multiorders\n  method: post\n  operationId: createMultiOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /multiorders/{nacelle-multi-order-id}\n  method: patch\n  operationId: updateMultiOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /multiordersasync\n  method: post\n  operationId: createAsyncMultiOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orderitems/{nacelle-order-item-id}\n  method: patch\n  operationId: updateOrderItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentintent/create\n\
  \  method: post\n  operationId: createPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentintent/{payment-intent-id}/capture\n  method: patch\n  operationId: capturePaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentintent/{payment-intent-id}/refund\n  method: patch\n  operationId: refundPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentintent/{payment-intent-id}/retrieve\n  method: get\n  operationId: retrievePaymentIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paymentintent/{payment-intent-id}/update\n  method: patch\n  operationId: updatePaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{nacelle-payment-id}\n  method: patch\n\
  \  operationId: updatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/agentic-access/nacelle-agentic-access.yml
summary_line: 55 operations · 51 acting
tags:
- Commerce
- Headless Commerce
- Composable Commerce
- GraphQL
- Content
- Data Indexing
---
