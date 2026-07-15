---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 7
api_specs:
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel Voice Call API
  slug: exotel-voice-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel Call Details API
  slug: exotel-call-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel SMS API
  slug: exotel-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel Numbers API
  slug: exotel-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel Campaigns API
  slug: exotel-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-asyncapi.yml
  format: yaml
  label: Exotel AgentStream Voice Streaming API
  slug: exotel-agentstream-voice-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/asyncapi/exotel-asyncapi.yml
consequence_counts:
  physical: 1
  read: 7
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Exotel Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/Accounts/{sid}/Sms/send.json
operation_count: 12
overview: 'Exotel exposes 12 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Exotel
provider_slug: exotel
slug: exotel-agentic-access
source_filename: exotel-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/exotel-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 5\n    connected: 7\n  by_consequence:\n    write: 4\n    read: 7\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/Accounts/{sid}/Calls/connect.json\n  method: post\n  operationId: connectCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Accounts/{sid}/Calls/{CallSid}.json\n  method: get\n  operationId: getCallDetails\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Accounts/{sid}/Calls.json\n  method: get\n  operationId: listCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/Accounts/{sid}/Sms/send.json\n  method: post\n  operationId: sendSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/Accounts/{sid}/Sms/Messages/{SmsSid}.json\n  method: get\n  operationId: getSmsDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /v1/Accounts/{sid}/Numbers/{Number}.json\n  method: get\n  operationId: getNumberMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{sid}/campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{sid}/campaigns\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{sid}/campaigns/{campaign_id}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{sid}/campaigns/{campaign_id}\n  method: put\n  operationId: updateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{sid}/campaigns/{campaign_id}\n  method: delete\n  operationId: deleteCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{sid}/campaigns/{campaign_id}/call-details\n  method: get\n  operationId: getCampaignCallDetails\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/agentic-access/exotel-agentic-access.yml
summary_line: 12 operations · 5 acting
tags:
- Cloud Telephony
- Voice
- SMS
- India
- CPaaS
- Call Center
- IVR
- Numbers
- Communications
- Customer Engagement
---
