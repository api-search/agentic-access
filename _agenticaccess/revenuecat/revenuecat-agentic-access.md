---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 15
api_specs:
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Subscribers API
  slug: revenuecat-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Purchases & Receipts API
  slug: revenuecat-purchases-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Entitlements API (v1)
  slug: revenuecat-entitlements-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Offerings API (v1)
  slug: revenuecat-offerings-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Customer Attributes API
  slug: revenuecat-customer-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Projects API (v2)
  slug: revenuecat-projects-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Apps API (v2)
  slug: revenuecat-apps-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Customers API (v2)
  slug: revenuecat-customers-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Products API (v2)
  slug: revenuecat-products-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Entitlements API (v2)
  slug: revenuecat-entitlements-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Offerings API (v2)
  slug: revenuecat-offerings-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
- filename: revenuecat-openapi.yml
  format: yaml
  label: RevenueCat Packages API (v2)
  slug: revenuecat-packages-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/openapi/revenuecat-openapi.yml
consequence_counts:
  physical: 3
  read: 15
  safety-critical: 2
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Revenuecat Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /subscribers/{app_user_id}/entitlements/{entitlement_identifier}/revoke_promotionals
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /subscribers/{app_user_id}/offerings/{offering_uuid}/override
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /receipts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /subscribers/{app_user_id}/subscriptions/{product_identifier}/defer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /subscribers/{app_user_id}/transactions/{store_transaction_identifier}/refund
operation_count: 34
overview: 'RevenueCat exposes 34 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 14 write, 3 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RevenueCat
provider_slug: revenuecat
slug: revenuecat-agentic-access
source_filename: revenuecat-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/revenuecat-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 15\n    acting: 19\n  by_consequence:\n    read: 15\n    write: 14\n    physical: 3\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /subscribers/{app_user_id}\n  method: get\n  operationId: getOrCreateSubscriber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers/{app_user_id}\n  method: delete\n  operationId: deleteSubscriber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers/{app_user_id}/attributes\n  method: post\n  operationId: updateSubscriberAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /receipts\n  method: post\n  operationId: createReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers/{app_user_id}/transactions/{store_transaction_identifier}/refund\n\
  \  method: post\n  operationId: refundTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers/{app_user_id}/subscriptions/{product_identifier}/defer\n  method: post\n  operationId: deferSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers/{app_user_id}/entitlements/{entitlement_identifier}/promotional\n  method: post\n  operationId: grantPromotionalEntitlement\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers/{app_user_id}/entitlements/{entitlement_identifier}/revoke_promotionals\n  method: post\n  operationId: revokePromotionalEntitlements\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /subscribers/{app_user_id}/offerings\n  method: get\n  operationId: getOfferings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers/{app_user_id}/offerings/{offering_uuid}/override\n\
  \  method: post\n  operationId: overrideOffering\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/apps\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/apps\n  method: post\n  operationId: createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/apps/{app_id}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/apps/{app_id}\n  method: delete\n  operationId: deleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/customers\n  method: get\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/customers\n\
  \  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/customers/{customer_id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/customers/{customer_id}\n  method: delete\n  operationId: deleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/products\n  method:\
  \ get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/products\n  method: post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/products/{product_id}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/products/{product_id}\n  method: delete\n  operationId: deleteProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/entitlements\n  method: get\n  operationId: listEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/entitlements\n  method: post\n  operationId: createEntitlement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/entitlements/{entitlement_id}\n  method: get\n  operationId: getEntitlement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /projects/{project_id}/entitlements/{entitlement_id}\n  method: delete\n  operationId: deleteEntitlement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/offerings\n  method: get\n  operationId: listOfferingsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/offerings\n  method: post\n  operationId: createOfferingV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /projects/{project_id}/offerings/{offering_id}\n  method: get\n  operationId: getOfferingV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/offerings/{offering_id}/packages\n  method: get\n  operationId: listPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/offerings/{offering_id}/packages\n  method: post\n  operationId: createPackage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/offerings/{offering_id}/packages/{package_id}\n  method: get\n\
  \  operationId: getPackage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/offerings/{offering_id}/packages/{package_id}\n  method: delete\n  operationId: deletePackage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revenuecat/refs/heads/main/agentic-access/revenuecat-agentic-access.yml
summary_line: 34 operations · 19 acting · 2 human-in-the-loop
tags:
- Subscriptions
- In-App Purchases
- Billing
- Mobile
- Entitlements
---
