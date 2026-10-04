---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 11
api_specs:
- filename: mytomorrows-legacy-graphql-proxy-api-openapi.yml
  format: yaml
  label: myTomorrows Legacy GraphQL Proxy API
  slug: mytomorrows-legacy-graphql-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-legacy-graphql-proxy-api-openapi.yml
- filename: mytomorrows-public-api-openapi.yml
  format: yaml
  label: myTomorrows Public API
  slug: mytomorrows-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-public-api-openapi.yml
- filename: mytomorrows-system-api-openapi.yml
  format: yaml
  label: myTomorrows System API
  slug: mytomorrows-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-system-api-openapi.yml
- filename: mytomorrows-anno-api-openapi.yml
  format: yaml
  label: myTomorrows Anno API
  slug: mytomorrows-anno-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-anno-api-openapi.yml
- filename: mytomorrows-autocomplete-api-openapi.yml
  format: yaml
  label: myTomorrows Autocomplete API
  slug: mytomorrows-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-autocomplete-api-openapi.yml
- filename: mytomorrows-docs-api-openapi.yml
  format: yaml
  label: myTomorrows Docs API
  slug: mytomorrows-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-docs-api-openapi.yml
- filename: mytomorrows-document-api-openapi.yml
  format: yaml
  label: myTomorrows Document API
  slug: mytomorrows-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-document-api-openapi.yml
- filename: mytomorrows-es-api-openapi.yml
  format: yaml
  label: myTomorrows Es API
  slug: mytomorrows-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-es-api-openapi.yml
- filename: mytomorrows-llm-api-openapi.yml
  format: yaml
  label: myTomorrows Llm API
  slug: mytomorrows-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-llm-api-openapi.yml
- filename: mytomorrows-mdt-api-openapi.yml
  format: yaml
  label: myTomorrows Mdt API
  slug: mytomorrows-mdt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-mdt-api-openapi.yml
- filename: mytomorrows-search-api-openapi.yml
  format: yaml
  label: myTomorrows Search API
  slug: mytomorrows-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-search-api-openapi.yml
- filename: mytomorrows-wrapper-api-openapi.yml
  format: yaml
  label: myTomorrows Wrapper API
  slug: mytomorrows-wrapper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/openapi/mytomorrows-wrapper-api-openapi.yml
consequence_counts:
  read: 11
  write: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mytomorrows Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 42
