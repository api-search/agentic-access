---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 5
api_specs:
- filename: punchh-mobile-api-openapi.yml
  format: yaml
  label: Punchh Mobile API
  slug: punchh-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-mobile-api-openapi.yml
- filename: punchh-mobile-redemptions-legacy-openapi.yml
  format: yaml
  label: Punchh Redemptions 1.0 (Legacy) API - Mobile
  slug: punchh-mobile-redemptions-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-mobile-redemptions-legacy-openapi.yml
- filename: punchh-mobile-redemptions-v2-openapi.yml
  format: yaml
  label: Punchh Redemptions 2.0 (New) API - Mobile
  slug: punchh-mobile-redemptions-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-mobile-redemptions-v2-openapi.yml
- filename: punchh-mobile-subscription-openapi.yml
  format: yaml
  label: Punchh Subscription API - Mobile
  slug: punchh-mobile-subscription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-mobile-subscription-openapi.yml
- filename: punchh-online-ordering-redemptions-legacy-openapi.yml
  format: yaml
  label: Punchh Redemptions 1.0 (Legacy) API - Online Ordering
  slug: punchh-online-ordering-redemptions-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-online-ordering-redemptions-legacy-openapi.yml
- filename: punchh-online-ordering-redemptions-v2-openapi.yml
  format: yaml
  label: Punchh Redemptions 2.0 (New) API - Online Ordering
  slug: punchh-online-ordering-redemptions-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-online-ordering-redemptions-v2-openapi.yml
- filename: punchh-online-ordering-sso-api-openapi.yml
  format: yaml
  label: Punchh Online Ordering and SSO API
  slug: punchh-online-ordering-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-online-ordering-sso-api-openapi.yml
- filename: punchh-online-ordering-subscription-openapi.yml
  format: yaml
  label: Punchh Subscription API - Online Ordering
  slug: punchh-online-ordering-subscription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-online-ordering-subscription-openapi.yml
- filename: punchh-platform-functions-api-openapi.yml
  format: yaml
  label: Punchh Platform Functions API
  slug: punchh-platform-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-platform-functions-api-openapi.yml
- filename: punchh-platform-functions-headless-offers-openapi.yml
  format: yaml
  label: Punchh Headless Offers API - Platform Functions
  slug: punchh-platform-functions-headless-offers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-platform-functions-headless-offers-openapi.yml
- filename: punchh-platform-functions-offers-ingestion-openapi.yml
  format: yaml
  label: Punchh Offers Ingestion API - Platform Functions
  slug: punchh-platform-functions-offers-ingestion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-platform-functions-offers-ingestion-openapi.yml
- filename: punchh-platform-functions-subscription-openapi.yml
  format: yaml
  label: Punchh Subscription API - Platform Functions
  slug: punchh-platform-functions-subscription
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-platform-functions-subscription-openapi.yml
- filename: punchh-pos-api-openapi.yml
  format: yaml
  label: Punchh POS API
  slug: punchh-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-pos-api-openapi.yml
- filename: punchh-pos-redemptions-legacy-openapi.yml
  format: yaml
  label: Punchh Redemptions 1.0 (Legacy) API - POS
  slug: punchh-pos-redemptions-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-pos-redemptions-legacy-openapi.yml
- filename: punchh-pos-redemptions-v2-openapi.yml
  format: yaml
  label: Punchh Redemptions 2.0 (New) API - POS
  slug: punchh-pos-redemptions-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/openapi/punchh-pos-redemptions-v2-openapi.yml
consequence_counts:
  physical: 2
  read: 5
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Punchh Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/auth/checkins/online_order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/auth/redemptions/online_order
operation_count: 17
overview: 'Punchh exposes 17 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 10 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Punchh
provider_slug: punchh
slug: punchh-agentic-access
source_filename: punchh-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/punchh-mobile-openapi.yml, openapi/punchh-online-ordering-openapi.yml, openapi/punchh-platform-functions-openapi.yml,\n  openapi/punchh-pos-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 12\n    connected: 5\n  by_consequence:\n    write: 10\n    read: 5\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api2/mobile/users\n  method: post\n  operationId: createMobileUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api2/mobile/users\n  method: put\n  operationId: updateMobileUserProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api2/mobile/users/login\n  method: post\n  operationId: loginMobileUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api2/mobile/checkins/transactions\n  method: get\n  operationId: getCheckinTransactionDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api2/mobile/offers/mark_read\n\
  \  method: put\n  operationId: markOffersAsRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/checkins/online_order\n  method: post\n  operationId: createOnlineOrderCheckin\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/redemptions/online_order\n  method: post\n  operationId: createOnlineOrderRedemption\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api2/dashboard/redeemables\n  method: get\n  operationId: getRedeemableList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pos/users/search\n  method: get\n  operationId: searchPosUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pos/users\n  method: post\n  operationId: createPosUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pos/checkins\n\
  \  method: post\n  operationId: createPosCheckin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pos/locations/configuration\n  method: get\n  operationId: getPosLocationConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pos/meta\n  method: get\n  operationId: getPosProgramMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/pos/redemptions/possible\n  method: post\n  operationId: getPosPossibleRedemptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pos/redemptions\n  method: post\n  operationId: createPosRedemption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/pos/redemptions\n  method: delete\n  operationId: voidPosRedemption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /receipt_details\n  method: post\n  operationId: storeReceiptDetails\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/punchh/refs/heads/main/agentic-access/punchh-agentic-access.yml
summary_line: 17 operations · 12 acting
tags:
- Gift Cards
- Guest Engagement
- Loyalty
- Marketing
- Mobile
- Offers
- Online Ordering
- PAR Technology
- Point Of Sale
- Restaurant
- Restaurant Technology
- Webhooks
---
