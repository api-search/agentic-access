---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 20
api_specs:
- filename: alation-aggregated-context-api-openapi.yml
  format: yaml
  label: Alation Aggregated Context API
  slug: alation-aggregated-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-aggregated-context-api-openapi.yml
- filename: alation-columns-api-openapi.yml
  format: yaml
  label: Alation Columns API
  slug: alation-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-columns-api-openapi.yml
- filename: alation-custom-fields-api-openapi.yml
  format: yaml
  label: Alation Custom Fields API
  slug: alation-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-custom-fields-api-openapi.yml
- filename: alation-data-quality-api-openapi.yml
  format: yaml
  label: Alation Data Quality API
  slug: alation-data-quality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-data-quality-api-openapi.yml
- filename: alation-data-sources-api-openapi.yml
  format: yaml
  label: Alation Data Sources API
  slug: alation-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-data-sources-api-openapi.yml
- filename: alation-dataflows-api-openapi.yml
  format: yaml
  label: Alation Dataflows API
  slug: alation-dataflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-dataflows-api-openapi.yml
- filename: alation-glossary-terms-api-openapi.yml
  format: yaml
  label: Alation Glossary Terms API
  slug: alation-glossary-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-glossary-terms-api-openapi.yml
- filename: alation-lineage-api-openapi.yml
  format: yaml
  label: Alation Lineage API
  slug: alation-lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-lineage-api-openapi.yml
- filename: alation-policies-api-openapi.yml
  format: yaml
  label: Alation Policies API
  slug: alation-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-policies-api-openapi.yml
- filename: alation-schemas-api-openapi.yml
  format: yaml
  label: Alation Schemas API
  slug: alation-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-schemas-api-openapi.yml
- filename: alation-search-api-openapi.yml
  format: yaml
  label: Alation Search API
  slug: alation-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-search-api-openapi.yml
- filename: alation-tables-api-openapi.yml
  format: yaml
  label: Alation Tables API
  slug: alation-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-tables-api-openapi.yml
consequence_counts:
  read: 20
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Alation Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'Alation exposes 30 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Alation
provider_slug: alation
slug: alation-agentic-access
source_filename: alation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/alation-data-catalog-openapi.yaml, openapi/alation-governance-openapi.yaml,\n  openapi/alation-lineage-openapi.yaml, openapi/alation-search-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 20\n    acting: 10\n  by_consequence:\n    read: 20\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /datasource/\n  method: get\n  operationId: listDataSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasource/{id}/\n  method: get\n  operationId: getDataSource\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schema/\n  method: get\n  operationId: listSchemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schema/{id}/\n  method: get\n  operationId: getSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /table/\n  method: get\n  operationId: listTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /table/{id}/\n  method: get\n  operationId: getTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attribute/\n  method: get\n  operationId: listColumns\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_field_value/\n  method: get\n  operationId: listCustomFieldValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_field_value/\n  method: put\n  operationId: updateCustomFieldValues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /glossary_term/\n  method: get\n  operationId: listGlossaryTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /glossary_term/\n  method: post\n  operationId: createGlossaryTerm\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /glossary_term/{id}/\n  method: get\n  operationId: getGlossaryTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /glossary_term/{id}/\n  method: put\n  operationId: updateGlossaryTerm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /glossary_term/{id}/\n  method: delete\n  operationId: deleteGlossaryTerm\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/\n  method: get\n  operationId: listPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/\n  method: post\n  operationId: createPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/{id}/\n  method: get\n  operationId: getPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data_quality/rule/\n\
  \  method: get\n  operationId: listDataQualityRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data_quality/rule/\n  method: post\n  operationId: createDataQualityRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data_quality/score/\n  method: get\n  operationId: getDataQualityScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataflow/\n  method: get\n  operationId: listDataflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /dataflow/\n  method: post\n  operationId: createDataflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dataflow/{id}/\n  method: get\n  operationId: getDataflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataflow/{id}/\n  method: put\n  operationId: updateDataflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dataflow/{id}/\n  method: delete\n  operationId: deleteDataflow\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lineage/\n  method: get\n  operationId: getLineage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/\n  method: get\n  operationId: searchCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aggregated_context/\n  method: post\n  operationId: getAggregatedContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /article/\n  method: get\n  operationId: listArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /article/{id}/\n  method: get\n  operationId: getArticle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/agentic-access/alation-agentic-access.yml
summary_line: 30 operations · 10 acting
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
---
