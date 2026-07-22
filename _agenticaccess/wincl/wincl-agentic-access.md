---
acting_count: 127
action_class_counts:
  acting: 127
  connected: 144
api_specs:
- filename: wincl-openapi-original.json
  format: json
  label: Wincl API
  slug: wincl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wincl/refs/heads/main/openapi/wincl-openapi-original.json
consequence_counts:
  physical: 29
  read: 144
  safety-critical: 1
  write: 97
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Wincl Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /bapi/v1/auth/clear-firebase-claim
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/order/one-dollar-product
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/order/stripe/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/order/stripe/create-payment-intent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/order/stripe/reserve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/utils/sms/message
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/wallet/credit/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/wallet/credit/transfer/test
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/order/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payment/kcp/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payment/kcp/reserve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payment/payco/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payment/payco/reserve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payment/stripe/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payment/stripe/reserve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payment/stripe/test/reserve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payment/stripe/webhook
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v3/rewards/internal/programs/{programId}/orders/{orderId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v3/rewards/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v3/rewards/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v3/rewards/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bapi/v1/hedera/contracts/paymaster/deposit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bapi/v1/hedera/contracts/paymaster/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bapi/v1/hedera/contracts/registry/transfer-record
operation_count: 271
overview: 'WinCL exposes 271 API operations that an AI agent could call, of which 127 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 144 read, 97 write, 29 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WinCL
provider_slug: wincl
slug: wincl-agentic-access
source_filename: wincl-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/wincl-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 271\n  by_action_class:\n    acting: 127\n    connected: 144\n  by_consequence:\n    safety-critical: 1\n    write: 97\n    read: 144\n    physical: 29\n  human_in_the_loop_required: 1\noperations:\n- path: /bapi/v1/auth/clear-firebase-claim\n  method: post\n  operationId: passwordResetUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /bapi/v1/auth/forgot-password\n  method: post\n  operationId: requestForgotPasswordUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/auth/signin\n  method: post\n  operationId: signInUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/admin\n  method: get\n  operationId: getAdminListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/admin\n  method: post\n  operationId: createAdminUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/admin/authority\n  method: get\n  operationId: getAuthoritiesUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/admin/profile\n  method: get\n  operationId: getAdminProfileUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/admin/tab\n  method: get\n  operationId:\
  \ getTabListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/admin/{id}\n  method: get\n  operationId: getAdminDetailUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/admin/{id}\n  method: put\n  operationId: updateAdminUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/admin/{id}\n  method: delete\n  operationId: deleteAdminUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v2/coupons/events/{eventId}\n  method: delete\n  operationId: deleteEventUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v2/coupons/magic/issue\n  method: post\n  operationId: issueIndividualCouponsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /bapi/v2/coupons/magic/register\n  method: post\n  operationId: registerMagicCouponsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/faq\n  method: get\n  operationId: getFaqByCategoryUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/faq\n  method: post\n  operationId: createFaqUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/faq/category\n  method: get\n  operationId: getFaqCategoryUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/faq/{id}\n  method: get\n  operationId: getFaqUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/faq/{id}\n  method: put\n  operationId: updateFaqUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/faq/{id}\n  method: delete\n  operationId: deleteFaqUsingDELETE\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/hedera/info\n  method: get\n  operationId: getHederaInfoUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/hedera/migrate-operator\n  method: post\n  operationId: migrateOperatorUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/hedera/transfer\n  method:\
  \ post\n  operationId: transferHbarUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/info/banner\n  method: get\n  operationId: bannerListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/info/banner\n  method: post\n  operationId: insertBannerUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /bapi/v1/info/banner/hide\n  method: delete\n  operationId: hideBannerUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/info/banner/show/{id}\n  method: get\n  operationId: showBannerUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/info/banner/{id}\n  method: get\n  operationId: getBannerUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/info/banner/{id}\n  method: put\n\
  \  operationId: modifyBannerUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/info/banner/{id}\n  method: delete\n  operationId: deleteBannerUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/info/popup\n  method: get\n  operationId: popupListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/info/popup\n\
  \  method: post\n  operationId: insertPopupUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/info/popup/hide\n  method: delete\n  operationId: hidePopupsUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/info/popup/show/{id}\n  method: put\n  operationId: showPopupUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/info/popup/{id}\n  method: get\n  operationId: getPopupUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/info/popup/{id}\n  method: put\n  operationId: modifyPopupUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/info/popup/{id}\n  method: delete\n  operationId: deletePopupUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/news\n  method: get\n  operationId: getNewsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/news\n  method: post\n  operationId: insertNewsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/news/category\n  method: get\n  operationId: getNewsCategoryListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/news/category\n  method: post\n  operationId: addNewsCategoryUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/news/category\n  method: delete\n  operationId: removeNewsCategoryUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/news/{no}\n  method: get\n  operationId: getNewsDetailUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/news/{no}\n  method: put\n  operationId: updateNewsUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/news/{no}\n  method: delete\n  operationId: deleteNewsUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/notice\n  method: get\n  operationId: noticeListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/notice\n  method: post\n  operationId: insertNoticeUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/notice/active\n  method: get\n  operationId: activeNoticeListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/notice/{id}\n  method: get\n  operationId: noticeInfoUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /bapi/v1/notice/{id}\n  method: put\n  operationId: modifyNoticeUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/notice/{id}\n  method: delete\n  operationId: deleteNoticeUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/order/list\n  method: get\n  operationId: orderListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /bapi/v1/order/{id}\n  method: get\n  operationId: orderInfoUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v2/payment/{purchaseId}/cancel\n  method: post\n  operationId: refundPaymentUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/product\n  method: get\n  operationId: productListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/product\n\
  \  method: post\n  operationId: insertProductUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/product/home\n  method: get\n  operationId: homeProductsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/product/home/{id}\n  method: put\n  operationId: updateHomeProductUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/product/home/{id}\n  method: post\n  operationId: addHomeProductUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/product/home/{id}\n  method: delete\n  operationId: removeHomeProductUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/product/{id}\n  method: get\n  operationId: productInfoUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/product/{id}\n  method: put\n  operationId: modifyProductUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/product/{id}\n  method: delete\n  operationId: deleteProductUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/product/{id}/history\n  method: get\n  operationId: productBalanceHistoryListUsingGET\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/product/{id}/increment\n  method: put\n  operationId: updateVolumeUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/project\n  method: get\n  operationId: projectListUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/project\n  method: post\n  operationId: insertProjectUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/project/agency\n  method: get\n  operationId: getCertificationAgencyUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/project/effect/list\n  method: get\n  operationId: projectEffectListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/project/type/list\n  method: get\n  operationId: projectTypeListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/project/{id}\n\
  \  method: get\n  operationId: projectInfoUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/project/{id}\n  method: put\n  operationId: modifyProjectUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/project/{id}/history\n  method: get\n  operationId: projectListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/project/{id}/increment\n  method: put\n  operationId: updateVolumeUsingPUT_1\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/qna\n  method: get\n  operationId: qnaListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/qna/{id}\n  method: get\n  operationId: qnaInfoUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v1/qna/{id}/answer\n  method: put\n  operationId: updateQnaAnswerUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/qna/{id}/answer\n  method: post\n  operationId: insertQnaAnswerUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/qna/{id}/answer\n  method: delete\n  operationId: deleteQnaAnswerUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v3/rewards/companies\n  method: get\n  operationId:\
  \ listUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v3/rewards/companies\n  method: post\n  operationId: createUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v3/rewards/companies/{id}\n  method: get\n  operationId: getUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v3/rewards/companies/{id}\n  method: put\n  operationId: updateUsingPUT\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v3/rewards/companies/{id}\n  method: delete\n  operationId: deleteUsingDELETE\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v3/rewards/issuances\n  method: get\n  operationId: listUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v3/rewards/issuances/{id}\n  method: get\n  operationId: getUsingGET_1\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v3/rewards/issuances/{id}\n  method: delete\n  operationId: deleteUsingDELETE_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v3/rewards/orders\n  method: get\n  operationId: listAllUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v3/rewards/orders/{id}\n  method: get\n  operationId: getUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /bapi/v3/rewards/orders/{id}\n  method: delete\n  operationId: deleteUsingDELETE_2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v3/rewards/orders/{id}/cancel/approve\n  method: post\n  operationId: approveCancelUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v3/rewards/programs/{programId}/orders\n  method:\
  \ get\n  operationId: listByProgramUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v3/rewards/payments\n  method: get\n  operationId: listUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v3/rewards/payments/{id}\n  method: get\n  operationId: getUsingGET_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v3/rewards/companies/{companyId}/programs\n  method: get\n  operationId: listByCompanyUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /bapi/v3/rewards/programs\n  method: get\n  operationId: listUsingGET_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v3/rewards/programs\n  method: post\n  operationId: createUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v3/rewards/programs/{id}\n  method: get\n  operationId: getUsingGET_4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - global\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bapi/v3/rewards/programs/{id}\n  method: put\n  operationId: updateUsingPUT_1\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v3/rewards/programs/{id}\n  method: delete\n  operationId: deleteUsingDELETE_3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/hedera/contracts/carbon-token/balance\n  method: post\n  operationId: getTokenBalanceUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - global\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bapi/v1/hedera/contracts/carbon-token/metadata\n  method: post\n  operationId: getTokenMetadataUsingPOS\n\n# --- truncated at 32 KB (84 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/wincl/refs/heads/main/agentic-access/wincl-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wincl/refs/heads/main/agentic-access/wincl-agentic-access.yml
summary_line: 271 operations · 127 acting · 1 human-in-the-loop
tags:
- Company
- Carbon Management
- Sustainability
- Greenhouse Gas
- Carbon Credits
- Carbon Offset
- ESG
- Climate
- Marketplace
- Payments
- Blockchain
- Hedera
---
