---
acting_count: 97
action_class_counts:
  acting: 97
api_specs:
- filename: bolt-eu-food-openapi.yml
  format: yaml
  label: Bolt Food API
  slug: bolt-eu-food-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-eu/refs/heads/main/openapi/bolt-eu-food-openapi.yml
- filename: bolt-eu-stores-openapi.yml
  format: yaml
  label: Bolt Stores API
  slug: bolt-eu-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-eu/refs/heads/main/openapi/bolt-eu-stores-openapi.yml
- filename: bolt-eu-delivery-openapi.yml
  format: yaml
  label: Bolt Delivery API
  slug: bolt-eu-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bolt-eu/refs/heads/main/openapi/bolt-eu-delivery-openapi.yml
consequence_counts:
  physical: 30
  write: 67
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bolt Eu Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/acceptOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/acceptOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/acceptOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/getOrderBasket
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/markOrderAsDelivered
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/markOrderAsDelivered
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/markOrderAsDelivered
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/markOrderAsPickedUp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/markOrderAsPickedUp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/markOrderAsPickedUp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/markOrderAsReadyForPickup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/markOrderAsReadyForPickup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/markOrderAsReadyForPickup
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/markOrderWithItemsAsReadyForPickUp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/markOrderWithItemsAsReadyForPickUp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/pauseOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/pauseOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/pauseOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/rejectOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/rejectOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/rejectOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/startAcceptingOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/startAcceptingOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/startAcceptingOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /genericClient/v2/markOrderWithItemsAsReadyForPickup
operation_count: 97
overview: 'Bolt exposes 97 API operations that an AI agent could call, of which 97 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 67 write and 30 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bolt
provider_slug: bolt-eu
slug: bolt-eu-agentic-access
source_filename: bolt-eu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bolt-eu-delivery-openapi.yml, openapi/bolt-eu-food-openapi.yml, openapi/bolt-eu-stores-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 97\n  by_action_class:\n    acting: 97\n  by_consequence:\n    write: 67\n    physical: 30\n  human_in_the_loop_required: 0\noperations:\n- path: /genericClient/pushMenu\n  method: post\n  operationId: genericClient-pushMenu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/getMenu\n  method:\
  \ post\n  operationId: genericClient-getMenu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/updateMenuItemAvailability\n  method: post\n  operationId: genericClient-updateMenuItemAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/acceptOrder\n  method: post\n  operationId: genericClient-acceptOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/rejectOrder\n  method: post\n  operationId: genericClient-rejectOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/markOrderAsReadyForPickup\n  method: post\n  operationId: genericClient-markOrderAsReadyForPickup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /genericClient/markOrderAsPickedUp\n  method: post\n  operationId: genericClient-markOrderAsPickedUp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/markOrderAsDelivered\n  method: post\n  operationId: genericClient-markOrderAsDelivered\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/waiter/createOrder\n  method: post\n  operationId: genericClient-waiter-createOrder\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/waiter/finalizeOrder\n  method: post\n  operationId: genericClient-waiter-finalizeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/startAcceptingOrders\n  method: post\n  operationId: genericClient-startAcceptingOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/pauseOrders\n  method: post\n  operationId: genericClient-pauseOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/updateProviderSchedule\n  method: post\n  operationId: genericClient-updateProviderSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /genericClient/updateMenuQuantity\n  method: post\n  operationId: genericClient-updateMenuQuantity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/markOrderWithItemsAsReadyForPickUp\n  method: post\n  operationId: genericClient-markOrderWithItemsAsReadyForPickUp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/v2/markOrderWithItemsAsReadyForPickup\n  method: post\n  operationId: genericClient-v2-markOrderWithItemsAsReadyForPickup\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/import/create\n  method: post\n  operationId: pim-v1-products-import-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/import/edit\n  method: post\n  operationId: pim-v1-products-import-edit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/import/status/retrieve\n  method: post\n  operationId: pim-v1-products-import-status-retrieve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/import/apply\n  method: post\n  operationId: pim-v1-products-import-apply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/import/cancel\n  method: post\n  operationId: pim-v1-products-import-cancel\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/timetable/createInBatch\n  method: post\n  operationId: pim-v1-timetable-createInBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/timetable/list\n  method: post\n  operationId: pim-v1-timetable-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/delist\n\
  \  method: post\n  operationId: pim-v1-products-delist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/menu/drafts/create\n  method: post\n  operationId: pim-v1-menu-drafts-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/menu/drafts/state/retrieve\n  method: post\n  operationId: pim-v1-menu-drafts-state-retrieve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/menu/drafts/reject\n  method: post\n  operationId: pim-v1-menu-drafts-reject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/menu/drafts/publish\n  method: post\n  operationId: pim-v1-menu-drafts-publish\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/menu/publish/list\n  method: post\n  operationId: pim-v1-menu-publish-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/menu/publish/cancel\n  method: post\n  operationId: pim-v1-menu-publish-cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/prices/import\n  method: post\n  operationId: pim-v1-products-prices-import\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/discount/prices/import\n\
  \  method: post\n  operationId: pim-v1-products-discount-prices-import\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/layout/set\n  method: post\n  operationId: pim-v1-layout-set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/categoryTree/get\n  method: post\n  operationId: pim-v1-categoryTree-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/categoryTree/set\n  method: post\n  operationId: pim-v1-categoryTree-set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/category/rearrange\n  method: post\n  operationId: pim-v1-category-rearrange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/category/products/set\n  method: post\n  operationId: pim-v1-category-products-set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/option/upsert\n  method: post\n  operationId: pim-v1-option-upsert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/option/list\n  method: post\n  operationId: pim-v1-option-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/optionGroup/upsert\n  method: post\n  operationId: pim-v1-optionGroup-upsert\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/optionGroup/list\n  method: post\n  operationId: pim-v1-optionGroup-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/fee/list\n  method: post\n  operationId: pim-v1-fee-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/fee/update\n\
  \  method: post\n  operationId: pim-v1-fee-update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/pushMenu\n  method: post\n  operationId: genericClient-pushMenu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/getMenu\n  method: post\n  operationId: genericClient-getMenu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/updateMenuItemAvailability\n  method: post\n  operationId: genericClient-updateMenuItemAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/acceptOrder\n  method: post\n  operationId: genericClient-acceptOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/rejectOrder\n  method: post\n  operationId: genericClient-rejectOrder\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/markOrderAsReadyForPickup\n  method: post\n  operationId: genericClient-markOrderAsReadyForPickup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/markOrderAsPickedUp\n  method: post\n  operationId: genericClient-markOrderAsPickedUp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/markOrderAsDelivered\n  method: post\n  operationId: genericClient-markOrderAsDelivered\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/waiter/createOrder\n  method: post\n  operationId: genericClient-waiter-createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/waiter/finalizeOrder\n  method: post\n  operationId: genericClient-waiter-finalizeOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/startAcceptingOrders\n  method: post\n  operationId: genericClient-startAcceptingOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/pauseOrders\n\
  \  method: post\n  operationId: genericClient-pauseOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/updateProviderSchedule\n  method: post\n  operationId: genericClient-updateProviderSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/option/upsert\n  method: post\n  operationId: pim-v1-option-upsert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/option/list\n  method: post\n  operationId: pim-v1-option-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/optionGroup/upsert\n  method: post\n  operationId: pim-v1-optionGroup-upsert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/optionGroup/list\n  method: post\n  operationId: pim-v1-optionGroup-list\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/getMenu\n  method: post\n  operationId: genericClient-getMenu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/acceptOrder\n  method: post\n  operationId: genericClient-acceptOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /genericClient/rejectOrder\n  method: post\n  operationId: genericClient-rejectOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/markOrderAsReadyForPickup\n  method: post\n  operationId: genericClient-markOrderAsReadyForPickup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/markOrderAsPickedUp\n  method: post\n  operationId: genericClient-markOrderAsPickedUp\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/markOrderWithItemsAsReadyForPickUp\n  method: post\n  operationId: genericClient-markOrderWithItemsAsReadyForPickUp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/v2/markOrderWithItemsAsReadyForPickup\n  method: post\n  operationId: genericClient-v2-markOrderWithItemsAsReadyForPickup\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/markOrderAsDelivered\n  method: post\n  operationId: genericClient-markOrderAsDelivered\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/getOrderBasket\n  method: post\n  operationId: genericClient-getOrderBasket\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/startAcceptingOrders\n  method: post\n  operationId: genericClient-startAcceptingOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/pauseOrders\n  method: post\n  operationId: genericClient-pauseOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /genericClient/updateProviderSchedule\n  method: post\n  operationId: genericClient-updateProviderSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /genericClient/updateMenuQuantity\n  method: post\n  operationId: genericClient-updateMenuQuantity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/import/create\n  method: post\n  operationId: pim-v1-products-import-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/import/edit\n  method: post\n  operationId: pim-v1-products-import-edit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/import/status/retrieve\n  method: post\n  operationId: pim-v1-products-import-status-retrieve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/import/apply\n  method:\
  \ post\n  operationId: pim-v1-products-import-apply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/import/cancel\n  method: post\n  operationId: pim-v1-products-import-cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/timetable/createInBatch\n  method: post\n  operationId: pim-v1-timetable-createInBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/timetable/list\n  method: post\n  operationId: pim-v1-timetable-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/products/delist\n  method: post\n  operationId: pim-v1-products-delist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/menu/drafts/create\n  method: post\n  operationId: pim-v1-menu-drafts-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/menu/drafts/state/retrieve\n  method: post\n  operationId: pim-v1-menu-drafts-state-retrieve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/menu/drafts/reject\n  method: post\n  operationId: pim-v1-menu-drafts-reject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pim/v1/menu/drafts/publish\n  method: post\n  operationId:\
  \ pim-v1-menu-drafts-publish\n  x-agentic-access\n\n# --- truncated at 32 KB (36 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/bolt-eu/refs/heads/main/agentic-access/bolt-eu-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolt-eu/refs/heads/main/agentic-access/bolt-eu-agentic-access.yml
summary_line: 97 operations · 97 acting
tags:
- Ride Booking
- Ride Hailing
- Mobility
- Transportation
- Food Delivery
- Micromobility
- Delivery
- Super App
---
