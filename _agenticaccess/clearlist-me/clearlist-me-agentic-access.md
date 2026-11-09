---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 8
api_specs:
- filename: clearlist-me-account-api-openapi.yml
  format: yaml
  label: ClearList Account API
  slug: clearlist-me-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-account-api-openapi.yml
- filename: clearlist-me-jobs-api-openapi.yml
  format: yaml
  label: ClearList Jobs API
  slug: clearlist-me-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-jobs-api-openapi.yml
- filename: clearlist-me-listings-api-openapi.yml
  format: yaml
  label: ClearList Listings API
  slug: clearlist-me-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-listings-api-openapi.yml
- filename: clearlist-me-onboarding-api-openapi.yml
  format: yaml
  label: ClearList Onboarding API
  slug: clearlist-me-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-onboarding-api-openapi.yml
- filename: clearlist-me-orders-api-openapi.yml
  format: yaml
  label: ClearList Orders API
  slug: clearlist-me-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-orders-api-openapi.yml
- filename: clearlist-me-publishing-api-openapi.yml
  format: yaml
  label: ClearList Publishing API
  slug: clearlist-me-publishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-publishing-api-openapi.yml
- filename: clearlist-me-scheduling-api-openapi.yml
  format: yaml
  label: ClearList Scheduling API
  slug: clearlist-me-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-scheduling-api-openapi.yml
- filename: clearlist-me-system-api-openapi.yml
  format: yaml
  label: ClearList System API
  slug: clearlist-me-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-system-api-openapi.yml
consequence_counts:
  physical: 8
  read: 8
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clearlist Me Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/auth/send-code
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/conversations/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/conversations/{id}/address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/conversations/{id}/address/prepare
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/conversations/{id}/reply/prepare
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/payments/checkout-link
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/reservations/{id}/pickup-confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/reservations/{id}/pickup-confirm/prepare
operation_count: 26
overview: 'ClearList exposes 26 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 10 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ClearList
provider_slug: clearlist-me
slug: clearlist-me-agentic-access
source_filename: clearlist-me-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/clearlist-me-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 18\n    connected: 8\n  by_consequence:\n    physical: 8\n    write: 10\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/auth/send-code\n  method: post\n  operationId: sendVerificationCode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/verify-code\n  method:\
  \ post\n  operationId: verifyCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/items\n  method: get\n  operationId: getListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/items\n  method: post\n  operationId: createListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/items/{id}\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/items/{id}\n  method: put\n  operationId: editListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/items/{id}\n  method: delete\n  operationId: deleteListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/items/{id}/restore\n  method: post\n  operationId: restoreListing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/items/bulk-upload\n  method: post\n  operationId: bulkCreateListings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/items/bulk-generate\n  method: post\n  operationId: generateListingFromPhotos\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/ai-jobs/{jobId}\n  method: get\n  operationId: getJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pages/publish\n  method: post\n  operationId: publishPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pages/renewal-options\n  method: get\n  operationId: getPageRenewalOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pages/extend\n  method: post\n  operationId: extendSalePage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/conversations\n  method: get\n  operationId: getReservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/conversations/{id}\n  method: post\n  operationId: replyToBuyer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/scheduling/availability\n  method: put\n  operationId: setAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/payments/status\n  method: get\n  operationId: checkTierStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/payments/checkout-link\n  method: post\n  operationId: generatePaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/conversations/{id}/address/prepare\n  method: post\n  operationId: prepareAddressShare\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/conversations/{id}/reply/prepare\n  method: post\n  operationId: prepareReplyToBuyer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write\n   \
  \ audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/reservations/{id}/pickup-confirm\n  method: post\n  operationId: confirmPickup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/reservations/{id}/pickup-confirm/prepare\n  method: post\n  operationId: preparePickupConfirm\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/conversations/{id}/address\n  method: post\n  operationId: shareAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/clearlist-me/agentic-access/clearlist-me-agentic-access.yml
summary_line: 26 operations · 18 acting
tags:
- Artificial Intelligence
- Resale
- Marketplace
- Automation
- E-Commerce
- Company
---
