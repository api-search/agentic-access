---
acting_count: 69
action_class_counts:
  acting: 69
  connected: 39
api_specs:
- filename: route-mobile-sms.yml
  format: yaml
  label: Route Mobile SMS API
  slug: route-mobile-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-sms.yml
- filename: route-mobile-whatsapp-business.yml
  format: yaml
  label: Route Mobile WhatsApp Business API
  slug: route-mobile-whatsapp-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-whatsapp-business.yml
- filename: route-mobile-rcs.yml
  format: yaml
  label: Route Mobile RCS Business Messaging API
  slug: route-mobile-rcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-rcs.yml
- filename: route-mobile-viber.yml
  format: yaml
  label: Route Mobile Viber Business Messages API
  slug: route-mobile-viber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-viber.yml
- filename: route-mobile-sendclean-email.yml
  format: yaml
  label: SendClean Email API
  slug: sendclean-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-sendclean-email.yml
- filename: Enterprise-Voice-2.0-APIs
  format: yaml
  label: Route Mobile Enterprise Voice 2.0 API
  slug: route-mobile-enterprise-voice-api
  spec_type: Postman
  url: https://github.com/routemobile/Enterprise-Voice-2.0-APIs
consequence_counts:
  physical: 15
  read: 39
  safety-critical: 3
  write: 51
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Route Mobile Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /rcs/v2/revoke_message
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /settings/keyResetWebhook
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /settings/resetSmtpPassword
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bulksms/jsonbulksms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bulksms2346/sendjsonsms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages/sendMail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages/sendTemplate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/send_bill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /settings/addSendingDomain
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /settings/checkSendingDomain
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /settings/deleteSendingDomain
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /settings/listSendingDomain
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /settings/verifySendingDomain
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vbs/api/v2/manage-campaign
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vbs/api/v2/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vbs/api/v3/send_bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wba/v1/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wba/v2/manage_campaign
operation_count: 108
overview: 'Route Mobile exposes 108 API operations that an AI agent could call, of which 69 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 39 read, 51 write, 15 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Route Mobile
provider_slug: route-mobile
slug: route-mobile-agentic-access
source_filename: route-mobile-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/route-mobile-rcs.yml, openapi/route-mobile-sendclean-email.yml, openapi/route-mobile-sms.yml,\n  openapi/route-mobile-viber.yml, openapi/route-mobile-whatsapp-business.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 108\n  by_action_class:\n    acting: 69\n    connected: 39\n  by_consequence:\n    write: 51\n    physical: 15\n    read: 39\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /auth/v1/login/\n  method: post\n  operationId: loginApi2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /rcs/v1/message\n  method: post\n  operationId: textTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcs/v1/bulk_message\n  method: post\n  operationId: bulkCampaignUploadRCS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/v1/send_bill\n  method: post\n  operationId: sendBillToUserRcs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcs/v1/typing_event\n  method: post\n  operationId: typingIndicator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcs/file_server/v2/uploadfile\n  method: post\n  operationId: fileUploadRCS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcs/management/v1/add_tester\n  method: post\n  operationId: ManagementRCS\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcs/management/v1/get_testers\n  method: get\n  operationId: managementRCS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcs/optins/v1/create_optin\n  method: post\n  operationId: optinRCS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcs/v1/mark_read\n  method: post\n  operationId: markingMessagesAsRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcs/v2/revoke_message\n  method: delete\n  operationId: revokeWithSmsFallback\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /callback\n  method: post\n  operationId: post-callback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcs-template-apis/api/v1/template/template\n  method:\
  \ post\n  operationId: createTemplateRCS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcs-template-apis/api/v1/template/template\n  method: put\n  operationId: updateTemplateRCS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcs-template-apis/api/v1/template/template\n  method: get\n  operationId: getTemplateRCS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcs-template-apis/api/v1/template/template\n  method:\
  \ delete\n  operationId: deleteTemplateRCS\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcs-template-apis/api/v1/template//template\n  method: get\n  operationId: getTemplateStatusRCS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rcs-template-apis/api/v1//template//template\n  method: get\n  operationId: getSingleTemplateRCS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilityCheck/getCapabilityDetails\n  method: get\n  operationId: getCapabilityDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilityCheck/checkBulkCapability\n  method: post\n  operationId: checkBulkCapability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rcs/dnd/v1/bulk_dnd_set\n  method: post\n  operationId: bulkDndSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/addSmtp\n  method: post\n  operationId: addSmtpUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/editSmtp\n  method: post\n  operationId: editSmtpUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/resetSmtpPassword\n  method: post\n  operationId: resetSmtpPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /settings/listSmtp\n  method: post\n  operationId: listSmtpUsers\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/addSendingDomain\n  method: post\n  operationId: addSendingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/checkSendingDomain\n  method: post\n  operationId: checkSendingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/verifySendingDomain\n  method: post\n  operationId: verifySendingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/listSendingDomain\n  method: post\n  operationId: listSendingDomains\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/deleteSendingDomain\n  method: post\n  operationId:\
  \ deleteSendingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/addTrackingDomain\n  method: post\n  operationId: addTrackingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/checkTrackingDomain\n  method: post\n  operationId: checkTrackingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/listTrackingDomain\n  method: post\n  operationId: listTrackingDomains\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/deleteTrackingDomain\n  method: post\n  operationId: deleteTrackingDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/addWebhook\n  method: post\n  operationId: addWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/editWebhook\n  method: post\n  operationId: editWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/keyResetWebhook\n  method: post\n  operationId: keyResetWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /settings/listWebhook\n  method: post\n  operationId: listWebhooks\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/deleteWebhook\n  method: post\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings/getWebhookInfo\n  method: post\n  operationId: getWebhookInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/sendMail\n\
  \  method: post\n  operationId: sendMail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/sendTemplate\n  method: post\n  operationId: sendTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/sendTemplateHTTPGet\n  method: get\n  operationId: sendTemplateHTTPGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /messages/getMessageInfo\n  method: post\n  operationId: getMessageInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/userDetails\n  method: post\n  operationId: getUserDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulksms/bulksms\n  method: get\n  operationId: sendSmsSecured\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CreditCheck/checkcredits\n  method: get\n\
  \  operationId: checkCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OtpApi/otpgenerate\n  method: get\n  operationId: generateOtp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OtpApi/checkotp\n  method: get\n  operationId: verifyOtp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulksms/schedulemsg\n  method: get\n  operationId: scheduleSms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulksms/sbulksms\n  method: get\n  operationId: sendPersonalisedSms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulksms/personalizedbulksms\n  method: get\n  operationId: sendUnicodeAcculyncSms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulksms/personalizedcustsms\n  method: get\n  operationId: sendAcculyncSms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulksms/generatetoken\n  method: get\n  operationId: generateToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulksms/bulksubmit\n  method: get\n  operationId: submitSmsWithToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulksms/jsonbulksms\n \
  \ method: post\n  operationId: sendJsonBulkSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulksms/custommsgsubmit\n  method: post\n  operationId: submitMoengageSms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulksms2346/sendjsonsms\n  method: post\n  operationId: submitWebengageSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n  \
  \    purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /routeDetailMail.php\n  method: get\n  operationId: downloadCoverageMap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /callback\n  method: post\n  operationId: viberClientCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/v1/login/\n  method: post\n  operationId: loginApi2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vbs/api/v2/send\n  method: post\n  operationId: singleVideoText\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vbs/api/v2/manage-campaign\n  method: post\n  operationId: campaignVideoText\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vbs/api/v2/upload\n  method: post\n  operationId: campaignFileUpload\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vbs/api/v3/send_bulk\n  method: post\n  operationId: sendBulkMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viber-reports/api/v2/summary-cards\n  method: get\n  operationId: getSummaryCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viber-reports/api/v2/graph\n  method: get\n  operationId: getGraphReport\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viber-reports/api/v2/media-cards\n  method: get\n  operationId: getMediaCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viber-reports/api/v2/camps\n  method: get\n  operationId: getCampaignReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viber-reports/api/v2/tabular\n  method: get\n  operationId: getDailyTabularReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viber-reports/api/v2/viber_templates\n  method: get\n  operationId: listViberTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viber-reports/api/v2/viber_templates\n  method: post\n  operationId: addViberTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /viber-report-creator/v1/fetch_reports\n  method: get\n  operationId: fetchReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /viber-report-creator/v1/create_report\n  method: post\n  operationId: createReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /viber-report-creator/v1/download/{file_name}\n  method: get\n  operationId: downloadReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wba/v2/upload\n  method: post\n  operationId: fileUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wba/v2/manage_campaign\n  method: post\n  operationId: sendBulkCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /wba/catalog/manager/v1/upload\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wba/catalog/manager/v1/create_product_feed\n  method: post\n  operationId: createProductFeed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wba/catalog/manager/v1/update_product_feed\n  method: post\n  operationId: updateProductFeed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wba/catalog/manager/v1/delete_product_feed\n  method: post\n  operationId: deleteProductFeed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wba/catalog/manager/v1/fetch_product_feed\n  method: get\n  operationId: fetchProductFeedDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wba/catalog/manager/v1/fetch_product_details\n  method: get\n  operationId: fetchAllProductFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wba/catalog/manager/v1/fetch_catalog_details\n  method: get\n  operationId: fetchCatalogDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wba/catalog/manager/v1/schedule_product_feed_details\n  method: get\n  operationId: fetchScheduleProductFeedDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wba/catalog/manager/v1/fetch_errors\n  method: get\n  operationId: fetchErrors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whatsapp/report/v1/create_report/myaccounts_panel\n  method: post\n  operationId: createReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /whatsapp/report/v1/create_campaign_specific_report/myaccounts_panel\n  method: post\n  operationId: createCampaignSpecificReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /whatsapp/report/v1/fetch_campaign_specific_report/{report_id}\n  method: get\n  operationId: fetchReportUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whatsapp/report/v1/fetch_campaign_details\n  method: get\n  operationId: viewCampaignSummary\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whatsapp/report/v1/fetch_reports\n  method: get\n  operationId: viewReportSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wbo/v2/optin/store\n  method: post\n  operationId: createOptin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wbo/v2/optinout/store\n  method: post\n  operationId: createOptinOut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wbo/v2/optin/check\n  method: get\n  operationId: checkOptin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /callbacks\n  method: post\n  operationId: whatsappClientCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wba/templates\n  method: get\n  operationId: viewTemplateMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wba/template/create\n  method: post\n  operationId: createTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wba/v1/messages\n  method: post\n  operationId: sendSessionMessageApi\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/v1/login/\n  method: post\n  operationId: loginApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /whatsapp/report/v1/optin-download\n\
  \  method: get\n  operationId: optindownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whatsapp/report/v1/summary/download_optin_report\n  method: get\n  operationId: downloadOptin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wba/templates/media-id\n  method: post\n  operationId: media-idapis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wba/media/v1/get-media-id\n  method: post\n  operationId: media-idapi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wba/management/v1\n\n# --- truncated at 32 KB (33 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/agentic-access/route-mobile-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/agentic-access/route-mobile-agentic-access.yml
summary_line: 108 operations · 69 acting · 3 human-in-the-loop
tags:
- Telecommunications
- India
- CPaaS
- Messaging
- SMS
- A2P Messaging
- WhatsApp Business
- RCS
- Voice
- Email
- Identity Verification
- OTP
- Aggregator
---
