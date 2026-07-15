---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 12
api_specs:
- filename: usercentrics-app-cmp-sdk-openapi.yml
  format: yaml
  label: Usercentrics App CMP SDK
  slug: app-cmp-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-app-cmp-sdk-openapi.yml
- filename: usercentrics-web-cmp-v3-openapi.yml
  format: yaml
  label: Usercentrics Web CMP (V3)
  slug: web-cmp-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-web-cmp-v3-openapi.yml
- filename: usercentrics-cookiebot-cmp-openapi.yml
  format: yaml
  label: Cookiebot CMP
  slug: cookiebot-cmp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/openapi/usercentrics-cookiebot-cmp-openapi.yml
consequence_counts:
  physical: 1
  read: 12
  safety-critical: 1
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Usercentrics Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /consent/withdraw
operation_count: 29
overview: 'Usercentrics exposes 29 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 15 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Usercentrics
provider_slug: usercentrics
slug: usercentrics-agentic-access
source_filename: usercentrics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/usercentrics-app-cmp-sdk-openapi.yml, openapi/usercentrics-cookiebot-cmp-openapi.yml,\n  openapi/usercentrics-web-cmp-v3-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 17\n    connected: 12\n  by_consequence:\n    write: 15\n    read: 12\n    safety-critical: 1\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /configure\n  method: post\n  operationId: configureSdk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /is-ready\n  method: get\n  operationId: isReady\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cmp-data\n  method: get\n  operationId: getCmpData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consents\n  method: get\n  operationId: getConsents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tcf-data\n  method: get\n  operationId: getTcfData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ccpa-data\n  method: get\n  operationId: getCcpaData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /controller-id\n  method: get\n  operationId: getControllerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restore-user-session\n  method: post\n  operationId: restoreUserSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reset\n  method: post\n  operationId: resetUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /dialog/show\n  method: post\n  operationId: cookiebotShow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dialog/hide\n  method: post\n  operationId: cookiebotHide\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dialog/renew\n  method: post\n  operationId: cookiebotRenew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /consent/withdraw\n  method: post\n  operationId: cookiebotWithdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consent/submit-custom\n  method: post\n  operationId: cookiebotSubmitCustomConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consent/state\n  method: get\n  operationId: cookiebotGetConsent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /scripts/get\n  method: get\n  operationId: cookiebotGetScript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scripts/run\n  method: post\n  operationId: cookiebotRunScripts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scanner/last-report\n  method: get\n  operationId: cookiebotLastReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ui/show-first-layer\n  method: post\n  operationId: uiShowFirstLayer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ui/show-second-layer\n  method: post\n  operationId: uiShowSecondLayer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ui/accept-all\n  method: post\n  operationId: uiAcceptAll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ui/deny-all\n  method: post\n  operationId: uiDenyAll\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ui/update-services\n  method: post\n  operationId: uiUpdateServices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ui/services-base-info\n  method: get\n  operationId: uiGetServicesBaseInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tcf/get-tc-data\n  method: post\n  operationId: tcfGetTCData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tcf/add-event-listener\n  method: post\n  operationId: tcfAddEventListener\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gpp/ping\n  method: get\n  operationId: gppPing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gpp/get-gpp-data\n  method: get\n  operationId: gppGetGppData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consent-mode/update\n  method: post\n  operationId:\
  \ consentModeUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usercentrics/refs/heads/main/agentic-access/usercentrics-agentic-access.yml
summary_line: 29 operations · 17 acting · 1 human-in-the-loop
tags:
- Privacy
- Consent
- CMP
- Compliance
- GDPR
- CCPA
- TCF
- GPP
- Cookies
- AI Governance
---
