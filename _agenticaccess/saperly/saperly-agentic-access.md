---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 24
api_specs:
- filename: saperly-api-token-registry-api-openapi.yml
  format: yaml
  label: Saperly API Token Registry API
  slug: saperly-api-token-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-api-token-registry-api-openapi.yml
- filename: saperly-assistant-api-openapi.yml
  format: yaml
  label: Saperly Assistant API
  slug: saperly-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-assistant-api-openapi.yml
- filename: saperly-connections-api-openapi.yml
  format: yaml
  label: Saperly Connections API
  slug: saperly-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-connections-api-openapi.yml
- filename: saperly-consent-api-openapi.yml
  format: yaml
  label: Saperly Consent API
  slug: saperly-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-consent-api-openapi.yml
- filename: saperly-customvoices-api-openapi.yml
  format: yaml
  label: Saperly Custom Voices API
  slug: saperly-customvoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-customvoices-api-openapi.yml
- filename: saperly-health-api-openapi.yml
  format: yaml
  label: Saperly Health API
  slug: saperly-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-health-api-openapi.yml
- filename: saperly-keys-api-openapi.yml
  format: yaml
  label: Saperly Keys API
  slug: saperly-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-keys-api-openapi.yml
- filename: saperly-languages-api-openapi.yml
  format: yaml
  label: Saperly Languages API
  slug: saperly-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-languages-api-openapi.yml
- filename: saperly-messaging-api-openapi.yml
  format: yaml
  label: Saperly Messaging API
  slug: saperly-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-messaging-api-openapi.yml
- filename: saperly-numbers-api-openapi.yml
  format: yaml
  label: Saperly Numbers API
  slug: saperly-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-numbers-api-openapi.yml
- filename: saperly-pricing-api-openapi.yml
  format: yaml
  label: Saperly Pricing API
  slug: saperly-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-pricing-api-openapi.yml
- filename: saperly-usage-api-openapi.yml
  format: yaml
  label: Saperly Usage API
  slug: saperly-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-usage-api-openapi.yml
- filename: saperly-voice-api-openapi.yml
  format: yaml
  label: Saperly Voice API
  slug: saperly-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-voice-api-openapi.yml
- filename: saperly-voices-api-openapi.yml
  format: yaml
  label: Saperly Voices API
  slug: saperly-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-voices-api-openapi.yml
- filename: saperly-workspace-api-openapi.yml
  format: yaml
  label: Saperly Workspace API
  slug: saperly-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-workspace-api-openapi.yml
- filename: saperly-workspace-invitations-api-openapi.yml
  format: yaml
  label: Saperly Workspace Invitations API
  slug: saperly-workspace-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/openapi/saperly-workspace-invitations-api-openapi.yml
consequence_counts:
  physical: 6
  read: 24
  safety-critical: 3
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Saperly Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api-tokens/{id}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /consent/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workspaces/{slug}/api-tokens/{tokenId}/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /calls/{id}/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /connections
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /numbers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /numbers/{id}/sms-sender
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /workspaces/{slug}/invitations
operation_count: 48
overview: 'Saperly exposes 48 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 15 write, 6 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Saperly
provider_slug: saperly
slug: saperly-agentic-access
source_filename: saperly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: generated\nsource: openapi/saperly-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 24\n    acting: 24\n  by_consequence:\n    read: 24\n    write: 15\n    safety-critical: 3\n    physical: 6\n  human_in_the_loop_required: 3\noperations:\n- path: /health\n  method: get\n  operationId: health.check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{slug}/members\n  method: get\n  operationId: workspace.members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /workspaces/{slug}/api-tokens\n  method: get\n  operationId: workspace.api-tokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{slug}/api-tokens\n  method: post\n  operationId: api-token-registry.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{slug}/webhooks\n  method: get\n  operationId: workspace.webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{slug}/webhooks\n  method: post\n  operationId: workspace.create-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{slug}/webhooks/{webhookId}/deliveries\n  method: get\n  operationId: workspace.webhook-deliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{slug}/audit-events\n  method: get\n  operationId: workspace.audit-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{slug}/api-tokens/{tokenId}/revoke\n  method: post\n  operationId: api-token-registry.revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /workspaces/{slug}/invitations\n  method: post\n  operationId: workspace-invitations.send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assistant/answer\n  method: post\n  operationId: assistant.answer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /numbers\n  method: get\n  operationId: numbers.list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /numbers\n  method: post\n  operationId: numbers.provision\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /numbers/{id}\n  method: get\n  operationId: numbers.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /numbers/{id}/release\n  method: post\n  operationId: numbers.release\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /numbers/{id}/connection\n  method: post\n  operationId: numbers.assignConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /numbers/{id}/webhook\n  method: post\n  operationId: numbers.setWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /numbers/{id}/sms-sender\n  method: post\n  operationId: numbers.setSmsSenderId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /numbers/{id}/caller-id\n  method: post\n  operationId: numbers.setCallerIdName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections\n  method: get\n  operationId: connections.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections\n  method: post\n  operationId: connections.create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/{id}\n  method: get\n  operationId: connections.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/{id}\n  method: patch\n  operationId: connections.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/{id}\n  method: delete\n  operationId: connections.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: post\n  operationId: messaging.send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: get\n  operationId: messaging.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls\n  method: post\n  operationId: voice.place\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls\n  method: get\n  operationId: voice.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/{id}/end\n  method: post\n  operationId: voice.end\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/{id}/transfer\n  method: post\n  operationId: voice.transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /calls/{id}\n  method: get\n  operationId: voice.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/{id}/recording\n  method: get\n  operationId: voice.recording\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/{id}/transcript\n  method: get\n  operationId: voice.transcript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voices\n  method: get\n  operationId: voices.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-voices\n  method: get\n  operationId: customVoices.list\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-voices\n  method: post\n  operationId: customVoices.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom-voices/{id}\n  method: get\n  operationId: customVoices.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-voices/{id}\n  method: delete\n  operationId: customVoices.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /languages\n  method: get\n  operationId: languages.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: usage.summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consent\n  method: get\n  operationId: consent.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consent\n  method: post\n  operationId: consent.record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /consent/revoke\n  method: post\n  operationId: consent.revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /consent/check\n  method: get\n  operationId: consent.check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing/quote\n  method: get\n  operationId: pricing.quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-tokens\n  method: get\n  operationId: keys.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /api-tokens\n  method: post\n  operationId: keys.mint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-tokens/{id}/revoke\n  method: post\n  operationId: keys.revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saperly/refs/heads/main/agentic-access/saperly-agentic-access.yml
summary_line: 48 operations · 24 acting · 3 human-in-the-loop
tags:
- Telephony
- Voice
- SMS
- Phone Numbers
- AI Agents
- Consent
- Compliance
- MCP
- Messaging
- Communications
---
