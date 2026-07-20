---
acting_count: 93
action_class_counts:
  acting: 93
  connected: 37
api_specs:
- filename: deliverart-openapi.yml
  format: yaml
  label: Deliverart API
  slug: deliverart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-openapi.yml
consequence_counts:
  physical: 22
  read: 37
  safety-critical: 3
  write: 68
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Deliverart Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /password/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /password/reset/code/check
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /password/reset/code/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /delivery/order/{id}/delivered
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /delivery/{id}/end
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /delivery/{id}/take
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /me/customer/ownership/pos
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/cost/{id}/delete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/abort
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/cost/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/delete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/reserved/delivery/time
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/reserved/delivery/time/remove
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/reserved/take-away/time
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/reserved/take-away/time/remove
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/unset/customer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/unset/customer-address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/unset/customer-business-profile
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/update/customer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/update/customer-address
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/update/customer-business-profile
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/update/menu/items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/update/note
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /order/{id}/update/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pos/{id}/order/init
operation_count: 130
overview: 'Deliverart exposes 130 API operations that an AI agent could call, of which 93 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read, 68 write, 22 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Deliverart
provider_slug: deliverart
slug: deliverart-agentic-access
source_filename: deliverart-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/deliverart-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 130\n  by_action_class:\n    acting: 93\n    connected: 37\n  by_consequence:\n    write: 68\n    safety-critical: 3\n    read: 37\n    physical: 22\n  human_in_the_loop_required: 3\noperations:\n- path: /registration/register/customer\n  method: post\n  operationId: registrationRegisterCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registration/register/courier\n  method:\
  \ post\n  operationId: registrationRegisterCourier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registration/activate\n  method: post\n  operationId: registrationActivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /password/reset/code/request\n  method: post\n  operationId: passwordResetRequestCode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n     \
  \ proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /password/reset/code/check\n  method: post\n  operationId: passwordResetCheckValidCode\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /password/reset\n  method: post\n  operationId: passwordResetResetPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /me\n  method: get\n  operationId: meInfo\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/update\n  method: post\n  operationId: meUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/update/password\n  method: post\n  operationId: meUpdatePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/update/mobile-phone-number\n  method: post\n  operationId: meUpdateMobilePhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/verification/mobile/request\n  method: post\n  operationId: meVerificationMobilePhoneNumberRequest2faCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/verification/mobile/validate\n  method: post\n  operationId: meVerificationMobilePhoneNumberValidate2faCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/update/email\n  method:\
  \ post\n  operationId: meUpdateEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/verification/email/request\n  method: post\n  operationId: meVerificationEmailRequest2faCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/verification/email/validate\n  method: post\n  operationId: meVerificationEmailValidate2faCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/order/list\n  method: get\n  operationId: meOrderList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - order_admin\n    - order_list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/customer/detail/pos/{id}\n  method: get\n  operationId: meCustomerDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/customer/create\n  method: post\n  operationId: meCustomerCreateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/customer/ownership/pos\n  method: post\n  operationId:\
  \ meCustomerRedeemProfileByPos\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/customer/addresses/pos/{id}\n  method: get\n  operationId: meCustomerAddressList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/workshift/list\n  method: get\n  operationId: meWorkshiftList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/pos/list\n  method: get\n  operationId: mePosList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /company/{id}/detail\n  method: get\n  operationId: companiesDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - company_admin\n    - company_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/{id}/pos/list\n  method: get\n  operationId: companiesPosList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - company_admin\n    - company_pos_read\n    - company_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/{id}/detail\n  method: get\n  operationId: pointsOfSaleDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/{id}/customers\n  method: get\n  operationId: pointsOfSaleCustomersList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    scope:\n    - customer_admin\n    - point_of_sale_admin\n    - read_customer\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/{id}/workshifts\n  method: get\n  operationId: pointsOfSaleWorkshiftsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - point_of_sale_admin\n    - workshifts_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/{id}/delivery/fees\n  method: get\n  operationId: pointsOfSaleDeliveryFeesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - deliveries_fee_read\n    - point_of_sale_admin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/{id}/deliveries\n  method: get\n  operationId: pointsOfSaleDeliveriesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - deliveries_read\n    - point_of_sale_admin\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/{id}/customer/find/phone-number/{phoneNumber}\n  method: get\n  operationId: pointsOfSaleCustomersFindByPhoneNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customer_admin\n    - point_of_sale_admin\n    - read_customer\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/invitation/accept\n  method: post\n  operationId: pointsOfSaleInvitationAccept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/invitation/reject\n  method: post\n  operationId: pointsOfSaleInvitationReject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pos/{id}/settings\n  method: get\n  operationId: pointsOfSaleSettingsDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - point_of_sale_admin\n    - point_of_sale_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/{id}/settings/update\n  method: post\n  operationId: pointsOfSaleSettingsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - point_of_sale_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /address/{id}/detail\n  method: get\n  operationId: addressesDetail\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - address_admin\n    - address_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /address/create/coordinates\n  method: post\n  operationId: addressesCreateFromCoordinates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - address_admin\n    - address_create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /address/create/place-id\n  method: post\n  operationId: addressesCreateFromGooglePlaceId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - address_admin\n    - address_create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /customer/{id}/detail\n  method: get\n  operationId: customersDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customer_admin\n    - customer_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pos/{id}/customer/create\n  method: post\n  operationId: customersCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - create_customer\n    - customer_admin\n    - point_of_sale_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/{id}/update\n  method: post\n  operationId: customersUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer_admin\n    - customer_update\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/{id}/delete\n  method: post\n  operationId: customersDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_category_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/{id}/order/list\n  method: get\n  operationId: customersOrderList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customer_admin\n    - customer_orders_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/address/{customerId}/detail\n  method: get\n  operationId: customerAddressesDetail\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - customer_address_read\n    - customer_admin\n    - customer_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/{id}/address/create\n  method: post\n  operationId: customerAddressesCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer_address_create\n    - customer_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/address/{id}/update\n  method: post\n  operationId: customerAddressesUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer_address_update\n    - customer_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /customer/address/{id}/default\n  method: post\n  operationId: customerAddressesSetAsDefault\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer_address_update\n    - customer_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/address/{id}/delete\n  method: post\n  operationId: customerAddressesDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer_address_update\n    - customer_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/business-profile/{id}/detail\n  method: get\n  operationId:\
  \ customerBusinessProfilesDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customer_admin\n    - customer_business_profile_read\n    - customer_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/{id}/business-profile/create\n  method: post\n  operationId: customerBusinessProfilesCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer_admin\n    - customer_business_profile_create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/business-profile/{id}/update\n  method: post\n  operationId: customerBusinessProfilesUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer_admin\n    - customer_business_profile_update\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/business-profile/{id}/default\n  method: post\n  operationId: customerBusinessProfilesSetAsDefault\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer_admin\n    - customer_business_profile_update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/business-profile/{id}/delete\n  method: post\n  operationId: customerBusinessProfilesDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - customer_admin\n    - customer_business_profile_update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/{id}/detail\n  method: get\n  operationId: menuDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /menu/create\n  method: post\n  operationId: menuCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/{id}/update\n  method: post\n  operationId: menuUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /menu/categories\n  method: get\n  operationId: menuCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /menu/category/{id}/detail\n  method: get\n  operationId: menuCategoriesDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - menu_admin\n    - menu_item_category_admin\n    - menu_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /menu/category/create\n  method: post\n  operationId: menuCategoriesCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/category/{id}/update\n  method: post\n  operationId:\
  \ menuCategoriesUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_category_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/allergen/{id}/category/meta\n  method: post\n  operationId: menuCategoriesUpdateMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_category_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/category/{id}/delete\n  method: post\n  operationId: menuCategoriesDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - menu_admin\n    - menu_item_category_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/category/{id}/translate\n  method: post\n  operationId: menuCategoriesTranslate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_category_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/category/{id}/sort\n  method: post\n  operationId: menuCategoriesSort\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_category_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/category/{id}/media/upload\n  method: post\n  operationId: menuCategoriesMediaUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_category_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/category/{id}/media/remove\n  method: post\n  operationId: menuCategoriesMediaRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_category_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/allergens\n  method:\
  \ get\n  operationId: menuAllergens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /menu/allergen/{id}/detail\n  method: get\n  operationId: menuAllergensDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - menu_admin\n    - menu_item_allergen_admin\n    - menu_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /menu/allergen/create\n  method: post\n  operationId: menuAllergensCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/allergen/{id}/update\n  method: post\n  operationId: menuAllergensUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_allergen_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/allergen/{id}/update/meta\n  method: post\n  operationId: menuAllergensUpdateMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_allergen_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/allergen/{id}/delete\n  method: post\n  operationId: menuAllergensDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_allergen_admin\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/allergen/{id}/translate\n  method: post\n  operationId: menuAllergensTranslate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_allergen_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/ingredients\n  method: get\n  operationId: menuIngredients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /menu/ingredient/{id}/detail\n  method: get\n  operationId: menuIngredientsDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - menu_admin\n\
  \    - menu_item_ingredient_admin\n    - menu_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /menu/ingredient/create\n  method: post\n  operationId: menuIngredientsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/ingredient/{id}/update\n  method: post\n  operationId: menuIngredientsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_ingredient_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/ingredient/{id}/update/meta\n  method: post\n  operationId: menuIngredientsUpdateMetadata\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_ingredient_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/ingredient/{id}/delete\n  method: post\n  operationId: menuIngredientsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_ingredient_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/ingredient/{id}/translate\n  method: post\n  operationId: menuIngredientsTranslate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n  \
  \  - menu_item_ingredient_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/item/{id}/detail\n  method: get\n  operationId: menuItemsDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /menu/item/create\n  method: post\n  operationId: menuItemsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/item/{id}/update\n  method: post\n  operationId: menuItemsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n  \
  \  - menu_item_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/item/{id}/update/meta\n  method: post\n  operationId: menuItemsUpdateMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/item/{id}/delete\n  method: post\n  operationId: menuItemsDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /menu/item/{id}/suspend\n  method: post\n  operationId: menuItemsSuspend\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/item/{id}/resume\n  method: post\n  operationId: menuItemsResume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /menu/item/{id}/translate\n  method: post\n  operationId: menuItemsTranslate\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - menu_admin\n    - menu_item_ingredient_admin\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workshift/{id}/detail\n  method: get\n  operationId: workshiftsDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workshifts_admin\n    - workshifts_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workshift/{workshiftId}/address/{addressId}/delivery/times\n  method: get\n  operationId: workshiftsDeliveryTimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - workshifts_admin\n    - workshifts_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workshift/{workshiftId}/take-away/times\n  method: get\n  operationId: workshiftsTakeAwayTimes\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - take_away_time_read\n    - workshifts_admin\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workshift/invitation/accept\n  method: post\n  operationId: workshiftsInvitationAccept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workshift/invitation/reject\n  method: post\n  operationId: workshiftsInvitationReject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/fee/{id}/detail\n  method:\
  \ get\n  operationId: deliveryFeeDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - delivery_admin\n    - delivery_fee_admin\n    - delivery_fee_\n\n# --- truncated at 32 KB (47 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/agentic-access/deliverart-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/agentic-access/deliverart-agentic-access.yml
summary_line: 130 operations · 93 acting · 3 human-in-the-loop
tags:
- Company
- Food Delivery
- Restaurants
- Order Management
- Logistics
- Delivery
- Menu Management
- Point of Sale
---
