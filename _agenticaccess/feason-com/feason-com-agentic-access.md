---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: feason-com-context-api-openapi.yml
  format: yaml
  label: Feason Context API
  slug: feason-com-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feason-com/openapi/feason-com-context-api-openapi.yml
- filename: feason-com-proof-api-openapi.yml
  format: yaml
  label: Feason Proof API
  slug: feason-com-proof-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feason-com/openapi/feason-com-proof-api-openapi.yml
- filename: feason-com-well-known-api-openapi.yml
  format: yaml
  label: Feason .well Known API
  slug: feason-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feason-com/openapi/feason-com-well-known-api-openapi.yml
consequence_counts:
  read: 5
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Feason Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Feason exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Feason
provider_slug: feason-com
slug: feason-com-agentic-access
source_filename: feason-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: generated\nsource: openapi/feason-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 5\n    acting: 7\n  by_consequence:\n    read: 5\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/context/v1/manifest\n  method: get\n  operationId: getCorpusManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/context/v1/contextualize\n  method: post\n  operationId: contextualize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/context/v1/evaluate-claim\n  method: post\n  operationId: evaluateClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/context/v1/claim-proof\n  method: post\n  operationId: buildClaimProof\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/proof/publish\n  method: post\n  operationId: publishSignedClaimProof\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/proof/verify\n  method: post\n  operationId: verifySignedClaimProof\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/proof/records/{proofId}\n  method: get\n  operationId: getPublishedSignedProof\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/proof/transparency\n  method: get\n  operationId: getProofTransparencyCheckpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /.well-known/feason-proof-keys.json\n  method: get\n  operationId: getFeasonProofSigningKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/context/v1/search\n  method: post\n  operationId: searchSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/context/v1/evidence-packet\n  method: post\n  operationId: buildEvidencePacket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/context/v1/verify-citation\n  method: post\n  operationId: verifyCitation\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/feason-com/agentic-access/feason-com-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- Scripture
- Courses
- Christian History
- Fellowship
- Prayer
---
