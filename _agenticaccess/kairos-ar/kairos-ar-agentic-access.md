---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 2
api_specs:
- filename: kairos-ar-openapi.yml
  format: yaml
  label: Kairos Face Recognition & Emotion Analysis API
  slug: kairos-face-recognition-emotion-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kairos-ar/refs/heads/main/openapi/kairos-ar-openapi.yml
consequence_counts:
  read: 2
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kairos Ar Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Kairos AR exposes 13 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kairos AR
provider_slug: kairos-ar
slug: kairos-ar-agentic-access
source_filename: kairos-ar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/kairos-ar-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 11\n    connected: 2\n  by_consequence:\n    write: 11\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /enroll\n  method: post\n  operationId: enroll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify\n  method: post\n  operationId: verify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recognize\n  method: post\n  operationId: recognize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /detect\n  method: post\n  operationId: detect\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gallery/list_all\n  method: post\n  operationId: listGalleries\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gallery/view\n  method: post\n  operationId: viewGallery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gallery/view_subject\n  method: post\n  operationId: viewSubject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gallery/remove\n  method: post\n  operationId: removeGallery\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gallery/remove_subject\n  method: post\n  operationId: removeSubject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/media\n  method: post\n  operationId: createMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/media/{id}\n  method: get\n  operationId:\
  \ getMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/media/{id}\n  method: delete\n  operationId: deleteMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/analytics/{id}\n  method: get\n  operationId: getAnalytics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kairos-ar/refs/heads/main/agentic-access/kairos-ar-agentic-access.yml
summary_line: 13 operations · 11 acting
tags:
- Company
- Face Recognition
- Facial Recognition
- Biometrics
- Emotion Analysis
- Computer Vision
- Identity
- Artificial Intelligence
- Machine Learning
- Image Analysis
---
