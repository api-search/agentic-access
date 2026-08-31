---
acting_count: 41
action_class_counts:
  acting: 41
  connected: 26
api_specs:
- filename: push-account-api-openapi.yml
  format: yaml
  label: Push Account API
  slug: push-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-account-api-openapi.yml
- filename: push-audience-list-api-openapi.yml
  format: yaml
  label: Push Audience List API
  slug: push-audience-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-audience-list-api-openapi.yml
- filename: push-campaigns-api-openapi.yml
  format: yaml
  label: Push Campaigns API
  slug: push-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-campaigns-api-openapi.yml
- filename: push-company-api-openapi.yml
  format: yaml
  label: Push Company API
  slug: push-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-company-api-openapi.yml
- filename: push-company-custom-fields-api-openapi.yml
  format: yaml
  label: Push Company custom fields API
  slug: push-company-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-company-custom-fields-api-openapi.yml
- filename: push-contact-api-openapi.yml
  format: yaml
  label: Push Contact API
  slug: push-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-contact-api-openapi.yml
- filename: push-contact-custom-fields-api-openapi.yml
  format: yaml
  label: Push Contact Custom fields API
  slug: push-contact-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-contact-custom-fields-api-openapi.yml
- filename: push-coupon-lists-api-openapi.yml
  format: yaml
  label: Push Coupon lists API
  slug: push-coupon-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-coupon-lists-api-openapi.yml
- filename: push-deliveries-api-openapi.yml
  format: yaml
  label: Push Deliveries API
  slug: push-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-deliveries-api-openapi.yml
- filename: push-hotel-data-api-openapi.yml
  format: yaml
  label: Push Hotel Data API
  slug: push-hotel-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-hotel-data-api-openapi.yml
- filename: push-hotel-data-custom-fields-api-openapi.yml
  format: yaml
  label: Push Hotel Data custom fields API
  slug: push-hotel-data-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-hotel-data-custom-fields-api-openapi.yml
- filename: push-product-api-openapi.yml
  format: yaml
  label: Push Product API
  slug: push-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-product-api-openapi.yml
- filename: push-product-custom-fields-api-openapi.yml
  format: yaml
  label: Push Product custom fields API
  slug: push-product-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-product-custom-fields-api-openapi.yml
- filename: push-purchase-api-openapi.yml
  format: yaml
  label: Push Purchase API
  slug: push-purchase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-purchase-api-openapi.yml
- filename: push-sync-data-api-openapi.yml
  format: yaml
  label: Push Sync Data API
  slug: push-sync-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/openapi/push-sync-data-api-openapi.yml
