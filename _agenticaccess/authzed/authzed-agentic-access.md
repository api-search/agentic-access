---
acting_count: 27
action_class_counts:
  acting: 27
api_specs:
- filename: client-libraries
  format: yaml
  label: SpiceDB Permissions API
  slug: spicedb-permissions-api
  spec_type: OpenAPI
  url: https://authzed.com/docs/spicedb/getting-started/client-libraries
consequence_counts:
  physical: 13
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Authzed Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/experimental/countrelationships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/experimental/registerrelationshipcounter
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/experimental/relationships/bulkexport
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/experimental/relationships/bulkimport
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/experimental/unregisterrelationshipcounter
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/permissions/resources
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/permissions/subjects
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/relationships/delete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/relationships/exportbulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/relationships/importbulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/relationships/read
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/relationships/write
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/watch
operation_count: 27
overview: 'Authzed exposes 27 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 write and 13 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Authzed
provider_slug: authzed
slug: authzed-agentic-access
source_filename: authzed-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/authzed-spicedb-permissions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 27\n  by_consequence:\n    physical: 13\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/experimental/countrelationships\n  method: post\n  operationId: ExperimentalService_ExperimentalCountRelationships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/experimental/diffschema\n  method: post\n  operationId: ExperimentalService_ExperimentalDiffSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experimental/permissions/bulkcheckpermission\n  method: post\n  operationId: ExperimentalService_BulkCheckPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experimental/permissions/computable\n  method: post\n  operationId: ExperimentalService_ExperimentalComputablePermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experimental/permissions/dependent\n  method: post\n  operationId: ExperimentalService_ExperimentalDependentRelations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experimental/reflectschema\n  method: post\n  operationId: ExperimentalService_ExperimentalReflectSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/experimental/registerrelationshipcounter\n  method: post\n  operationId: ExperimentalService_ExperimentalRegisterRelationshipCounter\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experimental/relationships/bulkexport\n  method: post\n  operationId: ExperimentalService_BulkExportRelationships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experimental/relationships/bulkimport\n\
  \  method: post\n  operationId: ExperimentalService_BulkImportRelationships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/experimental/unregisterrelationshipcounter\n  method: post\n  operationId: ExperimentalService_ExperimentalUnregisterRelationshipCounter\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/permissions/check\n  method: post\n  operationId: PermissionsService_CheckPermission\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/permissions/checkbulk\n  method: post\n  operationId: PermissionsService_CheckBulkPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/permissions/expand\n  method: post\n  operationId: PermissionsService_ExpandPermissionTree\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/permissions/resources\n  method: post\n  operationId: PermissionsService_LookupResources\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/permissions/subjects\n  method: post\n  operationId: PermissionsService_LookupSubjects\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/relationships/delete\n  method: post\n  operationId: PermissionsService_DeleteRelationships\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/relationships/exportbulk\n  method: post\n  operationId: PermissionsService_ExportBulkRelationships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/relationships/importbulk\n  method: post\n  operationId: PermissionsService_ImportBulkRelationships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/relationships/read\n  method: post\n  operationId: PermissionsService_ReadRelationships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/relationships/write\n  method: post\n  operationId: PermissionsService_WriteRelationships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schema/diffschema\n  method: post\n  operationId: SchemaService_DiffSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schema/permissions/computable\n  method: post\n  operationId: SchemaService_ComputablePermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schema/permissions/dependent\n  method: post\n  operationId: SchemaService_DependentRelations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schema/read\n  method: post\n  operationId: SchemaService_ReadSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schema/reflectschema\n  method: post\n  operationId: SchemaService_ReflectSchema\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/schema/write\n  method: post\n  operationId: SchemaService_WriteSchema\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watch\n  method: post\n  operationId: WatchService_Watch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authzed/refs/heads/main/agentic-access/authzed-agentic-access.yml
summary_line: 27 operations · 27 acting
tags:
- Authorization
- Access Control
- Permissions
- Zanzibar
- SpiceDB
- gRPC
- REST
- Relationship-Based Access Control
- ReBAC
- Fine-Grained Authorization
- Identity
- Security
---
