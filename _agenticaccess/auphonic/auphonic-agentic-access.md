---
acting_count: 45
action_class_counts:
  acting: 45
  connected: 15
api_specs:
- filename: auphonic-info-api-openapi.yml
  format: yaml
  label: Auphonic Info API
  slug: auphonic-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-info-api-openapi.yml
- filename: auphonic-presets-api-openapi.yml
  format: yaml
  label: Auphonic Presets API
  slug: auphonic-presets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-presets-api-openapi.yml
- filename: auphonic-productions-api-openapi.yml
  format: yaml
  label: Auphonic Productions API
  slug: auphonic-productions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-productions-api-openapi.yml
- filename: auphonic-services-api-openapi.yml
  format: yaml
  label: Auphonic Services API
  slug: auphonic-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-services-api-openapi.yml
- filename: auphonic-simple-api-api-openapi.yml
  format: yaml
  label: Auphonic Simple API
  slug: auphonic-simple-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-simple-api-api-openapi.yml
- filename: auphonic-user-api-openapi.yml
  format: yaml
  label: Auphonic User API
  slug: auphonic-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-user-api-openapi.yml
consequence_counts:
  read: 15
  safety-critical: 17
  write: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 17
kind: agentic-access
layout: agentic-access
method: generated
name: Auphonic Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/preset/{uuid}.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/preset/{uuid}.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/preset/{uuid}/algorithms.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/preset/{uuid}/metadata.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/preset/{uuid}/multi_input_files.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/preset/{uuid}/multi_input_files.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/preset/{uuid}/multi_input_files/{track_id}.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/preset/{uuid}/multi_input_files/{track_id}.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/preset/{uuid}/outgoing_services.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/preset/{uuid}/outgoing_services.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/preset/{uuid}/output_files.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/preset/{uuid}/output_files.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/preset/{uuid}/upload.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/preset/{uuid}/webhook.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/preset/{uuid}/webhook.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/presets.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/production/{uuid}/stop.json
operation_count: 60
overview: 'Auphonic exposes 60 API operations that an AI agent could call, of which 45 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 28 write, and 17 safety-critical.


  17 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Auphonic
provider_slug: auphonic
slug: auphonic-agentic-access
source_filename: auphonic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/auphonic-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 60\n  by_action_class:\n    acting: 45\n    connected: 15\n  by_consequence:\n    write: 28\n    read: 15\n    safety-critical: 17\n  human_in_the_loop_required: 17\noperations:\n- path: /api/simple/productions.json\n  method: post\n  operationId: createSimpleProduction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/productions.json\n  method: get\n  operationId: listProductions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/productions.json\n  method: post\n  operationId: createProduction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}.json\n  method: get\n  operationId: getProduction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/production/{uuid}.json\n  method: post\n  operationId: updateProduction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}.json\n  method: delete\n  operationId: deleteProduction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/upload.json\n  method: post\n  operationId: uploadProductionFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/start.json\n  method: post\n  operationId: startProduction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/stop.json\n  method: post\n  operationId: stopProduction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/production/{uuid}/publish.json\n  method: post\n  operationId: publishProduction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/status.json\n\
  \  method: get\n  operationId: getProductionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/production/{uuid}/output_files.json\n  method: post\n  operationId: setProductionOutputFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/output_files.json\n  method: delete\n  operationId: deleteProductionOutputFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/chapters.json\n\
  \  method: post\n  operationId: setProductionChapters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/chapters.json\n  method: delete\n  operationId: deleteProductionChapters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/algorithms.json\n  method: post\n  operationId: setProductionAlgorithms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/metadata.json\n  method: post\n  operationId: setProductionMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/outgoing_services.json\n  method: get\n  operationId: getProductionOutgoingServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/production/{uuid}/outgoing_services.json\n  method: post\n  operationId: setProductionOutgoingServices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/outgoing_services.json\n  method: delete\n  operationId: deleteProductionOutgoingServices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/speech_recognition.json\n  method: post\n  operationId: setProductionSpeechRecognition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/speech_recognition.json\n  method: delete\n  operationId: deleteProductionSpeechRecognition\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/multi_input_files.json\n  method: post\n  operationId: setProductionMultiInputFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/multi_input_files.json\n  method: delete\n  operationId: deleteProductionMultiInputFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/multi_input_files/{track_id}.json\n  method: post\n  operationId: updateProductionMultiInputFileTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/multi_input_files/{track_id}.json\n  method: delete\n  operationId: deleteProductionMultiInputFileTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/cuts.json\n  method: post\n  operationId: setProductionCuts\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/cuts.json\n  method: delete\n  operationId: deleteProductionCuts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/segments.json\n  method: post\n  operationId: setProductionSegments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/production/{uuid}/segments.json\n  method: delete\n  operationId: deleteProductionSegments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/production/{uuid}/webhook.json\n  method: get\n  operationId: getProductionWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/production/{uuid}/webhook.json\n  method: post\n  operationId: setProductionWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/production/{uuid}/webhook.json\n  method: delete\n  operationId: deleteProductionWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/presets.json\n  method: get\n  operationId: listPresets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/presets.json\n  method: post\n  operationId: createPreset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}.json\n\
  \  method: get\n  operationId: getPreset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/preset/{uuid}.json\n  method: post\n  operationId: updatePreset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}.json\n  method: delete\n  operationId: deletePreset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}/upload.json\n\
  \  method: post\n  operationId: uploadPresetImage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}/output_files.json\n  method: post\n  operationId: setPresetOutputFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}/output_files.json\n  method: delete\n  operationId: deletePresetOutputFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}/outgoing_services.json\n  method: get\n  operationId: getPresetOutgoingServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/preset/{uuid}/outgoing_services.json\n  method: post\n  operationId: setPresetOutgoingServices\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}/outgoing_services.json\n  method: delete\n  operationId: deletePresetOutgoingServices\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}/algorithms.json\n  method: post\n  operationId: setPresetAlgorithms\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}/metadata.json\n  method: post\n  operationId: setPresetMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}/multi_input_files.json\n  method: post\n  operationId: setPresetMultiInputFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}/multi_input_files.json\n  method: delete\n  operationId: deletePresetMultiInputFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}/multi_input_files/{track_id}.json\n\
  \  method: post\n  operationId: updatePresetMultiInputFileTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}/multi_input_files/{track_id}.json\n  method: delete\n  operationId: deletePresetMultiInputFileTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}/webhook.json\n  method: get\n  operationId: getPresetWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/preset/{uuid}/webhook.json\n  method: post\n  operationId: setPresetWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/preset/{uuid}/webhook.json\n  method: delete\n  operationId: deletePresetWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/services.json\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/service/{uuid}/ls.json\n  method: get\n  operationId: listServiceFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/service/connect.json\n  method: post\n  operationId: connectService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/info.json\n  method: get\n  operationId: getAllInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/info/{subject}.json\n  method: get\n  operationId: getInfo\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/user.json\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/download/{dtype}/{uuid}/{filename}\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/agentic-access/auphonic-agentic-access.yml
summary_line: 60 operations · 45 acting · 17 human-in-the-loop
tags:
- Audio
- Podcasts
- Artificial Intelligence
- Automation
- Media
---
