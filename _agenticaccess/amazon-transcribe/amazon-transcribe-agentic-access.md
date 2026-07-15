---
acting_count: 5
action_class_counts:
  acting: 5
api_specs:
- filename: amazon-transcribe-openapi.yml
  format: yaml
  label: Amazon Transcribe REST API
  slug: amazon-transcribe-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-transcribe/refs/heads/main/openapi/amazon-transcribe-openapi.yml
consequence_counts:
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Transcribe Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Amazon Transcribe exposes 5 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Transcribe
provider_slug: amazon-transcribe
slug: amazon-transcribe-agentic-access
source_filename: amazon-transcribe-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-transcribe-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 5\n  by_consequence:\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /#StartTranscriptionJob\n  method: post\n  operationId: StartTranscriptionJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#GetTranscriptionJob\n  method: post\n  operationId: GetTranscriptionJob\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#ListTranscriptionJobs\n  method: post\n  operationId: ListTranscriptionJobs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DeleteTranscriptionJob\n  method: post\n  operationId: DeleteTranscriptionJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#CreateVocabulary\n  method: post\n\
  \  operationId: CreateVocabulary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-transcribe/refs/heads/main/agentic-access/amazon-transcribe-agentic-access.yml
summary_line: 5 operations · 5 acting
tags:
- Audio Processing
- Machine Learning
- Speech Recognition
- Speech-To-Text
- Transcription
---
