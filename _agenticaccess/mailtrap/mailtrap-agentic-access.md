---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 11
api_specs:
- filename: mailtrap-email-api-openapi.yml
  format: yaml
  label: Mailtrap Email Sending API
  slug: mailtrap-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailtrap/refs/heads/main/openapi/mailtrap-email-api-openapi.yml
- filename: mailtrap-email-sandbox-openapi.yml
  format: yaml
  label: Mailtrap Email Sandbox API
  slug: mailtrap-email-sandbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailtrap/refs/heads/main/openapi/mailtrap-email-sandbox-openapi.yml
consequence_counts:
  physical: 3
  read: 11
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Mailtrap Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/accounts/{account_id}/inboxes/{inbox_id}/reset_credentials
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/send/{inbox_id}
operation_count: 23
overview: 'Mailtrap exposes 23 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 8 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mailtrap
provider_slug: mailtrap
slug: mailtrap-agentic-access
source_filename: mailtrap-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mailtrap-email-api-openapi.yml, openapi/mailtrap-email-sandbox-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 12\n    connected: 11\n  by_consequence:\n    physical: 3\n    read: 11\n    write: 8\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/send\n  method: post\n  operationId: sendEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /api/batch\n  method: post\n  operationId: sendBatchEmails\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/send/{inbox_id}\n  method: post\n  operationId: sendToSandboxInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/inboxes\n  method: get\n  operationId: listInboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/projects/{project_id}/inboxes\n  method: post\n  operationId: createInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}\n  method: get\n  operationId: getInbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}\n  method: delete\n  operationId: deleteInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}\n  method: patch\n  operationId: updateInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/clean\n  method: patch\n  operationId: cleanInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/all_read\n  method: patch\n  operationId: markAllRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/reset_credentials\n  method: patch\n  operationId: resetCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/messages/{message_id}\n  method: get\n  operationId:\
  \ getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/messages/{message_id}\n  method: patch\n  operationId: updateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/messages/{message_id}\n  method: delete\n  operationId: deleteMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/messages/{message_id}/forward\n\
  \  method: post\n  operationId: forwardMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/messages/{message_id}/spam_report\n  method: get\n  operationId: getSpamReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/messages/{message_id}/analyze\n  method: get\n  operationId: getHtmlAnalyze\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/messages/{message_id}/body.txt\n  method: get\n  operationId: getMessageBodyText\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/messages/{message_id}/body.html\n  method: get\n  operationId: getMessageBodyHtml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/messages/{message_id}/body.raw\n  method: get\n  operationId: getMessageBodyRaw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/messages/{message_id}/body.eml\n  method: get\n  operationId: getMessageEml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/accounts/{account_id}/inboxes/{inbox_id}/messages/{message_id}/mail_headers\n\
  \  method: get\n  operationId: getMessageHeaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailtrap/refs/heads/main/agentic-access/mailtrap-agentic-access.yml
summary_line: 23 operations · 12 acting · 1 human-in-the-loop
tags:
- Email
- Email Delivery
- Email Sandbox
- Email Testing
- Transactional Email
---
