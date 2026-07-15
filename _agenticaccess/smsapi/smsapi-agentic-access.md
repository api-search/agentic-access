---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 10
api_specs:
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI SMS API
  slug: smsapi-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI MMS API
  slug: smsapi-mms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI VMS Voice API
  slug: smsapi-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI Contacts API
  slug: smsapi-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI Sender Names API
  slug: smsapi-sender-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI 2FA Authentication API
  slug: smsapi-2fa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI Subusers API
  slug: smsapi-subusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI Profile and Account API
  slug: smsapi-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI HLR Lookup API
  slug: smsapi-hlr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI Blacklist API
  slug: smsapi-blacklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI Short URLs API
  slug: smsapi-short-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
consequence_counts:
  physical: 7
  read: 10
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Smsapi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /authenticator/send_code
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mms.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sendernames
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /sendernames/{sender}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /sendernames/{sender}/default
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms.do
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vms.do
operation_count: 31
overview: 'SMSAPI exposes 31 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 14 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SMSAPI
provider_slug: smsapi
slug: smsapi-agentic-access
source_filename: smsapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/smsapi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    acting: 21\n    connected: 10\n  by_consequence:\n    physical: 7\n    read: 10\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /sms.do\n  method: post\n  operationId: sendSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mms.do\n  method: post\n  operationId: sendMms\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vms.do\n  method: post\n  operationId: sendVms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contactId}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contactId}\n  method: put\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /contacts/{contactId}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/groups\n  method: get\n  operationId: listContactGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/groups\n  method: post\n  operationId: createContactGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contactId}/groups/{groupId}\n\
  \  method: put\n  operationId: assignContactToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contactId}/groups/{groupId}\n  method: delete\n  operationId: removeContactFromGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sendernames\n  method: get\n  operationId: listSenderNames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sendernames\n  method: post\n  operationId: createSenderName\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sendernames/{sender}\n  method: get\n  operationId: getSenderName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sendernames/{sender}\n  method: delete\n  operationId: deleteSenderName\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sendernames/{sender}/default\n\
  \  method: put\n  operationId: setDefaultSenderName\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authenticator/send_code\n  method: post\n  operationId: sendAuthCode\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authenticator/check_code\n  method: post\n  operationId: checkAuthCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subusers\n  method: get\n  operationId: listSubusers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subusers\n  method: post\n  operationId: createSubuser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subusers/{subuserId}\n  method: get\n  operationId: getSubuser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subusers/{subuserId}\n  method: put\n  operationId: updateSubuser\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subusers/{subuserId}\n  method: delete\n  operationId: deleteSubuser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hlr.do\n  method: post\n  operationId: hlrLookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /blacklist/phone_numbers\n\
  \  method: get\n  operationId: listBlacklist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blacklist/phone_numbers\n  method: post\n  operationId: addBlacklistNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /blacklist/phone_numbers/{phoneNumber}\n  method: delete\n  operationId: removeBlacklistNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /short_urls/links\n  method: get\n  operationId: listShortUrls\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /short_urls/links\n  method: post\n  operationId: createShortUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/agentic-access/smsapi-agentic-access.yml
summary_line: 31 operations · 21 acting
tags:
- Messaging
- SMS
- MMS
- Voice
- 2FA
- Bulk Messaging
- Communications
- CPaaS
---
