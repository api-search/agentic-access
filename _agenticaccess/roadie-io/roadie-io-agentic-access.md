---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 14
api_specs:
- filename: roadie-io-openapi.yml
  format: yaml
  label: Roadie Catalog API
  slug: roadie-io-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadie-io/refs/heads/main/openapi/roadie-io-openapi.yml
- filename: roadie-io-openapi.yml
  format: yaml
  label: Roadie Entity Push API
  slug: roadie-io-entity-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadie-io/refs/heads/main/openapi/roadie-io-openapi.yml
- filename: roadie-io-openapi.yml
  format: yaml
  label: Roadie Scaffolder API
  slug: roadie-io-scaffolder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadie-io/refs/heads/main/openapi/roadie-io-openapi.yml
- filename: roadie-io-openapi.yml
  format: yaml
  label: Roadie Tech Insights API
  slug: roadie-io-tech-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadie-io/refs/heads/main/openapi/roadie-io-openapi.yml
- filename: roadie-io-openapi.yml
  format: yaml
  label: Roadie TechDocs API
  slug: roadie-io-techdocs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadie-io/refs/heads/main/openapi/roadie-io-openapi.yml
consequence_counts:
  read: 14
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Roadie Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Roadie exposes 21 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Roadie
provider_slug: roadie-io
slug: roadie-io-agentic-access
source_filename: roadie-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/roadie-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 14\n    acting: 7\n  by_consequence:\n    read: 14\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /catalog/entities\n  method: get\n  operationId: listCatalogEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/entities/by-query\n  method: get\n  operationId: queryCatalogEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/entities/by-name/{kind}/{namespace}/{name}\n\
  \  method: get\n  operationId: getCatalogEntityByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/entity-facets\n  method: get\n  operationId: getEntityFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/roadie-entities/entities\n  method: post\n  operationId: createRoadieEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/roadie-entities/entities/{entityId}\n  method: get\n  operationId: getRoadieEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /catalog/roadie-entities/entities/{entityId}\n  method: delete\n  operationId: deleteRoadieEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/roadie-entities/sets/{setName}\n  method: put\n  operationId: upsertEntitySet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /catalog/roadie-entities/sets/{setName}\n  method: delete\n  operationId: deleteEntitySet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scaffolder/v2/actions\n  method: get\n  operationId: listScaffolderActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scaffolder/v2/tasks\n  method: get\n  operationId: listScaffolderTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scaffolder/v2/tasks\n  method: post\n  operationId: createScaffolderTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scaffolder/v2/tasks/{taskId}\n\
  \  method: get\n  operationId: getScaffolderTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scaffolder/v2/tasks/{taskId}/eventstream\n  method: get\n  operationId: streamScaffolderTaskEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scaffolder/v2/dry-run\n  method: post\n  operationId: dryRunScaffolderTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tech-insights/v1/facts\n  method: get\n  operationId: listTechInsightsFacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /tech-insights/v1/checks\n  method: get\n  operationId: listTechInsightsChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tech-insights/v1/checks/run\n  method: post\n  operationId: runTechInsightsChecks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tech-insights/v1/scorecards\n  method: get\n  operationId: listScorecards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /techdocs/metadata/entity/{namespace}/{kind}/{name}\n  method: get\n  operationId: getTechDocsMetadata\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /techdocs/static/docs/{namespace}/{kind}/{name}/{path}\n  method: get\n  operationId: getTechDocsStatic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roadie-io/refs/heads/main/agentic-access/roadie-io-agentic-access.yml
summary_line: 21 operations · 7 acting
tags:
- Software Catalog
- Internal Developer Portal
- Backstage
- Developer Experience
- IDP
- Developer Portal
- Managed Backstage
- Scaffolder
- TechDocs
- Service Catalog
- Platform Engineering
---
