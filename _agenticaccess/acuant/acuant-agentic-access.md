---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: acuant-assureid-connect-openapi.yml
  format: yaml
  label: Acuant AssureID Connect API
  slug: assureid-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-assureid-connect-openapi.yml
- filename: acuant-frm-openapi.yml
  format: yaml
  label: Acuant FRM Face Recognition API
  slug: frm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-frm-openapi.yml
- filename: acuant-passive-liveness-openapi.yml
  format: yaml
  label: Acuant Passive Liveness API
  slug: passive-liveness
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-passive-liveness-openapi.yml
- filename: acuant-acas-openapi.yml
  format: yaml
  label: Acuant ACAS (Cloud Authentication Service) API
  slug: acas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-acas-openapi.yml
consequence_counts:
  read: 9
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Acuant Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Acuant exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Acuant
provider_slug: acuant
slug: acuant-agentic-access
source_filename: acuant-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/acuant-acas-openapi.yml, openapi/acuant-assureid-connect-openapi.yml, openapi/acuant-frm-openapi.yml,\n  openapi/acuant-passive-liveness-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 8\n    connected: 9\n  by_consequence:\n    write: 8\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/token\n  method: post\n  operationId: getAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/token/validate\n  method: get\n  operationId: validateToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Document/Instance\n  method: post\n  operationId: createDocumentInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Document/{instanceId}\n  method: get\n  operationId: getDocumentResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Document/{instanceId}\n  method: delete\n  operationId: deleteDocumentInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Document/{instanceId}/Image\n  method: post\n  operationId: uploadDocumentImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Document/{instanceId}/Image\n  method: get\n  operationId: getDocumentImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DocumentImageMetrics\n  method: get\n  operationId: getDocumentImageMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /Document/{instanceId}/Data\n  method: post\n  operationId: uploadDocumentData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /DocumentData\n  method: get\n  operationId: getDocumentData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DocumentChipData\n  method: post\n  operationId: uploadDocumentChipData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /DocumentChipData\n  method: get\n  operationId: getDocumentChipData\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DocumentTypes\n  method: get\n  operationId: listDocumentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DocumentLog\n  method: get\n  operationId: getDocumentLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/facematch\n  method: post\n  operationId: compareFaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/liveness\n  method: post\n  operationId: checkLiveness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/agentic-access/acuant-agentic-access.yml
summary_line: 17 operations · 8 acting
tags:
- Identity Verification
- Document Authentication
- Biometrics
- Face Matching
- Liveness Detection
- KYC
- AML
- ID Capture
---
