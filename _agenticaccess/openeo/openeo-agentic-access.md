---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 31
api_specs:
- filename: openeo-account-management-api-openapi.yml
  format: yaml
  label: openEO Account Management API
  slug: openeo-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-account-management-api-openapi.yml
- filename: openeo-batch-jobs-api-openapi.yml
  format: yaml
  label: openEO Batch Jobs API
  slug: openeo-batch-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-batch-jobs-api-openapi.yml
- filename: openeo-capabilities-api-openapi.yml
  format: yaml
  label: openEO Capabilities API
  slug: openeo-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-capabilities-api-openapi.yml
- filename: openeo-data-processing-api-openapi.yml
  format: yaml
  label: openEO Data Processing API
  slug: openeo-data-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-data-processing-api-openapi.yml
- filename: openeo-eo-data-discovery-api-openapi.yml
  format: yaml
  label: openEO EO Data Discovery API
  slug: openeo-eo-data-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-eo-data-discovery-api-openapi.yml
- filename: openeo-file-storage-api-openapi.yml
  format: yaml
  label: openEO File Storage API
  slug: openeo-file-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-file-storage-api-openapi.yml
- filename: openeo-orders-api-openapi.yml
  format: yaml
  label: openEO Orders API
  slug: openeo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-orders-api-openapi.yml
- filename: openeo-process-discovery-api-openapi.yml
  format: yaml
  label: openEO Process Discovery API
  slug: openeo-process-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-process-discovery-api-openapi.yml
- filename: openeo-secondary-services-api-openapi.yml
  format: yaml
  label: openEO Secondary Services API
  slug: openeo-secondary-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-secondary-services-api-openapi.yml
- filename: openeo-user-defined-processes-api-openapi.yml
  format: yaml
  label: openEO User-Defined Processes API
  slug: openeo-user-defined-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-user-defined-processes-api-openapi.yml
- filename: openeo-workspaces-api-openapi.yml
  format: yaml
  label: openEO Workspaces API
  slug: openeo-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/openapi/openeo-workspaces-api-openapi.yml
consequence_counts:
  physical: 3
  read: 31
  safety-critical: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Openeo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /jobs/{job_id}/results
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{order_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orders/{order_id}
operation_count: 51
overview: 'openEO exposes 51 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read, 16 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: openEO
provider_slug: openeo
slug: openeo-agentic-access
source_filename: openeo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/openeo-commercial-data-openapi.yml, openapi/openeo-openapi.yml, openapi/openeo-processing-parameters-openapi.yml,\n  openapi/openeo-workspaces-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 51\n  by_action_class:\n    connected: 31\n    acting: 20\n  by_consequence:\n    read: 31\n    physical: 3\n    write: 16\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /orders\n  method: get\n  operationId: list-orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: create-order\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}\n  method: get\n  operationId: describe-order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}\n  method: post\n  operationId: confirm-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}\n  method: delete\n  operationId: delete-order\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: capabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/openeo\n  method: get\n  operationId: connect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /file_formats\n  method: get\n  operationId: list-file-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conformance\n  method: get\n  operationId: conformance\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections\n  method: get\n  operationId: list-collections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}\n  method: get\n  operationId: describe-collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection_id}/queryables\n  method: get\n  operationId: list-collection-queryables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /processes\n  method: get\n  operationId: list-processes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /udf_runtimes\n  method: get\n  operationId: list-udf-runtimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credentials/oidc\n  method: get\n  operationId: authenticate-oidc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /credentials/basic\n  method: get\n  operationId: authenticate-basic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /validation\n  method: post\n  operationId: validate-custom-process\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /result\n  method: post\n  operationId: compute-result\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /process_graphs\n  method: get\n  operationId: list-custom-processes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /process_graphs/{process_graph_id}\n  method: get\n  operationId: describe-custom-process\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /process_graphs/{process_graph_id}\n  method: put\n  operationId: store-custom-process\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /process_graphs/{process_graph_id}\n  method: delete\n  operationId: delete-custom-process\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /service_types\n  method: get\n  operationId: list-service-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n  method: get\n  operationId: list-services\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n  method: post\n  operationId: create-service\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/{service_id}\n  method: patch\n  operationId: update-service\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/{service_id}\n  method: get\n  operationId: describe-service\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{service_id}\n\
  \  method: delete\n  operationId: delete-service\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/{service_id}/logs\n  method: get\n  operationId: debug-service\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs\n  method: get\n  operationId: list-jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs\n  method: post\n  operationId: create-job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{job_id}\n  method: patch\n  operationId: update-job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{job_id}\n  method: get\n  operationId: describe-job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}\n  method: delete\n  operationId: delete-job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /jobs/{job_id}/estimate\n  method: get\n  operationId: estimate-job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}/logs\n  method: get\n  operationId: debug-job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}/results\n  method: get\n  operationId: list-results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{job_id}/results\n  method: post\n  operationId: start-job\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /jobs/{job_id}/results\n  method: delete\n  operationId: stop-job\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /files\n  method: get\n  operationId: list-files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{path}\n  method: get\n  operationId: download-file\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{path}\n  method: put\n  operationId: upload-file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{path}\n  method: delete\n  operationId: delete-file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me\n  method: get\n  operationId: describe-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /processing_parameters\n  method: get\n  operationId: list-processing-parameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace_providers\n  method: get\n  operationId:\
  \ list-workspace-providers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces\n  method: get\n  operationId: list-workspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces\n  method: post\n  operationId: create-workspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace_id}\n  method: get\n  operationId: describe-workspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspace_id}\n\
  \  method: delete\n  operationId: delete-workspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspace_id}\n  method: patch\n  operationId: update-workspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openeo/refs/heads/main/agentic-access/openeo-agentic-access.yml
summary_line: 51 operations · 20 acting · 1 human-in-the-loop
tags:
- Company
- Earth Observation
- Geospatial
- Remote Sensing
- Cloud Processing
- Open Source
- API Specification
- Data Cubes
---
