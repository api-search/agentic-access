---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 4
api_specs:
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Video Generation API
  slug: video-generation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Avatars / Presenters API
  slug: avatars-presenters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Voices API
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Templates API
  slug: templates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
- filename: colossyan-openapi.yml
  format: yaml
  label: Colossyan Job Status / Webhooks API
  slug: job-status-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/openapi/colossyan-openapi.yml
consequence_counts:
  read: 4
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Colossyan Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Colossyan exposes 10 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Colossyan
provider_slug: colossyan
slug: colossyan-agentic-access
source_filename: colossyan-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/colossyan-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 6\n    connected: 4\n  by_consequence:\n    write: 6\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /video-generation-jobs\n  method: post\n  operationId: createVideoGenerationJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video-generation-jobs/{videoGenerationJobId}\n  method: get\n  operationId: getVideoGenerationJob\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /video-generation-jobs/{videoGenerationJobId}\n  method: delete\n  operationId: cancelVideoGenerationJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video-generation-jobs/template-jobs\n  method: post\n  operationId: createTemplateVideoGenerationJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generated-videos/{videoId}\n  method: get\n  operationId: getGeneratedVideo\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generated-videos/{videoId}\n  method: delete\n  operationId: deleteGeneratedVideo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/actors\n  method: get\n  operationId: listAvatars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/actors\n  method: post\n  operationId: createAvatar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/voices\n  method: get\n  operationId: listVoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /knowledge-to-draft/generate-draft\n  method: post\n  operationId: generateDraftFromKnowledge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colossyan/refs/heads/main/agentic-access/colossyan-agentic-access.yml
summary_line: 10 operations · 6 acting
tags:
- AI
- Video Generation
- Avatars
- Text to Video
- Learning and Development
---
