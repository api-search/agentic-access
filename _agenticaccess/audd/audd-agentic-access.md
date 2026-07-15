---
acting_count: 3
action_class_counts:
  acting: 3
api_specs:
- filename: audd-openapi.yml
  format: yaml
  label: AudD Music Recognition API
  slug: music-recognition
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-openapi.yml
- filename: audd-openapi.yml
  format: yaml
  label: AudD Recognize with Offset API
  slug: recognize-with-offset
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-openapi.yml
- filename: audd-openapi.yml
  format: yaml
  label: AudD Humming Recognition API
  slug: humming-recognition
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-openapi.yml
- filename: audd-openapi.yml
  format: yaml
  label: AudD Enterprise File Scan API
  slug: enterprise-file-scan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-openapi.yml
- filename: audd-openapi.yml
  format: yaml
  label: AudD Lyrics API
  slug: lyrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/openapi/audd-openapi.yml
consequence_counts:
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Audd Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'AudD exposes 3 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AudD
provider_slug: audd
slug: audd-agentic-access
source_filename: audd-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/audd-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 3\n  by_consequence:\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: recognize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recognizeWithOffset/\n  method: post\n  operationId: recognizeWithOffset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /findLyrics/\n  method: post\n  operationId: findLyrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audd/refs/heads/main/agentic-access/audd-agentic-access.yml
summary_line: 3 operations · 3 acting
tags:
- Music
- Music Recognition
- Audio
- Fingerprinting
- Lyrics
---
