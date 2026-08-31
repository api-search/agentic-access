---
acting_count: 0
action_class_counts:
  connected: 30
api_specs:
- filename: words-categories-api-openapi.yml
  format: yaml
  label: Words API Categories API
  slug: words-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-categories-api-openapi.yml
- filename: words-definitions-api-openapi.yml
  format: yaml
  label: Words API Definitions API
  slug: words-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-definitions-api-openapi.yml
- filename: words-examples-api-openapi.yml
  format: yaml
  label: Words API Examples API
  slug: words-examples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-examples-api-openapi.yml
- filename: words-frequency-api-openapi.yml
  format: yaml
  label: Words API Frequency API
  slug: words-frequency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-frequency-api-openapi.yml
- filename: words-hierarchy-api-openapi.yml
  format: yaml
  label: Words API Hierarchy API
  slug: words-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-hierarchy-api-openapi.yml
- filename: words-phonetics-api-openapi.yml
  format: yaml
  label: Words API Phonetics API
  slug: words-phonetics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-phonetics-api-openapi.yml
- filename: words-search-api-openapi.yml
  format: yaml
  label: Words API Search API
  slug: words-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-search-api-openapi.yml
- filename: words-thesaurus-api-openapi.yml
  format: yaml
  label: Words API Thesaurus API
  slug: words-thesaurus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-thesaurus-api-openapi.yml
- filename: words-word-api-openapi.yml
  format: yaml
  label: Words API Word API
  slug: words-word-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-word-api-openapi.yml
consequence_counts:
  read: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Words Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'Words API exposes 30 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Words API
provider_slug: words
slug: words-agentic-access
source_filename: words-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/words-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 30\n  by_consequence:\n    read: 30\n  human_in_the_loop_required: 0\noperations:\n- path: /words/{word}\n  method: get\n  operationId: getWord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/definitions\n  method: get\n  operationId: getDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/synonyms\n  method: get\n  operationId: getSynonyms\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/antonyms\n  method: get\n  operationId: getAntonyms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/examples\n  method: get\n  operationId: getExamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/rhymes\n  method: get\n  operationId: getRhymes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/frequency\n  method: get\n  operationId: getFrequency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /words/{word}/syllables\n  method: get\n  operationId: getSyllables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/pronunciation\n  method: get\n  operationId: getPronunciation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/hasTypes\n  method: get\n  operationId: getHasTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/typeOf\n  method: get\n  operationId: getTypeOf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/partOf\n  method: get\n  operationId: getPartOf\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/hasParts\n  method: get\n  operationId: getHasParts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/instances\n  method: get\n  operationId: getInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/instanceOf\n  method: get\n  operationId: getInstanceOf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/similar\n  method: get\n  operationId: getSimilarTo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /words/{word}/also\n  method: get\n  operationId: getAlso\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/entails\n  method: get\n  operationId: getEntails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/memberOf\n  method: get\n  operationId: getMemberOf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/hasMembers\n  method: get\n  operationId: getHasMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/substanceOf\n  method: get\n  operationId: getSubstanceOf\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/hasSubstances\n  method: get\n  operationId: getHasSubstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/inCategory\n  method: get\n  operationId: getInCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/hasCategories\n  method: get\n  operationId: getHasCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/usageOf\n  method: get\n  operationId: getUsageOf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /words/{word}/hasUsages\n  method: get\n  operationId: getHasUsages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/inRegion\n  method: get\n  operationId: getInRegion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/regionOf\n  method: get\n  operationId: getRegionOf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/{word}/pertainsTo\n  method: get\n  operationId: getPertainsTo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /words/\n  method: get\n  operationId: searchWords\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/agentic-access/words-agentic-access.yml
summary_line: 30 operations
tags:
- Dictionaries
- Linguistics
- English
- Thesaurus
- Lexical Data
- Public APIs
---
