---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 18
api_specs:
- filename: whippy-campaigns-api-openapi.yml
  format: yaml
  label: Whippy Campaigns API
  slug: whippy-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-campaigns-api-openapi.yml
- filename: whippy-channels-api-openapi.yml
  format: yaml
  label: Whippy Channels API
  slug: whippy-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-channels-api-openapi.yml
- filename: whippy-contacts-api-openapi.yml
  format: yaml
  label: Whippy Contacts API
  slug: whippy-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-contacts-api-openapi.yml
- filename: whippy-conversations-api-openapi.yml
  format: yaml
  label: Whippy Conversations API
  slug: whippy-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-conversations-api-openapi.yml
- filename: whippy-messaging-api-openapi.yml
  format: yaml
  label: Whippy Messaging API
  slug: whippy-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-messaging-api-openapi.yml
- filename: whippy-sequences-api-openapi.yml
  format: yaml
  label: Whippy Sequences API
  slug: whippy-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-sequences-api-openapi.yml
- filename: whippy-webhooks-api-openapi.yml
  format: yaml
  label: Whippy Webhooks API
  slug: whippy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-webhooks-api-openapi.yml
consequence_counts:
  physical: 5
  read: 18
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Whippy Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messaging/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messaging/fax
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messaging/sms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messaging/sms/campaign
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messaging/sms/campaign
operation_count: 34
overview: 'Whippy exposes 34 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 11 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Whippy
provider_slug: whippy
slug: whippy-agentic-access
source_filename: whippy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/whippy-campaigns-api-openapi.yml, openapi/whippy-channels-api-openapi.yml, openapi/whippy-contacts-api-openapi.yml,\n  openapi/whippy-conversations-api-openapi.yml, openapi/whippy-messaging-api-openapi.yml, openapi/whippy-sequences-api-openapi.yml,\n  openapi/whippy-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    acting: 16\n    connected: 18\n  by_consequence:\n    physical: 5\n    read: 18\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /messaging/sms/campaign\n  method: post\n  operationId: sendCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns\n  method: get\n  operationId: getCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}/contacts\n  method: get\n  operationId: getCampaignContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels\n  method: get\n  operationId: getChannels\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{id}\n  method: get\n  operationId: getChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{id}/users\n  method: get\n  operationId: getChannelUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: get\n  operationId: getContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{id}\n  method: put\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/search\n  method:\
  \ post\n  operationId: searchContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/upsert\n  method: put\n  operationId: upsertContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}/communication_preferences\n  method: get\n  operationId: getContactCommunicationPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{id}/communication_preferences/opt_in\n  method: post\n  operationId: optInCommunicationPreference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}/communication_preferences/opt_out\n  method: post\n  operationId: optOutCommunicationPreference\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations\n  method: get\n  operationId: getConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{id}\n  method: get\n  operationId: getConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /conversations/{id}\n  method: put\n  operationId: updateConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/search\n  method: post\n  operationId: searchConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{id}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/sms\n  method: post\n  operationId: sendSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/email\n  method: post\n  operationId: sendEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/fax\n  method: post\n  operationId: sendFax\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /messaging/sms/campaign\n  method: post\n  operationId: sendCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences\n  method: get\n  operationId: getSequences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/{id}\n  method: get\n  operationId: getSequence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/{id}/contacts\n  method: get\n  operationId: getSequenceContacts\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sequences/{id}/contacts\n  method: post\n  operationId: createSequenceContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/{id}/contacts\n  method: delete\n  operationId: removeSequenceContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/runs\n  method: get\n  operationId: getSequenceRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /custom_events\n  method: post\n  operationId: createCustomEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom_events/bulk\n  method: post\n  operationId: createBulkCustomEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/agentic-access/whippy-agentic-access.yml
summary_line: 34 operations · 16 acting
tags:
- Communications
- Messaging
- SMS
- Email
- Voice
- Artificial Intelligence
- Campaigns
- Sequences
---