consequence_counts:
  physical: 7
  read: 26
  write: 34
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Push Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/account/{account_id}/contact/{contact_id}/purchases
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/account/{account_id}/email/deliveries
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/account/{account_id}/purchases/delete_group
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/account/{account_id}/purchases/{purchase_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/account/{account_id}/purchases/{purchase_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/account/{account_id}/push/deliveries
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/account/{account_id}/sms/deliveries
operation_count: 67
overview: 'Push exposes 67 API operations that an AI agent could call, of which 41 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 34 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Push
provider_slug: push
slug: push-agentic-access
source_filename: push-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/push-cendyn-crm-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 67\n  by_action_class:\n    connected: 26\n    acting: 41\n  by_consequence:\n    read: 26\n    write: 34\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/account/{account_id}/balance/current\n  method: get\n  operationId: currentBalanceAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/sync_data\n  method: post\n  operationId: createSyncData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/sync_data/{id}\n  method: get\n  operationId: showSyncData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/contact\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/contact\n  method: get\n  operationId: listContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v2/account/{account_id}/contact/bulk\n  method: post\n  operationId: createBulkContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/contact/bulk/{bulk_id}\n  method: get\n  operationId: getBulkContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/contact/{contact_id}\n  method: get\n  operationId: showContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/contact/{contact_id}\n  method: put\n  operationId: updateContact\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/contact/{contact_id}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/contact/{contact_id}/email_validation\n  method: get\n  operationId: emailValidationContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/custom_fields\n  method: post\n  operationId: createContactCustomFields\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/custom_fields\n  method: get\n  operationId: listContactCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/custom_fields/{custom_id}\n  method: put\n  operationId: updateContactCustomFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/custom_fields/{custom_id}\n  method: delete\n \
  \ operationId: deleteContactCustomFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/company\n  method: post\n  operationId: createCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/company\n  method: get\n  operationId: listCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/company/{company_id}\n  method: get\n  operationId:\
  \ showCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/company/{company_id}\n  method: put\n  operationId: updateCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/company/{company_id}\n  method: delete\n  operationId: deleteCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/company_custom_fields\n  method: post\n  operationId:\
  \ createCompanyCustomFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/company_custom_fields\n  method: get\n  operationId: listCompanyCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/company_custom_fields/{custom_id}\n  method: put\n  operationId: updateCompanyCustomFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/company_custom_fields/{custom_id}\n\
  \  method: delete\n  operationId: deleteCompanyCustomFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/campaigns/{campaign_id}\n  method: get\n  operationId: showCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/campaigns/{campaign_id}/message/contact/{contact_id}\n  method: get\n  operationId: previewMessageCampaigns\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/products\n  method: post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/products\n  method: get\n  operationId: listProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/products/{UUID}\n  method: get\n  operationId: showProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/products/{UUID}\n  method:\
  \ put\n  operationId: updateProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/products/{UUID}\n  method: delete\n  operationId: deleteProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/product_custom_fields\n  method: post\n  operationId: createProductCustomFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/product_custom_fields\n  method: get\n  operationId: listProductCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/product_custom_fields/{product_custom_id}\n  method: put\n  operationId: updateProductCustomFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/product_custom_fields/{product_custom_id}\n  method: delete\n  operationId: deleteProductCustomFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/coupon_lists\n  method: post\n  operationId: createCouponLists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/coupon_lists\n  method: get\n  operationId: listCouponLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/coupon_lists/{coupon_list_id}\n  method: get\n  operationId: showCouponLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/account/{account_id}/coupon_lists/{coupon_list_id}\n  method: put\n  operationId: updateCouponLists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/coupon_lists/{coupon_list_id}\n  method: delete\n  operationId: deleteCouponLists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/coupon_lists/redeem\n  method: put\n  operationId: redeemCouponLists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/contact/{contact_id}/purchases\n  method: post\n  operationId: createPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/purchases/{purchase_id}\n  method: put\n  operationId: updatePurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/purchases/{purchase_id}\n  method: delete\n  operationId: deletePurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/purchases\n  method: get\n  operationId: listPurchase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/purchases/delete_group\n  method: delete\n  operationId: deleteGroupPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/hotel_data/{uuid}/add_language\n  method: put\n  operationId: addLanguageHotelData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/hotel_data\n  method: post\n  operationId: createHotelHotelData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/hotel_data\n  method: get\n \
  \ operationId: listHotelData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/hotel_data/{uuid}\n  method: delete\n  operationId: deleteHotelData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/hotel_data/{uuid}\n  method: get\n  operationId: showHotelData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/hotel_data/{uuid}/remove_language\n  method: delete\n  operationId: removeLanguageHotelData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/hotel_data_custom_fields\n  method: post\n  operationId: createHotelDataCustomFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/hotel_data_custom_fields\n  method: get\n  operationId: listHotelDataCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/hotel_data_custom_fields/{custom_id}\n  method: put\n  operationId: updateHotelDataCustomFields\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/hotel_data_custom_fields/{custom_id}\n  method: delete\n  operationId: deleteHotelDataCustomFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/email/deliveries\n  method: post\n  operationId: sendEmailDeliveries\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/push/deliveries\n  method: post\n  operationId: sendPushDeliveries\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/sms/deliveries\n  method: post\n  operationId: sendSMSDeliveries\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/delivery/{delivery_id}\n\
  \  method: get\n  operationId: showDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/deliveries\n  method: get\n  operationId: listDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/lists\n  method: post\n  operationId: createAudienceList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/lists\n  method: get\n  operationId: listAudienceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/lists/{id}\n  method: get\n  operationId: showAudienceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/lists/{id}\n  method: put\n  operationId: updateAudienceList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}/lists/{id}\n  method: delete\n  operationId: deleteAudienceList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/push/refs/heads/main/agentic-access/push-agentic-access.yml
summary_line: 67 operations · 41 acting
tags:
- Company
- CRM
- Customer Data Platform
- Marketing Automation
- Hospitality
- Hotels
- Guest Experience
- Email
- SMS
- Push Notifications
- Webhook
- Segmentation
---
