---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 10
api_specs:
- filename: mailbridgeapi-activity-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Activity API
  slug: mailbridgeapi-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailbridgeapi/refs/heads/main/openapi/mailbridgeapi-activity-api-openapi.yml
- filename: mailbridgeapi-compliance-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Compliance API
  slug: mailbridgeapi-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailbridgeapi/refs/heads/main/openapi/mailbridgeapi-compliance-api-openapi.yml
- filename: mailbridgeapi-mailbox-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Mailbox API
  slug: mailbridgeapi-mailbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailbridgeapi/refs/heads/main/openapi/mailbridgeapi-mailbox-api-openapi.yml
- filename: mailbridgeapi-receiving-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Receiving API
  slug: mailbridgeapi-receiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailbridgeapi/refs/heads/main/openapi/mailbridgeapi-receiving-api-openapi.yml
- filename: mailbridgeapi-sending-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Sending API
  slug: mailbridgeapi-sending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailbridgeapi/refs/heads/main/openapi/mailbridgeapi-sending-api-openapi.yml
- filename: mailbridgeapi-service-api-openapi.yml
  format: yaml
  label: MailBridgeAPI Service API
  slug: mailbridgeapi-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailbridgeapi/refs/heads/main/openapi/mailbridgeapi-service-api-openapi.yml
consequence_counts:
  physical: 2
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mailbridgeapi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /email/validate/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sendemail/
operation_count: 12
overview: 'MailBridgeAPI exposes 12 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MailBridgeAPI
provider_slug: mailbridgeapi
slug: mailbridgeapi-agentic-access
source_filename: mailbridgeapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: generated\nsource: openapi/mailbridgeapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 10\n    acting: 2\n  by_consequence:\n    read: 10\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /health/\n  method: get\n  operationId: getServiceHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sendemail/\n  method: post\n  operationId: sendEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getemail/\n  method: get\n  operationId: getLiveMailboxMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/unsubscribed/\n  method: get\n  operationId: listUnsubscribeRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/status/\n  method: get\n  operationId: getMailboxStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailbox/insights/\n  method: get\n  operationId: getMailboxInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /email/sent/\n  method: get\n  operationId: listSentEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/received/\n  method: get\n  operationId: listReceivedEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/message/\n  method: get\n  operationId: getEmailMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/search/\n  method: get\n  operationId: searchEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/activity/\n  method: get\n  operationId: getEmailActivity\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/validate/\n  method: post\n  operationId: validateEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailbridgeapi/refs/heads/main/agentic-access/mailbridgeapi-agentic-access.yml
summary_line: 12 operations · 2 acting
tags:
- Email API
- SMTP
- IMAP
- mailbox integration
- Developer Tools
- mailbox monitoring
---
