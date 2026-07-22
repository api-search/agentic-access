---
acting_count: 126
action_class_counts:
  acting: 126
  connected: 226
api_specs:
- filename: mirakl-mmp-seller-openapi.json
  format: json
  label: Mirakl Marketplace Platform — Seller API
  slug: mirakl-marketplace-platform-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mmp-seller-openapi.json
- filename: mirakl-mmp-operator-openapi.json
  format: json
  label: Mirakl Marketplace Platform — Operator API
  slug: mirakl-marketplace-platform-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mmp-operator-openapi.json
- filename: mirakl-mms-seller-openapi.json
  format: json
  label: Mirakl Platform for Services — Seller API
  slug: mirakl-platform-for-services-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mms-seller-openapi.json
- filename: mirakl-mms-operator-openapi.json
  format: json
  label: Mirakl Platform for Services — Operator API
  slug: mirakl-platform-for-services-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mms-operator-openapi.json
- filename: mirakl-mcm-seller-openapi.json
  format: json
  label: Mirakl Catalog Manager — Seller API
  slug: mirakl-catalog-manager-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mcm-seller-openapi.json
- filename: mirakl-mcm-operator-openapi.json
  format: json
  label: Mirakl Catalog Manager — Operator API
  slug: mirakl-catalog-manager-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mcm-operator-openapi.json
- filename: mirakl-connect-channel-openapi.json
  format: json
  label: Mirakl Connect Channel Platform API
  slug: mirakl-connect-channel-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-connect-channel-openapi.json
