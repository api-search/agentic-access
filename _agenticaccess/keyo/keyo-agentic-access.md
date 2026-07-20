---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 2
api_specs:
- filename: keyo-openapi.yml
  format: yaml
  label: Keyo REST API
  slug: keyo-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keyo/refs/heads/main/openapi/keyo-openapi.yml
consequence_counts:
  read: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Keyo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Keyo exposes 7 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Keyo
provider_slug: keyo
slug: keyo-agentic-access
source_filename: keyo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/keyo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 5\n    connected: 2\n  by_consequence:\n    write: 5\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token/\n  method: post\n  operationId: OAuthClientCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identities/\n  method: get\n  operationId: IdentitiesGet\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identities/\n  method: post\n  operationId: IdentitiesPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identities/{id}/\n  method: get\n  operationId: IdentityGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identities/{id}/\n  method: patch\n  operationId: IdentitiesPatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /identities/{id}/\n  method: delete\n  operationId: IdentitiesDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identities/{id}/start-enroll/\n  method: post\n  operationId: IdentitiesStartEnroll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keyo/refs/heads/main/agentic-access/keyo-agentic-access.yml
summary_line: 7 operations · 5 acting
tags:
- Company
- Biometrics
- Identity
- Authentication
- Palm Recognition
- Access Control
- Payments
- Identity Verification
---
