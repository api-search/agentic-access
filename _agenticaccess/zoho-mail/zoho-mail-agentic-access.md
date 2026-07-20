---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 13
api_specs:
- filename: openapi-specification.html
  format: yaml
  label: Zoho Mail API
  slug: zoho-mail-api
  spec_type: OpenAPI
  url: https://prezohoweb.zoho.com/mail/help/api/openapi-specification.html
consequence_counts:
  physical: 1
  read: 13
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zoho Mail Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/accounts/{accountId}/messages
operation_count: 23
overview: 'Zoho Mail exposes 23 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 9 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zoho Mail
provider_slug: zoho-mail
slug: zoho-mail-agentic-access
source_filename: zoho-mail-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 13\n    acting: 10\n  by_consequence:\n    read: 13\n    write: 9\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoMail.accounts.READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoMail.accounts.READ\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{accountId}\n  method: put\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoMail.accounts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{accountId}/folders\n  method: get\n  operationId: listFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoMail.folders\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{accountId}/folders\n  method: post\n  operationId: createFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoMail.folders\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{accountId}/folders/{folderId}\n  method: get\n  operationId: getFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoMail.folders\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{accountId}/folders/{folderId}\n  method: put\n  operationId: updateFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoMail.folders\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{accountId}/folders/{folderId}\n  method: delete\n  operationId: deleteFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   scope:\n    - ZohoMail.folders\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{accountId}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoMail.messages\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{accountId}/messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - ZohoMail.messages\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{accountId}/messages/search\n \
  \ method: get\n  operationId: searchMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoMail.messages\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{accountId}/messages/attachments\n  method: post\n  operationId: uploadAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoMail.messages\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{accountId}/messages/{messageId}\n  method: post\n  operationId: replyToMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoMail.messages\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{accountId}/messages/view\n  method: get\n  operationId: viewMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoMail.messages\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{accountId}/updatemessage\n  method: put\n  operationId: updateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoMail.messages\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{accountId}/folders/{folderId}/messages/{messageId}\n  method: delete\n  operationId: deleteMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoMail.messages\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{accountId}/folders/{folderId}/messages/{messageId}/header\n  method: get\n  operationId: getMessageHeader\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoMail.messages\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{accountId}/folders/{folderId}/messages/{messageId}/content\n  method: get\n  operationId: getMessageContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoMail.messages\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{accountId}/folders/{folderId}/messages/{messageId}/details\n  method: get\n  operationId: getMessageDetails\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - ZohoMail.messages\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{accountId}/folders/{folderId}/messages/{messageId}/attachmentinfo\n  method: get\n  operationId: getAttachmentInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoMail.messages\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{accountId}/folders/{folderId}/messages/{messageId}/attachments/{attachmentId}\n  method: get\n  operationId: getAttachmentContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - ZohoMail.messages\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{accountId}/messages/{messageId}/originalmessage\n  method: get\n  operationId: getOriginalMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - ZohoMail.messages\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organization/{zoid}/accounts/{accountId}\n  method: put\n  operationId: adminUpdateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoMail.organization.accounts\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-mail/refs/heads/main/agentic-access/zoho-mail-agentic-access.yml
summary_line: 23 operations · 10 acting
tags:
- Email
- Mail
- Collaboration
- Messaging
- Calendar
- Contacts
- Organization Management
- SaaS
---
