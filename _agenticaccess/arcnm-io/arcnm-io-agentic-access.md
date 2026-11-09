---
acting_count: 154
action_class_counts:
  acting: 154
  connected: 91
api_specs:
- filename: arcnm-io-calculations-api-openapi.yml
  format: yaml
  label: ARCNM Calculations API
  slug: arcnm-io-calculations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-calculations-api-openapi.yml
- filename: arcnm-io-calibration-api-openapi.yml
  format: yaml
  label: ARCNM Calibration API
  slug: arcnm-io-calibration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-calibration-api-openapi.yml
- filename: arcnm-io-datasets-api-openapi.yml
  format: yaml
  label: ARCNM Datasets API
  slug: arcnm-io-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-datasets-api-openapi.yml
- filename: arcnm-io-environments-api-openapi.yml
  format: yaml
  label: ARCNM Environments API
  slug: arcnm-io-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-environments-api-openapi.yml
- filename: arcnm-io-folders-api-openapi.yml
  format: yaml
  label: ARCNM Folders API
  slug: arcnm-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-folders-api-openapi.yml
- filename: arcnm-io-geometry-api-openapi.yml
  format: yaml
  label: ARCNM Geometry API
  slug: arcnm-io-geometry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-geometry-api-openapi.yml
- filename: arcnm-io-import-api-openapi.yml
  format: yaml
  label: ARCNM Import API
  slug: arcnm-io-import-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-import-api-openapi.yml
- filename: arcnm-io-machine-library-api-openapi.yml
  format: yaml
  label: ARCNM Machine Library API
  slug: arcnm-io-machine-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-machine-library-api-openapi.yml
- filename: arcnm-io-machines-api-openapi.yml
  format: yaml
  label: ARCNM Machines API
  slug: arcnm-io-machines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-machines-api-openapi.yml
- filename: arcnm-io-materials-api-openapi.yml
  format: yaml
  label: ARCNM Materials API
  slug: arcnm-io-materials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-materials-api-openapi.yml
- filename: arcnm-io-nesting-api-openapi.yml
  format: yaml
  label: ARCNM Nesting API
  slug: arcnm-io-nesting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-nesting-api-openapi.yml
- filename: arcnm-io-parts-api-openapi.yml
  format: yaml
  label: ARCNM Parts API
  slug: arcnm-io-parts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-parts-api-openapi.yml
- filename: arcnm-io-remnants-api-openapi.yml
  format: yaml
  label: ARCNM Remnants API
  slug: arcnm-io-remnants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-remnants-api-openapi.yml
- filename: arcnm-io-subcontractors-api-openapi.yml
  format: yaml
  label: ARCNM Subcontractors API
  slug: arcnm-io-subcontractors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-subcontractors-api-openapi.yml
- filename: arcnm-io-tools-api-openapi.yml
  format: yaml
  label: ARCNM Tools API
  slug: arcnm-io-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-tools-api-openapi.yml
- filename: arcnm-io-upload-links-api-openapi.yml
  format: yaml
  label: ARCNM Upload Links API
  slug: arcnm-io-upload-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-upload-links-api-openapi.yml
- filename: arcnm-io-uploads-api-openapi.yml
  format: yaml
  label: ARCNM Uploads API
  slug: arcnm-io-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-uploads-api-openapi.yml
