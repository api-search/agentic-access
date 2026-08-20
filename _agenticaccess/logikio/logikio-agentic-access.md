---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 20
api_specs:
- filename: logikio-blueprint-export-api-openapi.yml
  format: yaml
  label: Logik.io Blueprint > Export API
  slug: logikio-blueprint-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-blueprint-export-api-openapi.yml
- filename: logikio-blueprint-import-api-openapi.yml
  format: yaml
  label: Logik.io Blueprint > Import API
  slug: logikio-blueprint-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-blueprint-import-api-openapi.yml
- filename: logikio-bom-api-openapi.yml
  format: yaml
  label: Logik.io BOM API
  slug: logikio-bom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-bom-api-openapi.yml
- filename: logikio-configuration-api-openapi.yml
  format: yaml
  label: Logik.io Configuration API
  slug: logikio-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-configuration-api-openapi.yml
- filename: logikio-configuration-v2-api-openapi.yml
  format: yaml
  label: Logik.io Configuration (V2) API
  slug: logikio-configuration-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-configuration-v2-api-openapi.yml
- filename: logikio-managed-tables-export-tables-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Export Tables API
  slug: logikio-managed-tables-export-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-export-tables-api-openapi.yml
- filename: logikio-managed-tables-import-tables-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Import Tables API
  slug: logikio-managed-tables-import-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-import-tables-api-openapi.yml
- filename: logikio-managed-tables-metadata-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Metadata API
  slug: logikio-managed-tables-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-metadata-api-openapi.yml
- filename: logikio-managed-tables-table-rows-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Table Rows API
  slug: logikio-managed-tables-table-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-table-rows-api-openapi.yml
- filename: logikio-managed-tables-tables-api-openapi.yml
  format: yaml
  label: Logik.io Managed Tables > Tables API
  slug: logikio-managed-tables-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-managed-tables-tables-api-openapi.yml
- filename: logikio-runtime-bill-of-materials-api-openapi.yml
  format: yaml
  label: Logik.io Runtime - Bill of Materials API
  slug: logikio-runtime-bill-of-materials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/openapi/logikio-runtime-bill-of-materials-api-openapi.yml
consequence_counts:
  read: 20
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Logikio Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 36
overview: 'Logik.io exposes 36 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Logik.io
provider_slug: logikio
slug: logikio-agentic-access
source_filename: logikio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/logikio-admin-blueprint-openapi-original.yml, openapi/logikio-admin-managed-tables-openapi-original.yml,\n  openapi/logikio-runtime-v1-openapi-original.yml, openapi/logikio-runtime-v2-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 16\n    connected: 20\n  by_consequence:\n    write: 16\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /api/admin/v1/bulk/blueprints/export\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/v2/uploadFile\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/admin/v1/job/{jobId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/admin/v2/bulk/export/{jobId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/managedTables/v1/managedTables\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/managedTables/v1/managedTables\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/managedTables/v2/managedTables/{tableName}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/managedTables/v2/managedTables/{tableName}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/managedTables/v2/managedTables/{tableName}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/managedTables/v2/managedTables/{tableName}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/managedTables/v1/managedTables/{tableName}/metadata\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/managedTables/v1/managedTables/{tableName}/metadata/columns\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/managedTables/v1/managedTables/{tableName}/metadata/columns/{columnName}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/managedTables/v1/managedTables/{tableName}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/managedTables/v1/managedTables/{tableName}/{rowId}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/managedTables/v1/managedTables/{tableName}/{rowId}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/managedTables/v1/managedTables/{tableName}/{rowId}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/managedTables/v3/managedTables/{tableName}/export\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/managedTables/v2/job/{tableExportJobId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/managedTables/v2/job/{tableExportJobId}/file\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: initConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{uuid}\n  method: get\n  operationId: getConfig\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{uuid}\n  method: patch\n  operationId: updateConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{uuid}/sets/{setVariableName}\n  method: get\n  operationId: getSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{uuid}/bom/sales\n  method: get\n  operationId: getSalesBOM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{uuid}/bom/{custom}\n  method: get\n  operationId: getCustomBOM\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{uuid}/bom/manufacturing\n  method: get\n  operationId: getManufacturingBOM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{uuid}/bom/\n  method: get\n  operationId: getAllBOM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api\n  method: post\n  operationId: startConfigV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/{uuid}\n  method: get\n  operationId: getConfigByUuidV2\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/{uuid}\n  method: patch\n  operationId: updateConfigByUuidV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/{uuid}/sets/{setVariableName}\n  method: get\n  operationId: getSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/{uuid}/bom\n  method: get\n  operationId: getAllBomV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/{uuid}/bom/sales\n  method: get\n  operationId: getSalesBomV2\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/{uuid}/bom/manufacturing\n  method: get\n  operationId: getManufacturingBomV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/{uuid}/bom/{custom}\n  method: get\n  operationId: getBomByNameV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logikio/refs/heads/main/agentic-access/logikio-agentic-access.yml
summary_line: 36 operations · 16 acting
tags:
- Company
- Sales Tech
- CPQ
- Product Configuration
- Bill of Materials
- E-Commerce
- Salesforce
- API-First
---
