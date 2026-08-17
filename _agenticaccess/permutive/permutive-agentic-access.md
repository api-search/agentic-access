---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 8
api_specs:
- filename: permutive-cohorts-api-openapi.yml
  format: yaml
  label: Permutive Cohorts API
  slug: permutive-cohorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-cohorts-api-openapi.yml
- filename: permutive-contextual-api-openapi.yml
  format: yaml
  label: Permutive Contextual API
  slug: permutive-contextual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-contextual-api-openapi.yml
- filename: permutive-events-api-openapi.yml
  format: yaml
  label: Permutive Events API
  slug: permutive-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-events-api-openapi.yml
- filename: permutive-identity-api-openapi.yml
  format: yaml
  label: Permutive Identity API
  slug: permutive-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-identity-api-openapi.yml
- filename: permutive-segmentation-api-openapi.yml
  format: yaml
  label: Permutive Segmentation API
  slug: permutive-segmentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-segmentation-api-openapi.yml
- filename: permutive-taxonomy-api-openapi.yml
  format: yaml
  label: Permutive Taxonomy API
  slug: permutive-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-taxonomy-api-openapi.yml
consequence_counts:
  read: 8
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Permutive Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Permutive exposes 23 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Permutive
provider_slug: permutive
slug: permutive-agentic-access
source_filename: permutive-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/permutive-cohorts-api-openapi.yml, openapi/permutive-contextual-api-openapi.yml,\n  openapi/permutive-events-api-openapi.yml, openapi/permutive-identity-api-openapi.yml, openapi/permutive-segmentation-api-openapi.yml,\n  openapi/permutive-taxonomy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 8\n    acting: 15\n  by_consequence:\n    read: 8\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/cohorts\n  method: get\n  operationId: getV2Cohorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cohorts\n\
  \  method: post\n  operationId: postV2Cohorts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/cohorts/{cohortId}\n  method: get\n  operationId: getV2CohortsCohortid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cohorts/{cohortId}\n  method: delete\n  operationId: deleteV2CohortsCohortid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/cohorts/{cohortId}\n  method: patch\n  operationId: patchV2CohortsCohortid\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ctx/v1/segment\n  method: post\n  operationId: getContextualSegments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: post\n  operationId: createEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: post\n\
  \  operationId: createUserId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identify\n  method: post\n  operationId: identifyUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/aliases\n  method: get\n  operationId: getIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ccs/v1/segmentation\n  method: post\n  operationId: postCcsV1Segmentation\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ccs/v1/segmentation/stateless\n  method: post\n  operationId: postCcsV1SegmentationStateless\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /imports\n  method: get\n  operationId: getImports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /imports/{importId}\n  method: get\n  operationId: getImportsImportid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /imports/{importId}/segments\n  method: get\n  operationId: getImportsImportidSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /imports/{importId}/segments\n  method: post\n  operationId: postImportsImportidSegments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /imports/{importId}/segments\n  method: patch\n  operationId: patchImportsImportidSegments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /imports/{importId}/segments/{segmentId}\n  method: get\n  operationId: getImportsImportidSegmentsSegmentid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /imports/{importId}/segments/{segmentId}\n  method: delete\n  operationId: deleteImportsImportidSegmentsSegmentid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /imports/{importId}/segments/{segmentId}\n  method: patch\n  operationId: patchImportsImportidSegmentsSegmentid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /imports/{importId}/segments/code/{segmentCode}\n  method: get\n  operationId: getImportsImportidSegmentsCodeSegmentcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /imports/{importId}/segments/code/{segmentCode}\n  method: delete\n  operationId: deleteImportsImportidSegmentsCodeSegmentcode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /imports/{importId}/segments/code/{segmentCode}\n  method: patch\n  operationId: patchImportsImportidSegmentsCodeSegmentcode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/agentic-access/permutive-agentic-access.yml
summary_line: 23 operations · 15 acting
tags:
- Company
- Publishing
- Advertising
- AdTech
- MarTech
- Audience
- Data Collaboration
- Data Management Platform
- Contextual
- Identity
- Segmentation
- Agents
---