consequence_counts:
  physical: 7
  read: 91
  safety-critical: 11
  write: 136
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 11
kind: agentic-access
layout: agentic-access
method: generated
name: Arcnm Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/calculations/{calculation_id}/components/{component_key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/environments/clone-preset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/environments/{env_id}/rates/scrap/{material_category}/{scrap_class}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v1/materials/grades/{grade_id}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/materials/overrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/materials/overrides/{override_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/materials/overrides/{override_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/subcontractors/presets/{preset_key}/suppression
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/subcontractors/presets/{preset_key}/suppression
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/tools/{tool_id}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/upload-links/{upload_session_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/calibration/environments/{env_id}/auto-calibrate-from-erp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v1/environments/{env_id}/machines/{membership_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/environments/{env_id}/machines/{membership_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v1/environments/{env_id}/subcontractors/{membership_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/environments/{env_id}/subcontractors/{membership_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v1/environments/{env_id}/tools/{membership_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/environments/{env_id}/tools/{membership_id}
operation_count: 245
overview: 'ARCNM exposes 245 API operations that an AI agent could call, of which 154 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 91 read, 136 write, 7 physical, and 11 safety-critical.


  11 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ARCNM
provider_slug: arcnm-io
slug: arcnm-io-agentic-access
source_filename: arcnm-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/arcnm-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 245\n  by_action_class:\n    acting: 154\n    connected: 91\n  by_consequence:\n    write: 136\n    read: 91\n    safety-critical: 11\n    physical: 7\n  human_in_the_loop_required: 11\noperations:\n- path: /api/v1/uploads/presign\n  method: post\n  operationId: uploads-presign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/uploads/confirm\n  method: post\n  operationId: uploads-confirm\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/uploads/\n  method: get\n  operationId: uploads-list_uploads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/uploads/{data_source_id}/cancel\n  method: post\n  operationId: uploads-cancel_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/uploads/{data_source_id}/retry\n  method: post\n  operationId: uploads-retry_upload\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/uploads/bulk-cancel\n  method: post\n  operationId: uploads-bulk_cancel_uploads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/uploads/bulk-retry\n  method: post\n  operationId: uploads-bulk_retry_uploads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/uploads/{data_source_id}\n  method: patch\n  operationId: uploads-update_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/uploads/{data_source_id}\n  method: delete\n  operationId: uploads-delete_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/uploads/bulk-delete\n  method: post\n  operationId: uploads-bulk_delete_uploads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/uploads/{data_source_id}/download-url\n  method: get\n  operationId: uploads-download_url\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculations\n  method: post\n  operationId: calculations-create_calculation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations\n  method: get\n  operationId: calculations-list_calculations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculations/{calculation_id}/run\n\
  \  method: post\n  operationId: calculations-run_calculation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/inputs\n  method: post\n  operationId: calculations-upload_inputs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/entitlement\n  method: get\n  operationId: calculations-get_entitlement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculations/capacity\n\
  \  method: get\n  operationId: calculations-get_calculation_capacity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculations/{calculation_id}\n  method: get\n  operationId: calculations-get_calculation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculations/{calculation_id}\n  method: delete\n  operationId: calculations-delete_calculation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/bom\n  method: get\n  operationId: calculations-get_calculation_bom\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculations/{calculation_id}/drawings\n  method: post\n  operationId: calculations-upload_assembly_drawings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/drawings/{data_source_id}/assign\n  method: post\n  operationId: calculations-assign_assembly_drawing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/components/{component_key}/drawing\n\
  \  method: post\n  operationId: calculations-upload_component_drawing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/drawing\n  method: post\n  operationId: calculations-assign_drawing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/components/{component_key}/run\n  method: post\n  operationId: calculations-rerun_assembly_component\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/assembly-route\n  method: get\n  operationId: calculations-get_calculation_assembly_route\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculations/{calculation_id}/components/{component_key}\n  method: patch\n  operationId: calculations-patch_assembly_component\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/components\n  method: patch\n  operationId: calculations-patch_assembly_components_sourcing\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/components/calculate\n  method: post\n  operationId: calculations-calculate_assembly_components\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/optimization\n  method: get\n  operationId: calculations-get_calculation_optimization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculations/{calculation_id}/material\n\
  \  method: patch\n  operationId: calculations-patch_calculation_material\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/quote\n  method: post\n  operationId: calculations-quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/upload-and-quote\n  method: post\n  operationId: calculations-upload_and_quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/upload-and-quote-json\n  method: post\n  operationId: calculations-upload_and_quote_json\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/cancel\n  method: post\n  operationId: calculations-cancel_calculation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/bulk-cancel\n  method: post\n  operationId: calculations-bulk_cancel_calculations\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/bulk-retry\n  method: post\n  operationId: calculations-bulk_retry_calculations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/bulk-delete\n  method: post\n  operationId: calculations-bulk_delete_calculations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /api/v1/calculations/batch\n  method: post\n  operationId: calculations-batch_calculate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/batches/{batch_id}/comparison\n  method: get\n  operationId: calculations-batch_comparison\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculations/batches/{batch_id}/comparison/components\n  method: get\n  operationId: calculations-batch_comparison_components\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculations/comparison\n\
  \  method: post\n  operationId: calculations-compare_environment_runs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/batches/{batch_id}/cancel\n  method: post\n  operationId: calculations-cancel_batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/cost-sheet\n  method: get\n  operationId: calculations-get_cost_sheet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/calculations/{calculation_id}/preview\n  method: post\n  operationId: calculations-preview_cost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/scenarios\n  method: get\n  operationId: calculations-list_cost_scenarios\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calculations/{calculation_id}/scenarios\n  method: post\n  operationId: calculations-create_cost_scenario\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/scenarios/{scenario_id}\n  method: patch\n  operationId: calculations-update_cost_scenario\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calculations/{calculation_id}/scenarios/{scenario_id}\n  method: delete\n  operationId: calculations-delete_cost_scenario\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calibration/outcomes\n  method: post\n  operationId: calibration-ingest-environment-outcomes\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calibration/environments/{env_id}/finalize\n  method: post\n  operationId: calibration-finalize-environment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calibration/environments/{env_id}/teach\n  method: post\n  operationId: calibration-teach-environment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calibration/environments/{env_id}/auto-calibrate\n  method: post\n  operationId: calibration-auto-calibrate-environment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calibration/erp-preflight\n  method: post\n  operationId: calibration-erp-preflight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calibration/environments/{env_id}/auto-calibrate-from-erp\n  method: post\n  operationId: calibration-auto-calibrate-from-erp\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calibration/environments/{env_id}/learning-curve-fit\n  method: post\n  operationId: calibration-fit-learning-curve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calibration/environments/{env_id}/policy/calibrate\n  method: post\n  operationId: calibration-calibrate-selection-policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calibration/environments/{env_id}/status\n  method: get\n  operationId: calibration-environment-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calibration/environments/{env_id}/next-best-evidence\n  method: get\n  operationId: calibration-next-best-evidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calibration/environments/{env_id}/calibration-report\n  method: get\n  operationId: calibration-environment-report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calibration/environments/{env_id}/runs\n\
  \  method: get\n  operationId: calibration-environment-run-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calibration/environments/{env_id}/runs/{run_id}/revert\n  method: post\n  operationId: calibration-revert-environment-run\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calibration/environments/{env_id}/deactivate\n  method: post\n  operationId: calibration-deactivate-environment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /api/v1/calibration/imports\n  method: post\n  operationId: calibration-import-create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calibration/imports/{import_id}/price\n  method: post\n  operationId: calibration-import-price\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/calibration/imports/{import_id}\n  method: get\n  operationId: calibration-import-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calibration/imports/{import_id}/calibrate\n  method: post\n  operationId: calibration-import-calibrate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/import/machines/preview\n  method: post\n  operationId: import-preview_machine_import\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/import/machines\n  method: post\n  operationId: import-import_machines\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/import/tools/preview\n  method: post\n  operationId: import-preview_tool_import\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/import/tools\n  method: post\n  operationId: import-import_tools\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments/\n  method: get\n  operationId: environments-list_environments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/environments/presets\n  method: get\n  operationId: environments-list_presets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/environments/surcharge-presets\n  method: get\n  operationId: environments-list_surcharge_presets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/environments/clone-preset\n  method: post\n  operationId: environments-clone_preset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api/v1/environments/{env_id}/clone\n  method: post\n  operationId: environments-clone_environment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments/{env_id}\n  method: get\n  operationId: environments-get_environment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/environments/{env_id}\n  method: delete\n  operationId: environments-delete_environment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments/{env_id}/economics\n  method: patch\n  operationId: environments-economics-update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments\n  method: post\n  operationId: environments-create_environment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments/{env_id}/identity\n  method: put\n  operationId: environments-update_environment_identity\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments/{env_id}/machines\n  method: get\n  operationId: environments-list_env_machines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/environments/{env_id}/machines\n  method: post\n  operationId: environments-attach_machine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments/{env_id}/machines/{membership_id}\n  method: patch\n  operationId: environments-update_membership\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments/{env_id}/machines/{membership_id}\n  method: delete\n  operationId: environments-detach_machine\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments/{env_id}/tools\n  method: get\n  operationId: environments-list_env_tools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/environments/{env_id}/tools\n  method: post\n  operationId: environments-attach_env_tool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments/{env_id}/tools/{membership_id}\n  method: patch\n  operationId: environments-update_env_tool_membership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments/{env_id}/tools/{membership_id}\n  method: delete\n  operationId: environments-detach_env_tool\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments/{env_id}/rates\n  method: get\n  operationId: environments-list_rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/environments/{env_id}/rates\n  method: post\n  operationId: environments-upsert_rate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments/{env_id}/rates/material/{grade_id}\n\
  \  method: put\n  operationId: environments-material-price-set\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/environments/{env_id}/rates/material/{grade_id}\n  method: delete\n  operationId: environments-material-price-clear\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (78 KB total) ---\n# Full source: https://artifacts.apis.io/arcnm-io/agentic-access/arcnm-io-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/arcnm-io/agentic-access/arcnm-io-agentic-access.yml
summary_line: 245 operations · 154 acting · 11 human-in-the-loop
tags:
- Manufacturing
- Costing
- CAD
- Engineering
---
