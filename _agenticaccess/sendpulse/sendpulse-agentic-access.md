---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 14
api_specs:
- filename: sendpulse-openapi.yml
  format: yaml
  label: SendPulse Address Books & Email API
  slug: sendpulse-address-books-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-openapi.yml
- filename: sendpulse-openapi.yml
  format: yaml
  label: SendPulse SMTP / Transactional Email API
  slug: sendpulse-smtp-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-openapi.yml
- filename: sendpulse-openapi.yml
  format: yaml
  label: SendPulse SMS API
  slug: sendpulse-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-openapi.yml
- filename: sendpulse-openapi.yml
  format: yaml
  label: SendPulse Web Push API
  slug: sendpulse-web-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-openapi.yml
- filename: sendpulse-openapi.yml
  format: yaml
  label: SendPulse Chatbots API
  slug: sendpulse-chatbots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-openapi.yml
- filename: sendpulse-openapi.yml
  format: yaml
  label: SendPulse Automation 360 API
  slug: sendpulse-automation-360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-openapi.yml
consequence_counts:
  physical: 4
  read: 14
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sendpulse Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /campaigns
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /senders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /smtp/emails
operation_count: 31
overview: 'SendPulse exposes 31 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 13 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SendPulse
provider_slug: sendpulse
slug: sendpulse-agentic-access
source_filename: sendpulse-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sendpulse-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    acting: 17\n    connected: 14\n  by_consequence:\n    write: 13\n    read: 14\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/access_token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addressbooks\n  method: get\n  operationId: listAddressBooks\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addressbooks\n  method: post\n  operationId: createAddressBook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addressbooks/{id}\n  method: get\n  operationId: getAddressBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addressbooks/{id}\n  method: put\n  operationId: editAddressBook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /addressbooks/{id}\n  method: delete\n  operationId: deleteAddressBook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addressbooks/{id}/emails\n  method: get\n  operationId: listEmailsFromBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addressbooks/{id}/emails\n  method: post\n  operationId: addEmailsToBook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addressbooks/{id}/emails\n\
  \  method: delete\n  operationId: removeEmailsFromBook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}\n  method: get\n  operationId: getCampaign\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}\n  method: delete\n  operationId: cancelCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /senders\n  method: get\n  operationId: listSenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /senders\n  method: post\n  operationId: addSender\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /blacklist\n  method: get\n  operationId: listBlacklist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blacklist\n  method: post\n  operationId: addToBlacklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /blacklist\n  method: delete\n  operationId: removeFromBlacklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /smtp/emails\n  method: get\n  operationId: listSmtpEmails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /smtp/emails\n  method: post\n  operationId: sendSmtpEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /smtp/emails/{id}\n  method: get\n  operationId: getSmtpEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /smtp/unsubscribe\n  method: get\n  operationId: listSmtpUnsubscribed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /smtp/unsubscribe\n  method: post\n  operationId: addSmtpUnsubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/send\n  method: post\n  operationId: sendSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/campaigns\n  method: post\n  operationId: createSmsCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/campaigns/list\n  method: get\n  operationId: listSmsCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push/tasks\n  method: get\n  operationId: listPushCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push/tasks\n  method: post\n  operationId: createPushCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /push/websites\n  method: get\n  operationId: listPushWebsites\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/name/{eventName}\n  method: post\n  operationId: startEventAutomation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/agentic-access/sendpulse-agentic-access.yml
summary_line: 31 operations · 17 acting
tags:
- Marketing
- Email
- SMS
- Web Push
- Chatbots
- Transactional Email
- Multichannel
---
