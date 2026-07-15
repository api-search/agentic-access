---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 7
api_specs:
- filename: rekor-openapi.yaml
  format: yaml
  label: Rekor Transparency Log API
  slug: rekor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigstore/refs/heads/main/openapi/rekor-openapi.yaml
- filename: fulcio-openapi.json
  format: json
  label: Fulcio Certificate Authority API
  slug: fulcio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigstore/refs/heads/main/openapi/fulcio-openapi.json
consequence_counts:
  read: 7
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sigstore Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Sigstore exposes 11 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sigstore
provider_slug: sigstore
slug: sigstore-agentic-access
source_filename: sigstore-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fulcio-openapi.json, openapi/rekor-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 7\n    acting: 4\n  by_consequence:\n    read: 7\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/configuration\n  method: get\n  operationId: CA_GetConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/signingCert\n  method: post\n  operationId: CA_CreateSigningCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/trustBundle\n  method: get\n  operationId: CA_GetTrustBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/index/retrieve\n  method: post\n  operationId: searchIndex\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/log\n  method: get\n  operationId: getLogInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/log/publicKey\n  method: get\n  operationId: getPublicKey\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/log/proof\n  method: get\n  operationId: getLogProof\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/log/entries\n  method: post\n  operationId: createLogEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/log/entries\n  method: get\n  operationId: getLogEntryByIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/log/entries/{entryUUID}\n  method: get\n  operationId:\
  \ getLogEntryByUUID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/log/entries/retrieve\n  method: post\n  operationId: searchLogQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sigstore/refs/heads/main/agentic-access/sigstore-agentic-access.yml
summary_line: 11 operations · 4 acting
tags:
- Certificate Authority
- Code Signing
- Containers
- Cryptography
- Open Source
- PKI
- Security
- Software Supply Chain
- Transparency Log
---
