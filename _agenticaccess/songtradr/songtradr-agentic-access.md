---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 11
api_specs:
- filename: songtradr-allowed-values-api-openapi.yml
  format: yaml
  label: Songtradr Allowed Values API
  slug: songtradr-allowed-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songtradr/refs/heads/main/openapi/songtradr-allowed-values-api-openapi.yml
- filename: songtradr-similarity-vector-controller-api-openapi.yml
  format: yaml
  label: Songtradr Similarity Vector Controller API
  slug: songtradr-similarity-vector-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songtradr/refs/heads/main/openapi/songtradr-similarity-vector-controller-api-openapi.yml
- filename: songtradr-user-api-openapi.yml
  format: yaml
  label: Songtradr User API
  slug: songtradr-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songtradr/refs/heads/main/openapi/songtradr-user-api-openapi.yml
consequence_counts:
  read: 11
  safety-critical: 2
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Songtradr Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/user/forgot-password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/user/update-password
operation_count: 19
overview: 'Songtradr exposes 19 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 6 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Songtradr
provider_slug: songtradr
slug: songtradr-agentic-access
source_filename: songtradr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/songtradr-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 8\n    connected: 11\n  by_consequence:\n    safety-critical: 2\n    write: 6\n    read: 11\n  human_in_the_loop_required: 2\noperations:\n- path: /api/v1/user/update-password\n  method: post\n  operationId: updatePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/user/token\n  method: post\n\
  \  operationId: token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/user/sign-up\n  method: post\n  operationId: signUp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/user/me\n  method: get\n  operationId: me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/me\n  method: post\n  operationId: editMe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/user/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/user/forgot-password\n  method: post\n  operationId: forgotPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/user/file/{name}/initUpload\n  method: post\n  operationId:\
  \ initiateUserFileUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/user/recording/{ids}\n  method: get\n  operationId: recordingsMediumByIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/recording/{ids}/tagstrengths\n  method: get\n  operationId: recordingsByIdsWithTagstrengths\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/recording/{ids}/taggrams\n  method: get\n  operationId: recordingsByIdsWithTaggrams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/folder/{folderName}/tagstrengths\n  method: get\n  operationId: recordingsByFolderWithTagstrengths\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/files\n  method: get\n  operationId: userFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/filesSummary\n  method: get\n  operationId: userFilesSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/filesStatus\n  method: get\n  operationId: userFilesStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/file/{objectKey}\n\
  \  method: get\n  operationId: userFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user/file/{objectKey}\n  method: delete\n  operationId: deleteUserFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/similarityVectors/{isrcOrTrackId}\n  method: get\n  operationId: getSimilarityVector\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/allowedValues/musicalFeatures\n  method: get\n  operationId: allowedMusicalFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/songtradr/refs/heads/main/agentic-access/songtradr-agentic-access.yml
summary_line: 19 operations · 8 acting · 2 human-in-the-loop
tags:
- music
- music-licensing
- sync-licensing
- music-metadata
- audio-tagging
- semantic-search
- machine-learning
- media
- entertainment
- rights-management
- audio
---
