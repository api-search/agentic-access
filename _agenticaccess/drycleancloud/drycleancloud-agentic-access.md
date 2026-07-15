---
acting_count: 44
action_class_counts:
  acting: 44
api_specs:
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Customers API
  slug: drycleancloud-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Orders API
  slug: drycleancloud-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Products & Inventory API
  slug: drycleancloud-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Pickup & Delivery API
  slug: drycleancloud-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Payments & Promotions API
  slug: drycleancloud-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Business & Reporting API
  slug: drycleancloud-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Messaging API
  slug: drycleancloud-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
- filename: drycleancloud-openapi.yml
  format: yaml
  label: CleanCloud Webhooks
  slug: drycleancloud-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/openapi/drycleancloud-openapi.yml
consequence_counts:
  physical: 20
  safety-critical: 1
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Drycleancloud Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /passwordCustomer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /addCard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /addMessage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /addOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /addSubscription
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chargeCard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /convertLoyaltyPoints
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deleteOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deleteSubscription
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getCards
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getGarment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getGarments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getInvoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getPayments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getPhotos
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getSubscription
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /setDefaultCard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /updateGarment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /updateOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /usePromo
operation_count: 44
overview: 'CleanCloud exposes 44 API operations that an AI agent could call, of which 44 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 write, 20 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CleanCloud
provider_slug: drycleancloud
slug: drycleancloud-agentic-access
source_filename: drycleancloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/drycleancloud-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    acting: 44\n  by_consequence:\n    write: 23\n    safety-critical: 1\n    physical: 20\n  human_in_the_loop_required: 1\noperations:\n- path: /addCustomer\n  method: post\n  operationId: addCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /updateCustomer\n  method: post\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deleteCustomer\n  method: post\n  operationId: deleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getCustomer\n  method: post\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loginCustomer\n  method: post\n  operationId: loginCustomer\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /passwordCustomer\n  method: post\n  operationId: passwordCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /addOrder\n  method: post\n  operationId: addOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /updateOrder\n  method: post\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deleteOrder\n  method: post\n  operationId: deleteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getOrders\n  method: post\n  operationId: getOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getGarment\n  method: post\n  operationId: getGarment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getGarments\n  method: post\n  operationId: getGarments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /updateGarment\n  method: post\n  operationId: updateGarment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getProducts\n  method: post\n  operationId: getProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getPriceLists\n  method: post\n  operationId: getPriceLists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getInventory\n  method: post\n  operationId: getInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repeatPickup\n  method: post\n  operationId: repeatPickup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /updateRepeatPickup\n  method: post\n  operationId: updateRepeatPickup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deletePickup\n  method: post\n  operationId: deletePickup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getPickups\n  method: post\n  operationId: getPickups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getDates\n  method: post\n  operationId: getDates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getSlots\n  method: post\n  operationId: getSlots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getRoute\n  method: post\n  operationId: getRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /driverLocation\n  method: post\n  operationId: driverLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getPayments\n  method: post\n  operationId: getPayments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getInvoices\n  method: post\n  operationId: getInvoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /addCard\n  method: post\n  operationId: addCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chargeCard\n  method: post\n  operationId: chargeCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getCards\n  method: post\n  operationId: getCards\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n    \
  \  exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /setDefaultCard\n  method: post\n  operationId: setDefaultCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addSubscription\n  method: post\n  operationId: addSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deleteSubscription\n\
  \  method: post\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getSubscription\n  method: post\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usePromo\n  method: post\n  operationId: usePromo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /convertLoyaltyPoints\n  method: post\n  operationId: convertLoyaltyPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getBusinessAccounts\n  method: post\n  operationId: getBusinessAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /summaryReport\n  method: post\n\
  \  operationId: summaryReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getPhotos\n  method: post\n  operationId: getPhotos\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addToCustomerGroup\n  method: post\n  operationId: addToCustomerGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /getReferral\n  method: post\n  operationId: getReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addMessage\n  method: post\n  operationId: addMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getMessages\n  method: post\n  operationId: getMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addPushToken\n  method: post\n  operationId: addPushToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deletePushToken\n  method: post\n  operationId: deletePushToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drycleancloud/refs/heads/main/agentic-access/drycleancloud-agentic-access.yml
summary_line: 44 operations · 44 acting · 1 human-in-the-loop
tags:
- Dry Cleaning
- Laundry
- Point of Sale
- POS
- Field Service
- Pickup and Delivery
- SMB Software
---