consequence_counts:
  physical: 61
  read: 226
  write: 65
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mirakl Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/mms/orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/mms/orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/mms/orders/{order_id}/accept
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/mms/orders/{order_id}/accept
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/mms/orders/{order_id}/consume
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/mms/orders/{order_id}/consume
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/mms/orders/{order_id}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/mms/orders/{order_id}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/mms/orders/{order_id}/refuse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/mms/orders/{order_id}/refuse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mms/orders/{order_id}/threads
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mms/orders/{order_id}/threads
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders/adjust
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders/adjust
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/async-export
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/orders/async-export
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/orders/documents/{document_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/orders/documents/{document_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/orders/shipping_from
operation_count: 352
overview: 'Mirakl exposes 352 API operations that an AI agent could call, of which 126 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 226 read, 65 write, and 61 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mirakl
provider_slug: mirakl
slug: mirakl-agentic-access
source_filename: mirakl-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/mirakl-mcm-operator-openapi.json, openapi/mirakl-mcm-seller-openapi.json, openapi/mirakl-mmp-operator-openapi.json,\n  openapi/mirakl-mmp-seller-openapi.json, openapi/mirakl-mms-operator-openapi.json, openapi/mirakl-mms-seller-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 352\n  by_action_class:\n    connected: 226\n    acting: 126\n  by_consequence:\n    read: 226\n    write: 65\n    physical: 61\n  human_in_the_loop_required: 0\noperations:\n- path: /api/additional_fields\n  method: get\n  operationId: AF01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/channels\n\
  \  method: get\n  operationId: CH11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcm/products/sources/status/export\n  method: get\n  operationId: CM11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/currencies\n  method: get\n  operationId: CUR01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents\n  method: get\n  operationId: DO01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hierarchies\n  method: get\n  operationId: H11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /api/locales\n  method: get\n  operationId: L01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports\n  method: post\n  operationId: P41\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/products/imports\n  method: get\n  operationId: P51\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}\n  method: get\n  operationId: P42\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/products/imports/{import}/error_report\n  method: get\n  operationId: P44\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}/new_product_report\n  method: get\n  operationId: P45\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}/transformed_file\n  method: get\n  operationId: P46\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}/transformation_error_report\n  method: get\n  operationId: P47\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/configuration\n\
  \  method: get\n  operationId: PC01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/attributes\n  method: get\n  operationId: PM11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/shops/roles\n  method: get\n  operationId: RO02\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/shops/documents\n  method: get\n  operationId: S30\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/shops/documents\n  method: post\n  operationId: S32\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/shops/documents/download\n  method: get\n  operationId: S31\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/shops/documents/{document_id}\n  method: delete\n  operationId: S33\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/values_lists\n  method: get\n  operationId: VL11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account\n  method: get\n  operationId:\
  \ A01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_SHOP_READ\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/account\n  method: put\n  operationId: A02\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ROLE_PARTNER_SHOP_UPDATE\n    - ROLE_SHOP_ADMIN\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/account/statistics\n  method: get\n  operationId: A21\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_SHOP_READ\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/additional_fields\n  method: get\n  operationId: AF01\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_OFFER_SETTINGS_READ\n    - ROLE_PARTNER_ORDER_SETTINGS_READ\n    - ROLE_PARTNER_SHOP_SETTINGS_READ\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/channels\n  method: get\n  operationId: CH11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_CHANNEL_READ\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcm/products/sources/status/export\n  method: get\n  operationId: CM11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_PRODUCT_SOURCE_READ\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/currencies\n  method: get\n  operationId: CUR01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - ROLE_PARTNER_CURRENCY_SETTINGS_READ\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents\n  method: get\n  operationId: DO01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_ORDER_SETTINGS_READ\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/hierarchies\n  method: get\n  operationId: H11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/locales\n  method: get\n  operationId: L01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_I18N_SETTINGS_READ\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports\n  method: post\n  operationId: P41\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - ROLE_PARTNER_PRODUCT_WRITE\n    - ROLE_SHOP_ADMIN\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/products/imports\n  method: get\n  operationId: P51\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_PRODUCT_WRITE\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}\n  method: get\n  operationId: P42\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_PRODUCT_WRITE\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}/error_report\n  method: get\n  operationId: P44\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_PRODUCT_WRITE\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}/new_product_report\n  method: get\n  operationId: P45\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_PRODUCT_WRITE\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}/transformed_file\n  method: get\n  operationId: P46\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_PRODUCT_WRITE\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}/transformation_error_report\n  method: get\n  operationId: P47\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - ROLE_PARTNER_PRODUCT_WRITE\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/configuration\n  method: get\n  operationId: PC01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/attributes\n  method: get\n  operationId: PM11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/shops/roles\n  method: get\n  operationId: RO02\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_SHOP_USER_CREATE\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/shops/documents\n  method: get\n  operationId: S30\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - ROLE_PARTNER_SHOP_DOCUMENT_READ\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/shops/documents\n  method: post\n  operationId: S32\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ROLE_PARTNER_SHOP_DOCUMENT_WRITE\n    - ROLE_SHOP_ADMIN\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/shops/documents/download\n  method: get\n  operationId: S31\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ROLE_PARTNER_SHOP_DOCUMENT_READ\n    - ROLE_SHOP_ADMIN\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/shops/documents/{document_id}\n  method: delete\n  operationId: S33\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - ROLE_PARTNER_SHOP_DOCUMENT_DELETE\n    - ROLE_SHOP_ADMIN\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/version\n  method: get\n  operationId: V01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/values_lists\n  method: get\n  operationId: VL11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/additional_fields\n  method: get\n  operationId: AF01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/channels\n  method: get\n  operationId: CH11\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/currencies\n  method: get\n  operationId: CUR01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/documents\n  method: get\n  operationId: DO01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/document-request/requests\n  method: get\n  operationId: DR11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/document-request/{document_request_id}/lines\n  method: get\n  operationId: DR12\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/document-request/documents/download\n  method: get\n  operationId: DR73\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/document-request/documents/upload\n  method: post\n  operationId: DR74\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/hierarchies\n  method: get\n  operationId: H11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/invoices\n  method: get\n  operationId: IV01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/invoices/{accounting_document_id}\n  method: get\n  operationId: IV02\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/locales\n  method: get\n  operationId: L01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/messages\n  method: get\n  operationId: M01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/inbox/threads/{thread_id}\n  method: get\n  operationId: M10\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/inbox/threads\n  method: get\n  operationId: M11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/inbox/threads\n  method: post\n  operationId: M14\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inbox/threads/{thread_id}/message\n  method: post\n  operationId: M12\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/inbox/threads/{attachment_id}/download\n  method: get\n  operationId: M13\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/offers/imports\n  method: post\n  operationId: OF01\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/offers/imports\n  method: get\n  operationId: OF04\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/offers/imports/{import}\n  method: get\n  operationId: OF02\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/offers/imports/{import}/error_report\n  method: get\n  operationId: OF03\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /api/offers/{offer}\n  method: get\n  operationId: OF22\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/offers\n  method: post\n  operationId: OF24\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/offers/{offer}/quantity\n  method: get\n  operationId: OF26\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/offers/export\n  method: get\n  operationId: OF51\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/offers/export/async\n  method: post\n  operationId: OF52\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/offers/export/async/status/{tracking_id}\n  method: get\n  operationId: OF53\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dynamic-url/The+URL+is+retrieved+from+OF53+output/OF54\n  method: get\n  operationId: OF54\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/offers/states\n  method: get\n  operationId: OF61\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/orders\n  method: put\n  operationId: OR04\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders\n  method: get\n  operationId: OR11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/taxes\n  method: get\n  operationId: OR75\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/shipping_from\n  method: put\n  operationId: OR07\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_id}\n  method: get\n  operationId: OR12\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/async-export\n  method: post\n  operationId: OR13\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/async-export/status/{tracking_id}\n  method: get\n  operationId: OR14\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dynamic-url/The+URL+is+retrieved+from+OR14+output/OR15\n  method: get\n  operationId: OR15\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/{order_id}/accept\n  method: put\n  operationId: OR21\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_id}/tracking\n  method: put\n  operationId: OR23\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_id}/ship\n  method: put\n  operationId: OR24\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_id}/refund\n  method: put\n  operationId: OR26\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/refund\n  method: put\n  operationId:\
  \ OR28\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_id}/cancel\n  method: put\n  operationId: OR29\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/cancel\n  method: put\n  operationId: OR30\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_id}/additional_fields\n  method: put\n  operationId: OR31\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/adjust\n  method: put\n  operationId: OR32\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_id}/messages\n  method:\
  \ get\n  operationId: OR41\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/{order_id}/messages\n  method: post\n  operationId: OR42\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/{order_id}/threads\n  method: post\n  operationId: OR43\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/orders/{order_id}/evaluation\n  method: get\n  operationId: OR51\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/documents\n  method: get\n  operationId: OR72\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/documents/download\n  method: get\n  operationId: OR73\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/orders/{order_id}/documents\n  method: post\n  operationId: OR74\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/orders/documents/{document_id}\n  method: delete\n  operationId: OR76\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/products/offers\n  method: get\n  operationId: P11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products\n  method: get\n  operationId: P31\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports\n  method: post\n  operationId: P41\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/products/imports\n  method: get\n  operationId: P51\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}\n  method: get\n  operationId: P42\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}/error_report\n  method: get\n  operationId: P44\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}/new_product_report\n  method: get\n  operationId: P45\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}/transformed_file\n  method: get\n  operationId: P46\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/products/imports/{import}/transformation_error_report\n  method: get\n  operationId: P47\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/platform/configuration\n  method: get\n  operationId: PC01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/picklists\n  method: get\n  operationId: PL11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/products/attributes\n  method: get\n  operationId: PM11\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/promotions\n  method: get\n  operationId: PR01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/promotions\n  method: post\n  operationId: PR03\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/promotions/{promotion_internal_id}\n  method: put\n  operationId: PR04\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/offers/pricing/imports\n  method: post\n  operationId: PRI01\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/offers/pricing/imports\n  method: get\n  operationId: PRI02\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/offers/pricing/imports/{import_id}/error_report\n  method: get\n  operationId: PRI03\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reasons\n\
  \  method: get\n  operationId: RE01\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reasons/{reason_type}\n  method\n\n# --- truncated at 32 KB (101 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/agentic-access/mirakl-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/agentic-access/mirakl-agentic-access.yml
summary_line: 352 operations · 126 acting
tags:
- Company
- Commerce
- eCommerce
- Marketplace
- Dropship
- Retail
- Catalog
- Orders
- Retail Media
- B2B
---
