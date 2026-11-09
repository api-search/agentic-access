---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 17
api_specs:
- filename: aistoryhub-co-account-api-openapi.yml
  format: yaml
  label: AIStoryHub Account API
  slug: aistoryhub-co-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-account-api-openapi.yml
- filename: aistoryhub-co-ai-api-openapi.yml
  format: yaml
  label: AIStoryHub AI API
  slug: aistoryhub-co-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-ai-api-openapi.yml
- filename: aistoryhub-co-chapters-api-openapi.yml
  format: yaml
  label: AIStoryHub Chapters API
  slug: aistoryhub-co-chapters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-chapters-api-openapi.yml
- filename: aistoryhub-co-memory-api-openapi.yml
  format: yaml
  label: AIStoryHub Memory API
  slug: aistoryhub-co-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-memory-api-openapi.yml
- filename: aistoryhub-co-rules-api-openapi.yml
  format: yaml
  label: AIStoryHub Rules API
  slug: aistoryhub-co-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-rules-api-openapi.yml
- filename: aistoryhub-co-skills-api-openapi.yml
  format: yaml
  label: AIStoryHub Skills API
  slug: aistoryhub-co-skills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-skills-api-openapi.yml
- filename: aistoryhub-co-stories-api-openapi.yml
  format: yaml
  label: AIStoryHub Stories API
  slug: aistoryhub-co-stories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-stories-api-openapi.yml
- filename: aistoryhub-co-voice-api-openapi.yml
  format: yaml
  label: AIStoryHub Voice API
  slug: aistoryhub-co-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-voice-api-openapi.yml
- filename: aistoryhub-co-world-api-openapi.yml
  format: yaml
  label: AIStoryHub World API
  slug: aistoryhub-co-world-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aistoryhub-co/openapi/aistoryhub-co-world-api-openapi.yml
consequence_counts:
  read: 17
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aistoryhub Co Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 40
overview: 'AIStoryHub exposes 40 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 23 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AIStoryHub
provider_slug: aistoryhub-co
slug: aistoryhub-co-agentic-access
source_filename: aistoryhub-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/aistoryhub-co-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 17\n    acting: 23\n  by_consequence:\n    read: 17\n    write: 23\n  human_in_the_loop_required: 0\noperations:\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stories\n  method: get\n  operationId: listStories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stories\n  method: post\n  operationId: createStory\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stories/{id}\n  method: get\n  operationId: getStory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stories/{id}\n  method: patch\n  operationId: updateStory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stories/{id}/chapters\n  method: get\n  operationId: listChapters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /stories/{id}/chapters\n  method: post\n  operationId: createChapter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stories/{id}/chapters/{chapterId}\n  method: get\n  operationId: getChapter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stories/{id}/chapters/{chapterId}\n  method: patch\n  operationId: updateChapter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /stories/{id}/chapters/{chapterId}\n  method: delete\n  operationId: deleteChapter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stories/{id}/chapters/{chapterId}/apply-edit\n  method: post\n  operationId: applyEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stories/{id}/manuscript/find-replace\n  method: post\n  operationId: findReplace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stories/{id}/world\n  method: get\n  operationId: listWorld\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stories/{id}/world\n  method: post\n  operationId: createWorld\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stories/{id}/world/{nodeId}\n  method: get\n  operationId: getWorldNode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stories/{id}/world/{nodeId}\n  method: patch\n  operationId: updateWorldNode\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stories/{id}/world/{nodeId}\n  method: delete\n  operationId: deleteWorldNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stories/{id}/voice\n  method: get\n  operationId: getStoryVoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stories/{id}/voice\n  method: patch\n  operationId: setStoryVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/generate\n  method: post\n  operationId: aiGenerate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/revise\n  method: post\n  operationId: aiRevise\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/grit-pass\n  method: post\n  operationId: aiGritPass\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ai/editorial-pass\n  method: post\n  operationId: aiEditorialPass\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai/self-check\n  method: post\n  operationId: aiSelfCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /skills\n  method: get\n  operationId: listSkills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /skills/{slug}\n\
  \  method: get\n  operationId: loadSkill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /skills/{slug}/export\n  method: get\n  operationId: exportSkill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memory\n  method: get\n  operationId: listMemories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memory\n  method: post\n  operationId: saveMemory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /memory/{name}\n  method: delete\n  operationId:\
  \ forgetMemory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rules\n  method: get\n  operationId: listRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rules\n  method: post\n  operationId: createRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rules/{id}\n  method: get\n  operationId: getRule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /rules/{id}\n  method: patch\n  operationId: updateRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rules/{id}\n  method: delete\n  operationId: deleteRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voiceprints\n  method: get\n  operationId: listVoiceprints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voiceprints\n  method: post\n  operationId: createVoiceprint\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voiceprints/{id}\n  method: get\n  operationId: getVoiceprint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voiceprints/{id}\n  method: patch\n  operationId: updateVoiceprint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voiceprints/{id}\n  method: delete\n  operationId: deleteVoiceprint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/aistoryhub-co/agentic-access/aistoryhub-co-agentic-access.yml
summary_line: 40 operations · 23 acting
tags:
- Artificial Intelligence
- Writing
- Fiction
- Platform
- Free
---
