---
acting_count: 510
action_class_counts:
  acting: 510
  connected: 220
api_specs:
- filename: delphix-continuous-data-openapi.yml
  format: yaml
  label: Delphix DCT Continuous Data API
  slug: delphix-dct-continuous-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delphix/refs/heads/main/openapi/delphix-continuous-data-openapi.yml
- filename: delphix-continuous-compliance-openapi.yml
  format: yaml
  label: Delphix DCT Continuous Compliance API
  slug: delphix-dct-continuous-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delphix/refs/heads/main/openapi/delphix-continuous-compliance-openapi.yml
consequence_counts:
  physical: 19
  read: 220
  safety-critical: 15
  write: 476
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 15
kind: agentic-access
layout: agentic-access
method: generated
name: Delphix Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /algorithms/{algorithmId}/mappings/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cdb-dsources/{cdbDSourceId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cdbs/{cdbId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /dsources/{dsourceId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/enable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /paas-instances/{paaSInstanceId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /replication-profiles/{replicationProfileId}/disable-tag-replication
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /staging-cdbs/{stagingCdbId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /vcdbs/{vcdbId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /vcdbs/{vcdbId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /vdb-groups/{vdbGroupId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /vdb-groups/{vdbGroupId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /vdbs/{vdbId}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /vdbs/{vdbId}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paas-databases
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paas-databases/provision_from_bookmark
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paas-databases/{paaSDatabaseId}/de-provision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paas-databases/{paaSDatabaseId}/re-provision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paas-instances
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paas-instances/provision_from_bookmark
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paas-instances/{paaSInstanceId}/de-provision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paas-instances/{paaSInstanceId}/re-provision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /timeflows/{timeflowId}/timeflow_snapshot_ranges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /vdb-groups/provision_from_bookmark
operation_count: 730
overview: 'Delphix exposes 730 API operations that an AI agent could call, of which 510 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 220 read, 476 write, 19 physical, and 15 safety-critical.


  15 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Delphix
provider_slug: delphix
slug: delphix-agentic-access
source_filename: delphix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/delphix-continuous-compliance-openapi.yml, openapi/delphix-continuous-data-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 730\n  by_action_class:\n    acting: 510\n    connected: 220\n  by_consequence:\n    write: 476\n    read: 220\n    safety-critical: 15\n    physical: 19\n  human_in_the_loop_required: 15\noperations:\n- path: /hyperscale-instances\n  method: post\n  operationId: register_hyperscale_instance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /hyperscale-instances\n  method: get\n  operationId: get_hyperscale_instances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-instances/search\n  method: post\n  operationId: search_hyperscale_instances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-instances/{hyperscaleInstanceId}\n  method: get\n  operationId: get_hyperscale_instance_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-instances/{hyperscaleInstanceId}\n  method: patch\n  operationId: update_hyperscale_instance\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-instances/{hyperscaleInstanceId}\n  method: delete\n  operationId: unregister_hyperscale_instance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-instances/{hyperscaleInstanceId}/tags\n  method: post\n  operationId: create_hyperscale_instance_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-instances/{hyperscaleInstanceId}/tags\n  method: get\n  operationId: get_hyperscale_instance_tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-instances/{hyperscaleInstanceId}/tags/delete\n  method: post\n  operationId: delete_hyperscale_instance_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-instances/{hyperscaleInstanceId}/sync-engines\n  method: post\n  operationId: sync_engines_hyperscale_instance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-instances/{hyperscaleInstanceId}/add-engine\n  method: post\n  operationId: add_engine_to_hyperscale_instance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-instances/{hyperscaleInstanceId}/remove-engine\n  method: post\n  operationId: remove_engine_from_hyperscale_instance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-instances/{hyperscaleInstanceId}/move-to-job-orchestrator\n\
  \  method: put\n  operationId: move_compliance_nodes_to_job_orchestrator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-mount-points\n  method: get\n  operationId: get_hyperscale_mount_points\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-mount-points\n  method: post\n  operationId: create_hyperscale_mount_point\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-mount-points/{hyperscaleMountPointId}\n\
  \  method: get\n  operationId: get_hyperscale_mount_point_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-mount-points/{hyperscaleMountPointId}\n  method: patch\n  operationId: update_hyperscale_mount_point_by_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-mount-points/{hyperscaleMountPointId}\n  method: delete\n  operationId: delete_hyperscale_mount_point\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /hyperscale-mount-points/{hyperscaleMountPointId}/validate\n  method: get\n  operationId: validate_hyperscale_mount_point\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-mount-points/search\n  method: post\n  operationId: search_hyperscale_mount_points\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-connectors\n  method: get\n  operationId: get_hyperscale_connectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-connectors\n  method: post\n  operationId: create_hyperscale_connector\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-connectors/{hyperscaleConnectorId}\n  method: get\n  operationId: get_hyperscale_connector_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-connectors/{hyperscaleConnectorId}\n  method: patch\n  operationId: update_hyperscale_connector_by_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-connectors/{hyperscaleConnectorId}\n  method: delete\n  operationId:\
  \ delete_hyperscale_connector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-connectors/{hyperscaleConnectorId}/tags\n  method: post\n  operationId: create_hyperscale_connector_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-connectors/{hyperscaleConnectorId}/tags\n  method: get\n  operationId: get_hyperscale_connector_tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-connectors/{hyperscaleConnectorId}/tags/delete\n\
  \  method: post\n  operationId: delete_hyperscale_connector_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-connectors/search\n  method: post\n  operationId: search_hyperscale_connectors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-datasets\n  method: get\n  operationId: get_hyperscale_datasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-datasets/{hyperscaleDatasetId}\n\
  \  method: get\n  operationId: get_hyperscale_dataset_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-datasets/{hyperscaleDatasetId}\n  method: patch\n  operationId: update_hyperscale_dataset_by_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-datasets/{hyperscaleDatasetId}/tags\n  method: post\n  operationId: create_hyperscale_dataset_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /hyperscale-datasets/{hyperscaleDatasetId}/tags\n  method: get\n  operationId: get_hyperscale_dataset_tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-datasets/{hyperscaleDatasetId}/tags/delete\n  method: post\n  operationId: delete_hyperscale_dataset_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-datasets/{hyperscaleDatasetId}/tables-or-files/{hyperscaleDatasetTableOrFileId}\n  method: get\n  operationId: get_hyperscale_dataset_table_or_file_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-datasets/{hyperscaleDatasetId}/tables-or-files/{hyperscaleDatasetTableOrFileId}\n\
  \  method: patch\n  operationId: update_hyperscale_dataset_table_or_file_by_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-datasets/{hyperscaleDatasetId}/tables-or-files\n  method: get\n  operationId: get_hyperscale_dataset_tables_or_files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hyperscale-datasets/{hyperscaleDatasetId}/tables-or-files/search\n  method: post\n  operationId: search_hyperscale_dataset_tables_or_files\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /hyperscale-datasets/search\n  method: post\n  operationId: search_hyperscale_datasets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/masking-execution-metrics\n  method: get\n  operationId: get_masking_execution_metrics_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/masking-execution-metrics/search\n  method: post\n  operationId: search_masking_execution_metrics_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/{executionId}/generate-pdf-report\n  method: post\n  operationId: generate_execution_pdf_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/{executionId}/download-pdf-report\n  method: get\n  operationId: download_execution_pdf_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/engine-global-object-state-report\n  method: get\n  operationId: get_engine_global_object_state_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /reporting/engine-global-object-state-report/search\n  method: post\n  operationId: search_engine_global_object_state_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reporting/data-risk-report\n  method: get\n  operationId: get_data_risk_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reporting/data-risk-report/search\n  method: post\n  operationId: search_data_risk_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /classifiers\n  method: get\n  operationId: get_classifiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classifiers\n  method: post\n  operationId: create_classifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /classifiers/search\n  method: post\n  operationId: search_classifiers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /classifiers/{classifierId}\n\
  \  method: get\n  operationId: get_classifier_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classifiers/{classifierId}\n  method: patch\n  operationId: update_classifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /classifiers/{classifierId}\n  method: delete\n  operationId: delete_classifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /classifiers/{classifierId}/discovery-policies\n  method: get\n\
  \  operationId: get_classifier_discovery_policies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classifiers/{classifierId}/discovery-policies/search\n  method: post\n  operationId: search_classifier_discovery_policies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /classifiers/{classifierId}/tags\n  method: get\n  operationId: get_classifier_tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classifiers/{classifierId}/tags\n  method: post\n  operationId: create_classifier_tags\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /classifiers/{classifierId}/tags/delete\n  method: post\n  operationId: delete_classifier_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors\n  method: get\n  operationId: get_connectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connectors\n  method: post\n  operationId: create_connector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/test\n  method: post\n  operationId: test_unsaved_connector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/{connectorId}\n  method: get\n  operationId: get_connector_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connectors/{connectorId}\n  method: patch\n  operationId: update_connector_by_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/{connectorId}\n  method: delete\n  operationId: delete_connector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/{connectorId}/driver-support-tasks\n  method: get\n  operationId: get_connector_driver_support_tasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connectors/{connectorId}/test\n  method: post\n  operationId: test_connector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/{connectorId}/properties\n  method: get\n  operationId: get_connection_properties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connectors/{connectorId}/fetch-table-names\n  method: post\n  operationId: fetch_table_names\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/{connectorId}/masking-jobs/search\n  method: post\n  operationId: search_connector_jobs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/{connectorId}/tags\n  method: post\n  operationId: create_connector_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/{connectorId}/tags\n  method: get\n  operationId: get_connector_tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connectors/{connectorId}/tags/delete\n  method: post\n  operationId: delete_connector_tag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/search\n  method: post\n  operationId: search_connectors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-classes\n  method: get\n  operationId: get_data_classes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-classes\n  method: post\n  operationId: create_data_class\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /data-classes/search\n  method: post\n  operationId: search_data_classes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-classes/{dataClassId}\n  method: get\n  operationId: get_data_class_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-classes/{dataClassId}\n  method: patch\n  operationId: update_data_class\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-classes/{dataClassId}\n  method:\
  \ delete\n  operationId: delete_data_class\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-classes/{dataClassId}/algorithms\n  method: get\n  operationId: get_data_class_algorithms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-classes/{dataClassId}/algorithms\n  method: post\n  operationId: add_data_class_algorithms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-classes/{dataClassId}/algorithms/remove\n\
  \  method: post\n  operationId: remove_data_class_algorithms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-classes/{dataClassId}/algorithms/search\n  method: post\n  operationId: search_data_class_algorithms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-classes/{dataClassId}/tags\n  method: get\n  operationId: get_data_class_tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-classes/{dataClassId}/tags\n\
  \  method: post\n  operationId: create_data_class_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-classes/{dataClassId}/tags/delete\n  method: post\n  operationId: delete_data_class_tags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovery-policies\n  method: get\n  operationId: get_discovery_policies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery-policies\n  method: post\n  operationId:\
  \ create_discovery_policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovery-policies/search\n  method: post\n  operationId: search_discovery_policies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovery-policies/{discoveryPolicyId}\n  method: get\n  operationId: get_discovery_policy_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery-policies/{discoveryPolicyId}\n  method: delete\n  operationId:\
  \ delete_discovery_policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovery-policies/{discoveryPolicyId}\n  method: patch\n  operationId: update_discovery_policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovery-policies/{discoveryPolicyId}/classifiers\n  method: get\n  operationId: get_discovery_policy_classifiers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery-policies/{discoveryPolicyId}/classifiers\n\
  \  method: post\n  operationId: add_discovery_policy_classifiers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovery-policies/{discoveryPolicyId}/classifiers/remove\n  method: post\n  operationId: remove_discovery_policy_classifiers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovery-policies/{discoveryPolicyId}/classifiers/search\n  method: post\n  operationId: search_discovery_policy_classifiers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discovery-policies/{discoveryPolicyId}/expressions\n  method: get\n  operationId: get_discovery_policy_expressions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery-policies/{discoveryPolicyId}/expressions/search\n  method: post\n  operationId: search_discovery_policy_expressions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit\n\n# --- truncated at 32 KB (232 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/delphix/refs/heads/main/agentic-access/delphix-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delphix/refs/heads/main/agentic-access/delphix-agentic-access.yml
summary_line: 730 operations · 510 acting · 15 human-in-the-loop
tags:
- Company
- Data Management
- Test Data Management
- Data Virtualization
- Data Masking
- Data Compliance
- Database
- DevOps
- Synthetic Data
- Data Control Tower
---
