---
acting_count: 30
action_class_counts:
  acting: 30
  connected: 25
api_specs:
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Translation API
  slug: systran-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN File Translation API
  slug: systran-file-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Supported Languages API
  slug: systran-supported-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Language Detection API
  slug: systran-language-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN NLP API
  slug: systran-nlp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Dictionary API
  slug: systran-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Profiles API
  slug: systran-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
- filename: systran-openapi.yml
  format: yaml
  label: SYSTRAN Corpus API
  slug: systran-corpus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/openapi/systran-openapi.yml
consequence_counts:
  read: 25
  write: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Systran Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 55
overview: 'SYSTRAN exposes 55 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read and 30 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SYSTRAN
provider_slug: systran
slug: systran-agentic-access
source_filename: systran-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/systran-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 55\n  by_action_class:\n    acting: 30\n    connected: 25\n  by_consequence:\n    write: 30\n    read: 25\n  human_in_the_loop_required: 0\noperations:\n- path: /translation/text/translate\n  method: post\n  operationId: translateText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /translation/apiVersion\n  method: get\n  operationId: getTranslationApiVersion\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translation/supportedLanguages\n  method: get\n  operationId: getSupportedLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translation/supportedFeatures\n  method: get\n  operationId: getSupportedFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translation/supportedFormats\n  method: get\n  operationId: getSupportedFormats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translation/supportedSelectors\n  method: get\n  operationId: getSupportedSelectors\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translation/profiles\n  method: get\n  operationId: listTranslationProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translation/feedback/add\n  method: post\n  operationId: addTranslationFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /translation/file/translate\n  method: post\n  operationId: translateFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /translation/file/status\n  method: get\n  operationId: getFileTranslationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translation/file/result\n  method: get\n  operationId: getFileTranslationResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translation/file/cancel\n  method: post\n  operationId: cancelFileTranslation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /translation/file/batch/create\n  method: post\n  operationId: createTranslationBatch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /translation/file/batch/status\n  method: get\n  operationId: getTranslationBatchStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translation/file/batch/close\n  method: post\n  operationId: closeTranslationBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /translation/file/batch/cancel\n  method: post\n  operationId: cancelTranslationBatch\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/dictionary/lookup\n  method: get\n  operationId: dictionaryLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/dictionary/lookup/supportedLanguages\n  method: get\n  operationId: dictionaryLookupSupportedLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/dictionary/supportedLanguages\n  method: get\n  operationId: dictionarySupportedLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/dictionary/list\n\
  \  method: post\n  operationId: listDictionaries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/dictionary/add\n  method: post\n  operationId: addDictionary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/dictionary/update\n  method: post\n  operationId: updateDictionary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /resources/dictionary/delete\n  method: post\n  operationId: deleteDictionary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/dictionary/export\n  method: post\n  operationId: exportDictionary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/dictionary/apply\n  method: post\n  operationId: applyDictionary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/dictionary/entry/list\n  method: post\n  operationId: listDictionaryEntries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/dictionary/entry/add\n  method: post\n  operationId: addDictionaryEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/dictionary/entry/update\n  method: post\n  operationId: updateDictionaryEntry\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/dictionary/entry/delete\n  method: post\n  operationId: deleteDictionaryEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/dictionary/entry/import\n  method: post\n  operationId: importDictionaryEntries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /profiles\n  method: get\n  operationId: listProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/create\n  method: post\n  operationId: createProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/delete\n  method: post\n  operationId: deleteProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/activate\n  method: post\n  operationId: activateProfile\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/deactivate\n  method: post\n  operationId: deactivateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{id}/permissions\n  method: get\n  operationId: getProfilePermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{id}/permissions\n  method: post\n  operationId: updateProfilePermissions\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /translationResources\n  method: get\n  operationId: listTranslationResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/corpus/list\n  method: get\n  operationId: listCorpora\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/corpus/add\n  method: post\n  operationId: addCorpus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /resources/corpus/import\n  method: post\n  operationId: importCorpus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/corpus/details\n  method: get\n  operationId: getCorpusDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/corpus/match\n  method: get\n  operationId: matchCorpus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/corpus/update\n  method: post\n  operationId: updateCorpus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/corpus/delete\n  method: post\n  operationId: deleteCorpus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/corpus/segment/list\n  method: get\n  operationId: listCorpusSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resources/corpus/segment/add\n  method: post\n  operationId: addCorpusSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/corpus/segment/update\n  method: post\n  operationId: updateCorpusSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resources/corpus/segment/delete\n  method: post\n  operationId: deleteCorpusSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nlp/lid/detectLanguage\n  method: get\n  operationId: detectLanguage\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nlp/lid/supportedLanguages\n  method: get\n  operationId: lidSupportedLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nlp/morphology/extractRoots\n  method: get\n  operationId: extractRoots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nlp/tokenization/tokenize\n  method: get\n  operationId: tokenize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nlp/segmentation/segment\n  method: get\n  operationId: segment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /nlp/ner/extractNamedEntities\n  method: get\n  operationId: extractNamedEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/systran/refs/heads/main/agentic-access/systran-agentic-access.yml
summary_line: 55 operations · 30 acting
tags:
- Machine Translation
- Translation
- NLP
- Neural Machine Translation
- Localization
- Language Detection
---
