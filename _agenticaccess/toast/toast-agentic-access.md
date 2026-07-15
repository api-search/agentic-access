---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 20
api_specs:
- filename: toast-orders-openapi.yaml
  format: yaml
  label: Toast Orders API
  slug: toast-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-orders-openapi.yaml
- filename: toast-menus-openapi.yaml
  format: yaml
  label: Toast Menus API
  slug: toast-menus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-menus-openapi.yaml
- filename: toast-labor-openapi.yaml
  format: yaml
  label: Toast Labor API
  slug: toast-labor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-labor-openapi.yaml
- filename: toast-restaurants-openapi.yaml
  format: yaml
  label: Toast Restaurants API
  slug: toast-restaurants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-restaurants-openapi.yaml
- filename: toast-stock-openapi.yaml
  format: yaml
  label: Toast Stock API
  slug: toast-stock
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-stock-openapi.yaml
- filename: toast-partners-openapi.yaml
  format: yaml
  label: Toast Partners API
  slug: toast-partners
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-partners-openapi.yaml
- filename: toast-authentication-openapi.yaml
  format: yaml
  label: Toast Authentication API
  slug: toast-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/openapi/toast-authentication-openapi.yaml
consequence_counts:
  physical: 9
  read: 20
  safety-critical: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Toast Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /employees/{employeeId}/wageOverrides
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderGuid}/checks/{checkGuid}/appliedDiscounts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderGuid}/checks/{checkGuid}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /orders/{orderGuid}/checks/{checkGuid}/payments/{paymentGuid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderGuid}/checks/{checkGuid}/selections
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderGuid}/checks/{checkGuid}/selections/{selectionGuid}/appliedDiscounts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /orders/{orderGuid}/deliveryInfo
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{orderGuid}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /prices
operation_count: 46
overview: 'Toast exposes 46 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 16 write, 9 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Toast
provider_slug: toast
slug: toast-agentic-access
source_filename: toast-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/toast-authentication-openapi.yaml, openapi/toast-labor-openapi.yaml, openapi/toast-menus-openapi.yaml,\n  openapi/toast-orders-openapi.yaml, openapi/toast-partners-openapi.yaml, openapi/toast-restaurants-openapi.yaml,\n  openapi/toast-stock-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 46\n  by_action_class:\n    acting: 26\n    connected: 20\n  by_consequence:\n    write: 16\n    read: 20\n    safety-critical: 1\n    physical: 9\n  human_in_the_loop_required: 1\noperations:\n- path: /authentication/login\n  method: post\n  operationId: authenticationLoginPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees\n  method: get\n  operationId: employeesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - labor.employees:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees\n  method: post\n  operationId: employeesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - labor.employees:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{employeeId}\n  method: get\n  operationId: employeesEmployeeIdGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - labor.employees:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{employeeId}\n  method: delete\n  operationId: employeesEmployeeIdDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - labor.employees:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{employeeId}\n  method: patch\n  operationId: employeesEmployeeIdPatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - labor.employees:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{employeeId}/externalId\n  method: post\n  operationId: employeesEmployeeIdExternalIdPost\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - labor.employees:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{employeeId}/externalId\n  method: put\n  operationId: employeesEmployeeIdExternalIdPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - labor.employees:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{employeeId}/unarchive\n  method: put\n  operationId: employeesEmployeeIdUnarchivePut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - labor.employees:write\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{employeeId}/jobs\n  method: put\n  operationId: employeesEmployeeIdJobsPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - labor.employees:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{employeeId}/wageOverrides\n  method: put\n  operationId: employeesEmployeeIdWageOverridesPut\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - labor.employees:write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n \
  \     human-in-the-loop: required\n    audit: required\n- path: /shifts\n  method: get\n  operationId: shiftsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - labor:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shifts\n  method: post\n  operationId: shiftsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - labor.shifts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shifts/{shiftId}\n  method: get\n  operationId: shiftsShiftIdGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - labor:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shifts/{shiftId}\n  method: put\n  operationId: shiftsShiftIdPut\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - labor.shifts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shifts/{shiftId}\n  method: delete\n  operationId: shiftsShiftIdDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - labor.shifts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  operationId: jobsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - labor:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jobId}\n  method: get\n  operationId: jobsJobIdGet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - labor:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jobId}/externalId\n  method: post\n  operationId: jobsJobIdExternalIdPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - labor.jobs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{jobId}/externalId\n  method: put\n  operationId: jobsJobIdExternalIdPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - labor.jobs:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timeEntries\n  method: get\n  operationId:\
  \ timeEntriesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - labor:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeEntries/{timeEntryId}\n  method: get\n  operationId: timeEntriesTimeEntryIdGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - labor:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /menus\n  method: get\n  operationId: menusGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - menus:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata\n  method: get\n  operationId: metadataGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - menus:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: get\n  operationId: paymentsGet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{guid}\n  method: get\n  operationId: paymentsGuidGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prices\n  method: post\n  operationId: pricesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - orders.orders:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{guid}\n  method: get\n  operationId: ordersGuidGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - orders:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ordersBulk\n  method: get\n  operationId: ordersBulkGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{orderGuid}/checks/{checkGuid}/payments\n  method: post\n  operationId: ordersChecksPaymentsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - orders.payments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderGuid}/checks/{checkGuid}/payments/{paymentGuid}\n  method: patch\n  operationId: ordersOrderGuidChecksCheckGuidPaymentsPaymentGuidPatch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    scope:\n    - orders.payments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderGuid}/checks/{checkGuid}/selections\n  method: post\n  operationId: ordersOrderGuidChecksCheckGuidSelectionsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - orders.items:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderGuid}/checks/{checkGuid}/appliedDiscounts\n  method: post\n  operationId: ordersChecksAppliedDiscountsPost\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    scope:\n    - orders.discounts:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderGuid}/checks/{checkGuid}/selections/{selectionGuid}/appliedDiscounts\n  method: post\n  operationId: ordersChecksSelectionsAppliedDiscountsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - orders.discounts:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderGuid}/deliveryInfo\n  method: patch\n  operationId: ordersOrderGuidDeliveryInfoPatch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - orders.delivery_info:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{orderGuid}/void\n  method: post\n  operationId: voidOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - orders.channel:void\n    - orders:void\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: post\n  operationId: ordersPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - orders.orders:write\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders\n  method: get\n  operationId: ordersGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - orders:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicableDiscounts\n  method: post\n  operationId: applicableDiscountsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - orders.orders:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restaurants\n  method: get\n  operationId: restaurantsGet\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connectedRestaurants\n  method: get\n  operationId: connectedRestaurantsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restaurants/{restaurantGUID}\n  method: get\n  operationId: restaurantsRestaurantGuidGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - restaurants:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{managementGroupGUID}/restaurants\n  method: get\n  operationId: groupsManagementGroupGuidRestaurantsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - restaurants:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inventory\n  method: get\n  operationId: getInventory\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - stock:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/inventory/search\n  method: post\n  operationId: postInventorySearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - stock:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/inventory/update\n  method: put\n  operationId: updateInventory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - stock:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toast/refs/heads/main/agentic-access/toast-agentic-access.yml
summary_line: 46 operations · 26 acting · 1 human-in-the-loop
tags:
- Food Service
- Point of Sale
- Restaurants
- Hospitality
---