overview: 'myTomorrows exposes 42 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 31 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: myTomorrows
provider_slug: mytomorrows
slug: mytomorrows-agentic-access
source_filename: mytomorrows-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/mytomorrows-legacy-graphql-proxy-api-openapi.yml, openapi/mytomorrows-public-api-openapi.yml,\n  openapi/mytomorrows-system-api-openapi.yml, openapi/mytomorrows-v1-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    acting: 31\n    connected: 11\n  by_consequence:\n    write: 31\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /gql/graphql\n  method: post\n  operationId: forward_legacy_graphql_request_gql_graphql_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/\n  method: get\n  operationId: root_es_api__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /es/api/health\n  method: get\n  operationId: health_es_api_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /es/api/v01/docs\n  method: get\n  operationId: api_docs_es_api_v01_docs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /es/api/v01/anno/to_annotate\n  method: post\n  operationId:\
  \ get_annotations_endpoint_es_api_v01_anno_to_annotate_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /es/api/v01/llm/llm_tsr_generate\n  method: post\n  operationId: llm_tsr_generate_endpoint_es_api_v01_llm_llm_tsr_generate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/document/transcribe_documents\n  method: post\n  operationId: document_transcription_endpoint_es_api_v01_document_transcribe_documents_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/anno/process\n  method: post\n  operationId: process_annotations_endpoint_es_api_v01_anno_process_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/search/request_tsr\n  method: post\n  operationId: request_tsr_endpoint_es_api_v01_search_request_tsr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/search/generate_tsr\n  method: post\n  operationId: generate_tsr_endpoint_es_api_v01_search_generate_tsr_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/search/questionnaire\n  method: post\n  operationId: questionnaire_endpoint_es_api_v01_search_questionnaire_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/llm/email_tsr\n  method: post\n  operationId: emailTSR_endpoint_es_api_v01_llm_email_tsr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/llm/request_tsr\n  method: post\n  operationId: llm_tsr_request_endpoint_es_api_v01_llm_request_tsr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/llm/autocomplete_country\n  method: post\n  operationId: autocomplete_country_endpoint_es_api_v01_llm_autocomplete_country_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/llm/autocomplete_aliases\n  method: post\n  operationId: autocomplete_aliases_endpoint_es_api_v01_llm_autocomplete_aliases_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/llm/review_tsr\n  method: post\n  operationId: llm_tsr_review_endpoint_es_api_v01_llm_review_tsr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/autocomplete/autocomplete_aliases_graph\n  method: post\n  operationId: autocomplete_aliases_graph_endpoint_es_api_v01_autocomplete_autocomplete_aliases_graph_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/llm/autocomplete_conditions_synonyms\n  method: post\n  operationId: autocomplete_conditions_endpoint_es_api_v01_llm_autocomplete_conditions_synonyms_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/llm/autocomplete_trial_id\n  method: post\n  operationId: autocomplete_trial_id_endpoint_es_api_v01_llm_autocomplete_trial_id_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /es/api/v01/mdt/request_pdf\n  method: post\n  operationId: mdt_request_pdf_endpoint_es_api_v01_mdt_request_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /es/api/v01/wrapper/autocomplete\n  method: get\n  operationId: autocomplete_wrapper_endpoint_es_api_v01_wrapper_autocomplete_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /es/api/v01/wrapper/study/search/counts\n  method: get\n  operationId: count_wrapper_endpoint_es_api_v01_wrapper_study_search_counts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v01/docs\n  method: get\n  operationId: api_docs_v01_docs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v01/anno/to_annotate\n  method: post\n  operationId: get_annotations_endpoint_v01_anno_to_annotate_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v01/llm/llm_tsr_generate\n  method: post\n  operationId: llm_tsr_generate_endpoint_v01_llm_llm_tsr_generate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v01/document/transcribe_documents\n  method: post\n  operationId: document_transcription_endpoint_v01_document_transcribe_documents_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v01/anno/process\n  method: post\n  operationId: process_annotations_endpoint_v01_anno_process_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v01/search/request_tsr\n  method: post\n  operationId: request_tsr_endpoint_v01_search_request_tsr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /v01/search/generate_tsr\n  method: post\n  operationId: generate_tsr_endpoint_v01_search_generate_tsr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v01/search/questionnaire\n  method: post\n  operationId: questionnaire_endpoint_v01_search_questionnaire_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v01/llm/email_tsr\n  method: post\n  operationId: emailTSR_endpoint_v01_llm_email_tsr_post\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v01/llm/request_tsr\n  method: post\n  operationId: llm_tsr_request_endpoint_v01_llm_request_tsr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v01/llm/autocomplete_country\n  method: post\n  operationId: autocomplete_country_endpoint_v01_llm_autocomplete_country_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v01/llm/autocomplete_aliases\n  method: post\n  operationId: autocomplete_aliases_endpoint_v01_llm_autocomplete_aliases_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v01/llm/review_tsr\n  method: post\n  operationId: llm_tsr_review_endpoint_v01_llm_review_tsr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v01/autocomplete/autocomplete_aliases_graph\n  method: post\n  operationId: autocomplete_aliases_graph_endpoint_v01_autocomplete_autocomplete_aliases_graph_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v01/llm/autocomplete_conditions_synonyms\n  method: post\n  operationId: autocomplete_conditions_endpoint_v01_llm_autocomplete_conditions_synonyms_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v01/llm/autocomplete_trial_id\n  method: post\n  operationId: autocomplete_trial_id_endpoint_v01_llm_autocomplete_trial_id_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v01/mdt/request_pdf\n  method: post\n  operationId: mdt_request_pdf_endpoint_v01_mdt_request_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v01/wrapper/autocomplete\n  method: get\n  operationId: autocomplete_wrapper_endpoint_v01_wrapper_autocomplete_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v01/wrapper/study/search/counts\n  method: get\n  operationId: count_wrapper_endpoint_v01_wrapper_study_search_counts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mytomorrows/refs/heads/main/agentic-access/mytomorrows-agentic-access.yml
summary_line: 42 operations · 31 acting
tags:
- Company
- Healthcare
- Clinical Trials
- Expanded Access
- Pharmaceuticals
- Patient Access
- Life Sciences
- Search
- Artificial Intelligence
---
