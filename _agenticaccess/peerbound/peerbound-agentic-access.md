---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: peerbound-activities-api-openapi.yml
  format: yaml
  label: Peerbound Activities API
  slug: peerbound-activities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-activities-api-openapi.yml
- filename: peerbound-moments-api-openapi.yml
  format: yaml
  label: Peerbound Moments API
  slug: peerbound-moments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-moments-api-openapi.yml
- filename: peerbound-notes-api-openapi.yml
  format: yaml
  label: Peerbound Notes API
  slug: peerbound-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-notes-api-openapi.yml
- filename: peerbound-reviews-api-openapi.yml
  format: yaml
  label: Peerbound Reviews API
  slug: peerbound-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-reviews-api-openapi.yml
- filename: peerbound-stories-api-openapi.yml
  format: yaml
  label: Peerbound Stories API
  slug: peerbound-stories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-stories-api-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Peerbound Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Peerbound exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Peerbound
provider_slug: peerbound
slug: peerbound-agentic-access
source_filename: peerbound-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/peerbound-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /stories\n  method: get\n  operationId: list_stories_stories_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stories/{story_id}\n  method: get\n  operationId: get_story_stories__story_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reviews\n  method: get\n  operationId:\
  \ list_reviews_reviews_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reviews/{review_id}\n  method: get\n  operationId: get_review_reviews__review_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /moments\n  method: get\n  operationId: list_moments_moments_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /moments/{moment_id}\n  method: get\n  operationId: get_moment_moments__moment_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notes\n  method: get\n  operationId: list_notes_notes_get\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notes/{note_id}\n  method: get\n  operationId: get_note_notes__note_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activities\n  method: get\n  operationId: list_activities_activities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activities/{activity_id}\n  method: get\n  operationId: get_activity_activities__activity_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/peerbound/agentic-access/peerbound-agentic-access.yml
summary_line: 10 operations
tags:
- Company
- Software-as-a-Service
- Sales Enablement
- Customer Proof
- Analytics
---
