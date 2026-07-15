---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 9
api_specs:
- filename: tolgee-openapi.yml
  format: yaml
  label: Tolgee Projects API
  slug: projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-openapi.yml
- filename: tolgee-openapi.yml
  format: yaml
  label: Tolgee Keys API
  slug: keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-openapi.yml
- filename: tolgee-openapi.yml
  format: yaml
  label: Tolgee Translations API
  slug: translations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-openapi.yml
- filename: tolgee-openapi.yml
  format: yaml
  label: Tolgee Languages API
  slug: languages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-openapi.yml
- filename: tolgee-openapi.yml
  format: yaml
  label: Tolgee Import/Export API
  slug: import-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-openapi.yml
- filename: tolgee-openapi.yml
  format: yaml
  label: Tolgee Screenshots API
  slug: screenshots
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/openapi/tolgee-openapi.yml
consequence_counts:
  read: 9
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tolgee Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Tolgee exposes 25 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tolgee
provider_slug: tolgee
slug: tolgee-agentic-access
source_filename: tolgee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tolgee-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 9\n    acting: 16\n  by_consequence:\n    read: 9\n    write: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/api-keys/current\n  method: get\n  operationId: getCurrentApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects\n  method: get\n  operationId: getAllProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects\n  method: post\n\
  \  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{projectId}\n  method: put\n  operationId: editProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}/keys\n  method: get\n  operationId: getKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{projectId}/keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}/keys/{id}\n  method: delete\n  operationId: deleteKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}/keys/search\n  method: get\n  operationId: searchForKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{projectId}/keys/import\n  method: post\n  operationId: importKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}/translations\n  method: get\n  operationId: getTranslations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/projects/{projectId}/translations\n  method: put\n  operationId: setTranslations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}/translations\n  method: post\n  operationId: createOrUpdateTranslations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}/translations/{translationId}/set-state/{state}\n  method: put\n  operationId: setTranslationState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}/languages\n  method: get\n  operationId: getLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{projectId}/languages\n  method: post\n  operationId: createLanguage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}/languages/{languageId}\n  method: put\n  operationId: editLanguage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}/languages/{languageId}\n  method: delete\n  operationId: deleteLanguage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/export\n  method: get\n  operationId: exportData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{projectId}/import\n  method: post\n  operationId: addImportFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}/import/apply\n  method: put\n  operationId: applyImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}/keys/{keyId}/screenshots\n  method: get\n  operationId: getKeyScreenshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/projects/{projectId}/keys/{keyId}/screenshots\n  method: post\n  operationId: uploadScreenshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/projects/{projectId}/keys/{keyId}/screenshots/{screenshotId}\n  method: delete\n  operationId: deleteScreenshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tolgee/refs/heads/main/agentic-access/tolgee-agentic-access.yml
summary_line: 25 operations · 16 acting
tags:
- Localization
- i18n
- Translation
- Open Source
- Developer Tools
---
