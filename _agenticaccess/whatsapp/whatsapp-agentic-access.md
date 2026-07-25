---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 16
api_specs:
- filename: whatsapp-flows-api-openapi.yml
  format: yaml
  label: WhatsApp Flows API
  slug: flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-flows-api-openapi.yml
- filename: whatsapp-on-premises-api-deprecated
  format: yaml
  label: WhatsApp On-Premises API
  slug: on-premises-api
  spec_type: Postman
  url: https://www.postman.com/meta/whatsapp-business-platform/collection/vdi189b/whatsapp-on-premises-api-deprecated
- filename: whatsapp-analytics-api-openapi.yml
  format: yaml
  label: WhatsApp Analytics API
  slug: whatsapp-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-analytics-api-openapi.yml
- filename: whatsapp-assets-api-openapi.yml
  format: yaml
  label: WhatsApp Assets API
  slug: whatsapp-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-assets-api-openapi.yml
- filename: whatsapp-assigned-users-api-openapi.yml
  format: yaml
  label: WhatsApp Assigned Users API
  slug: whatsapp-assigned-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-assigned-users-api-openapi.yml
- filename: whatsapp-business-accounts-api-openapi.yml
  format: yaml
  label: WhatsApp Business Accounts API
  slug: whatsapp-business-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-business-accounts-api-openapi.yml
- filename: whatsapp-business-profile-api-openapi.yml
  format: yaml
  label: WhatsApp Business Profile API
  slug: whatsapp-business-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-business-profile-api-openapi.yml
- filename: whatsapp-lifecycle-api-openapi.yml
  format: yaml
  label: WhatsApp Lifecycle API
  slug: whatsapp-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-lifecycle-api-openapi.yml
- filename: whatsapp-media-api-openapi.yml
  format: yaml
  label: WhatsApp Media API
  slug: whatsapp-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-media-api-openapi.yml
- filename: whatsapp-message-templates-api-openapi.yml
  format: yaml
  label: WhatsApp Message Templates API
  slug: whatsapp-message-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-message-templates-api-openapi.yml
- filename: whatsapp-messages-api-openapi.yml
  format: yaml
  label: WhatsApp Messages API
  slug: whatsapp-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-messages-api-openapi.yml
- filename: whatsapp-phone-numbers-api-openapi.yml
  format: yaml
  label: WhatsApp Phone Numbers API
  slug: whatsapp-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-phone-numbers-api-openapi.yml
- filename: whatsapp-product-catalogs-api-openapi.yml
  format: yaml
  label: WhatsApp Product Catalogs API
  slug: whatsapp-product-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-product-catalogs-api-openapi.yml
- filename: whatsapp-qr-codes-api-openapi.yml
  format: yaml
  label: WhatsApp QR Codes API
  slug: whatsapp-qr-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-qr-codes-api-openapi.yml
- filename: whatsapp-registration-api-openapi.yml
  format: yaml
  label: WhatsApp Registration API
  slug: whatsapp-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-registration-api-openapi.yml
- filename: whatsapp-subscribed-apps-api-openapi.yml
  format: yaml
  label: WhatsApp Subscribed Apps API
  slug: whatsapp-subscribed-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-subscribed-apps-api-openapi.yml
- filename: whatsapp-two-step-verification-api-openapi.yml
  format: yaml
  label: WhatsApp Two-Step Verification API
  slug: whatsapp-two-step-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/openapi/whatsapp-two-step-verification-api-openapi.yml
consequence_counts:
  physical: 1
  read: 16
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Whatsapp Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{phone-number-id}/messages
operation_count: 43
overview: 'WhatsApp exposes 43 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 26 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WhatsApp
provider_slug: whatsapp
slug: whatsapp-agentic-access
source_filename: whatsapp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/whatsapp-business-management-api-openapi.yml, openapi/whatsapp-cloud-api-openapi.yml,\n  openapi/whatsapp-flows-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 16\n    acting: 27\n  by_consequence:\n    read: 16\n    write: 26\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /{waba-id}\n  method: get\n  operationId: getWhatsAppBusinessAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{waba-id}/phone_numbers\n  method: get\n  operationId: listPhoneNumbers\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{waba-id}/message_templates\n  method: get\n  operationId: listMessageTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{waba-id}/message_templates\n  method: post\n  operationId: createMessageTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{waba-id}/message_templates\n  method: delete\n  operationId: deleteMessageTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{message-template-id}\n  method: post\n  operationId: updateMessageTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{waba-id}/conversation_analytics\n  method: get\n  operationId: getConversationAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{waba-id}/template_analytics\n  method: get\n  operationId: getTemplateAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{waba-id}/subscribed_apps\n  method: get\n  operationId: listSubscribedApps\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{waba-id}/subscribed_apps\n  method: post\n  operationId: subscribeApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{waba-id}/subscribed_apps\n  method: delete\n  operationId: unsubscribeApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{waba-id}/assigned_users\n  method: get\n  operationId: listAssignedUsers\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{waba-id}/assigned_users\n  method: post\n  operationId: assignUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{waba-id}/assigned_users\n  method: delete\n  operationId: removeAssignedUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{waba-id}/product_catalogs\n  method: get\n  operationId: listProductCatalogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /{waba-id}/product_catalogs\n  method: post\n  operationId: connectProductCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{waba-id}/product_catalogs\n  method: delete\n  operationId: disconnectProductCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{phone-number-id}/messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{phone-number-id}/media\n  method: post\n  operationId: uploadMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{media-id}\n  method: get\n  operationId: getMediaUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{media-id}\n  method: delete\n  operationId: deleteMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{phone-number-id}\n  method: get\n  operationId: getPhoneNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{phone-number-id}\n  method: post\n  operationId: setTwoStepVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{phone-number-id}/whatsapp_business_profile\n  method: get\n  operationId: getBusinessProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{phone-number-id}/whatsapp_business_profile\n\
  \  method: post\n  operationId: updateBusinessProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{phone-number-id}/request_code\n  method: post\n  operationId: requestVerificationCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{phone-number-id}/verify_code\n  method: post\n  operationId: verifyCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /{phone-number-id}/register\n  method: post\n  operationId: registerPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{phone-number-id}/deregister\n  method: post\n  operationId: deregisterPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{phone-number-id}/message_qrdls\n  method: post\n  operationId: createQrCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{phone-number-id}/message_qrdls\n  method: get\n  operationId: listQrCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{phone-number-id}/message_qrdls/{qr-code-id}\n  method: get\n  operationId: getQrCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{phone-number-id}/message_qrdls/{qr-code-id}\n  method: post\n  operationId: updateQrCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /{phone-number-id}/message_qrdls/{qr-code-id}\n  method: delete\n  operationId: deleteQrCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{waba-id}/flows\n  method: get\n  operationId: listFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{waba-id}/flows\n  method: post\n  operationId: createFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{flow-id}\n  method: get\n  operationId:\
  \ getFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{flow-id}\n  method: post\n  operationId: updateFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{flow-id}\n  method: delete\n  operationId: deleteFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{flow-id}/assets\n  method: get\n  operationId: getFlowAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /{flow-id}/assets\n  method: post\n  operationId: uploadFlowJson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{flow-id}/publish\n  method: post\n  operationId: publishFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{flow-id}/deprecate\n  method: post\n  operationId: deprecateFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/agentic-access/whatsapp-agentic-access.yml
summary_line: 43 operations · 27 acting
tags: []
---
