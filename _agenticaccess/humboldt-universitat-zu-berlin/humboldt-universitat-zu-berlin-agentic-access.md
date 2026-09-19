---
acting_count: 0
action_class_counts:
  connected: 31
api_specs:
- filename: humboldt-universitat-zu-berlin-core-api-openapi.yml
  format: yaml
  label: edoc-Server DSpace REST API
  slug: edoc-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humboldt-universitat-zu-berlin/refs/heads/main/openapi/humboldt-universitat-zu-berlin-core-api-openapi.yml
- filename: humboldt-universitat-zu-berlin-oai-pmh-api-openapi.yml
  format: yaml
  label: edoc-Server OAI-PMH 2.0 Interface
  slug: edoc-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humboldt-universitat-zu-berlin/refs/heads/main/openapi/humboldt-universitat-zu-berlin-oai-pmh-api-openapi.yml
- filename: humboldt-universitat-zu-berlin-annotations-api-openapi.yml
  format: yaml
  label: Humboldt-Universität zu Berlin Annotations API
  slug: humboldt-universitat-zu-berlin-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humboldt-universitat-zu-berlin/refs/heads/main/openapi/humboldt-universitat-zu-berlin-annotations-api-openapi.yml
- filename: humboldt-universitat-zu-berlin-corpora-api-openapi.yml
  format: yaml
  label: Humboldt-Universität zu Berlin Corpora API
  slug: humboldt-universitat-zu-berlin-corpora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humboldt-universitat-zu-berlin/refs/heads/main/openapi/humboldt-universitat-zu-berlin-corpora-api-openapi.yml
- filename: humboldt-universitat-zu-berlin-documents-api-openapi.yml
  format: yaml
  label: Humboldt-Universität zu Berlin Documents API
  slug: humboldt-universitat-zu-berlin-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humboldt-universitat-zu-berlin/refs/heads/main/openapi/humboldt-universitat-zu-berlin-documents-api-openapi.yml
consequence_counts:
  read: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Humboldt Universitat Zu Berlin Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 31
overview: 'Humboldt-Universität zu Berlin exposes 31 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Humboldt-Universität zu Berlin
provider_slug: humboldt-universitat-zu-berlin
slug: humboldt-universitat-zu-berlin-agentic-access
source_filename: humboldt-universitat-zu-berlin-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/humboldt-universitat-zu-berlin-annotations-api-openapi.yml, openapi/humboldt-universitat-zu-berlin-core-api-openapi.yml,\n  openapi/humboldt-universitat-zu-berlin-corpora-api-openapi.yml, openapi/humboldt-universitat-zu-berlin-discovery-api-openapi.yml,\n  openapi/humboldt-universitat-zu-berlin-documents-api-openapi.yml, openapi/humboldt-universitat-zu-berlin-oai-pmh-api-openapi.yml,\n  openapi/humboldt-universitat-zu-berlin-root-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 31\n  by_consequence:\n    read: 31\n  human_in_the_loop_required: 0\noperations:\n- path: /api/elasticapi/v1/annotations\n  method: get\n  operationId: listAnnotations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/annotations/latest/count\n  method: get\n  operationId: countLatestAnnotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/annotations/latest/{from}/{size}\n  method: get\n  operationId: listLatestAnnotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/annotations/latest/searchMain\n  method: get\n  operationId: searchLatestAnnotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/annotations/latest/searchMain/count\n  method: get\n \
  \ operationId: countSearchLatestAnnotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/annotations/{id}/{index}\n  method: get\n  operationId: getAnnotation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/annotations/{id}/{index}/documents\n  method: get\n  operationId: getAnnotationDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/communities\n  method: get\n  operationId: listCommunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/communities/{uuid}\n  method: get\n  operationId: getCommunity\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/communities/{uuid}/collections\n  method: get\n  operationId: listCommunityCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/collections\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/collections/{uuid}\n  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/items/{uuid}\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/corpora\n  method: get\n  operationId: listCorpora\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/corpora/latest/count\n  method: get\n  operationId: countLatestCorpora\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/corpora/latest/{from}/{size}\n  method: get\n  operationId: listLatestCorpora\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/corpora/latest/searchMain\n  method: get\n  operationId: searchLatestCorpora\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/elasticapi/v1/corpora/latest/searchMain/count\n  method: get\n  operationId: countSearchLatestCorpora\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/corpora/{id}/{index}\n  method: get\n  operationId: getCorpus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/corpora/{id}/{index}/documents\n  method: get\n  operationId: getCorpusDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/corpora/{id}/{index}/annotations\n  method: get\n  operationId: getCorpusAnnotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /discover/search/objects\n  method: get\n  operationId: searchObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/documents/latest/count\n  method: get\n  operationId: countLatestDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/documents/latest/{from}/{size}\n  method: get\n  operationId: listLatestDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/documents/latest/searchMain\n\
  \  method: get\n  operationId: searchLatestDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/documents/latest/searchMain/count\n  method: get\n  operationId: countSearchLatestDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/documents/{id}/{index}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/elasticapi/v1/documents/{id}/{index}/annotations\n  method: get\n  operationId: getDocumentAnnotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /request\n  method: get\n\
  \  operationId: oaiRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getApiRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humboldt-universitat-zu-berlin/refs/heads/main/agentic-access/humboldt-universitat-zu-berlin-agentic-access.yml
summary_line: 31 operations
tags:
- University
- Higher Education
- Education
- Research
- Germany
- Berlin
- Institutional Repository
- Research Data
- Open Access
- Library
- Identity Federation
- OAI-PMH
- DataCite
- Shibboleth
- Corpus Linguistics
---
