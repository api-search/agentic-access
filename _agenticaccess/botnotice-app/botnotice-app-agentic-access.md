---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 4
api_specs:
- filename: botnotice-app-consent-api-openapi.yml
  format: yaml
  label: BotNotice Consent API
  slug: botnotice-app-consent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-consent-api-openapi.yml
- filename: botnotice-app-content-register-api-openapi.yml
  format: yaml
  label: BotNotice Content register API
  slug: botnotice-app-content-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-content-register-api-openapi.yml
- filename: botnotice-app-free-tools-api-openapi.yml
  format: yaml
  label: BotNotice Free tools API
  slug: botnotice-app-free-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-free-tools-api-openapi.yml
- filename: botnotice-app-law-dataset-api-openapi.yml
  format: yaml
  label: BotNotice Law dataset API
  slug: botnotice-app-law-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-law-dataset-api-openapi.yml
- filename: botnotice-app-voice-api-openapi.yml
  format: yaml
  label: BotNotice Voice API
  slug: botnotice-app-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botnotice-app/openapi/botnotice-app-voice-api-openapi.yml
consequence_counts:
  read: 4
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Botnotice App Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/consent/revoke
operation_count: 10
overview: 'BotNotice exposes 10 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 5 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BotNotice
provider_slug: botnotice-app
slug: botnotice-app-agentic-access
source_filename: botnotice-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/botnotice-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 6\n    connected: 4\n  by_consequence:\n    write: 5\n    read: 4\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/scan\n  method: post\n  operationId: scanWebsite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/ai-disclosure-laws.json\n  method: get\n  operationId: lawDataset\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/ai-disclosure-laws.csv\n  method: get\n  operationId: lawDatasetCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/ai-disclosure-laws/{slug}.json\n  method: get\n  operationId: lawBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/consent\n  method: post\n  operationId: recordConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/consent/check\n  method: post\n  operationId:\
  \ checkConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/consent/revoke\n  method: post\n  operationId: revokeConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/voice/policy\n  method: get\n  operationId: voicePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/voice/event\n  method: post\n  operationId: voiceEvent\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ingest/content\n  method: post\n  operationId: ingestContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/botnotice-app/agentic-access/botnotice-app-agentic-access.yml
summary_line: 10 operations · 6 acting · 1 human-in-the-loop
tags:
- AI disclosure
- chatbot compliance
- Recordkeeping
- website widget
- managed compliance
- subscription pricing
---
