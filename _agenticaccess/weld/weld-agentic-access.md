---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 32
api_specs:
- filename: weld-connect-openapi.json
  format: json
  label: Weld Connect API
  slug: weld-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-connect-openapi.json
consequence_counts:
  read: 32
  safety-critical: 33
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 33
kind: agentic-access
layout: agentic-access
method: generated
name: Weld Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /connection_bridges
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /connections/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /custom_reports
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /elt_streams/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /elt_streams/{id}/cancel_full_refresh
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /elt_streams/{id}/request_full_refresh
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /elt_streams/{id}/request_run
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /elt_syncs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /elt_syncs/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /elt_syncs/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /elt_syncs/{id}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /elt_syncs/{id}/enable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /elt_syncs/{id}/orchestration
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /elt_syncs/{id}/orchestration
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /elt_syncs/{id}/source_streams
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /orchestrations/{id}/request_run
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reverse_etl_failed_records/retry
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reverse_etl_failed_records/retry_all
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reverse_etl_syncs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reverse_etl_syncs/settings_schema
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reverse_etl_syncs/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /reverse_etl_syncs/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reverse_etl_syncs/{id}/activate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reverse_etl_syncs/{id}/deactivate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /reverse_etl_syncs/{id}/request_run
operation_count: 65
overview: 'Weld exposes 65 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read and 33 safety-critical.


  33 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Weld
provider_slug: weld
slug: weld-agentic-access
source_filename: weld-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/weld-connect-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 65\n  by_action_class:\n    connected: 32\n    acting: 33\n  by_consequence:\n    read: 32\n    safety-critical: 33\n  human_in_the_loop_required: 33\noperations:\n- path: /connection_bridges\n  method: get\n  operationId: ConnectionBridgeOpenApiController_listConnectionBridges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connection_bridges\n  method: post\n  operationId: ConnectionBridgeOpenApiController_createConnectionBridge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /connections/{id}/settings\n  method: get\n  operationId: ConnectionsOpenApiController_getEltSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections\n  method: get\n  operationId: ConnectionsOpenApiController_listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/{id}\n  method: delete\n  operationId: ConnectionsOpenApiController_deleteConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n \
  \     exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /custom_reports\n  method: post\n  operationId: CustomReportsOpenApiController_createCustomReports\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /elt_streams\n  method: get\n  operationId: EltStreamsOpenApiController_getEltStreams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /elt_streams/{id}\n  method: get\n  operationId: EltStreamsOpenApiController_getEltStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /elt_streams/{id}\n  method: delete\n  operationId: EltStreamsOpenApiController_deleteEltStream\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /elt_streams/{id}/request_run\n  method: post\n  operationId: EltStreamsOpenApiController_requestRun\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /elt_streams/{id}/request_full_refresh\n  method: post\n  operationId: EltStreamsOpenApiController_requestFullRefresh\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /elt_streams/{id}/cancel_full_refresh\n  method: post\n  operationId: EltStreamsOpenApiController_cancelFullRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /elt_stream_runs/{id}\n  method: get\n  operationId: EltStreamRunsOpenApiController_getEltStreamRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /elt_stream_runs\n  method: get\n  operationId: EltStreamRunsOpenApiController_getEltStreamRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /elt_syncs/{id}/enable\n  method: post\n  operationId: EltSyncsOpenApiController_enableEltSync\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /elt_syncs/{id}/disable\n  method: post\n  operationId: EltSyncsOpenApiController_disableEltSync\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /elt_syncs\n  method: get\n  operationId: EltSyncsOpenApiController_getEltSyncs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /elt_syncs\n  method: post\n  operationId: EltSyncsOpenApiController_createEltSync\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /elt_syncs/{id}\n  method: post\n  operationId: EltSyncsOpenApiController_updateEltSync\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n  \
  \    purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /elt_syncs/{id}\n  method: get\n  operationId: EltSyncsOpenApiController_getEltSync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /elt_syncs/{id}\n  method: delete\n  operationId: EltSyncsOpenApiController_deleteEltSync\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /elt_syncs/{id}/orchestration\n  method: post\n  operationId: EltSyncsOpenApiController_attachOrchestration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /elt_syncs/{id}/orchestration\n  method: delete\n  operationId: EltSyncsOpenApiController_detachOrchestration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /elt_syncs/{id}/available_source_streams\n  method: get\n  operationId: EltSyncsOpenApiController_getSourceStreams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /elt_syncs/{id}/source_streams\n  method: post\n  operationId: EltSyncsOpenApiController_addSourceStreams\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /elt_syncs/{id}/status\n  method: get\n  operationId: EltSyncsOpenApiController_getEltSyncStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations\n  method: get\n  operationId: IntegrationsOpenApiController_getIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orchestration_runs\n  method: get\n  operationId: OrchestrationRunsOpenApiController_getOrchestrationRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orchestration_runs/{id}\n  method: get\n  operationId: OrchestrationRunsOpenApiController_getOrchestrationRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orchestrations\n  method: get\n  operationId: OrchestrationsOpenApiController_getOrchestrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orchestrations/{id}\n  method: get\n  operationId: OrchestrationsOpenApiController_getOrchestration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orchestrations/{id}/request_run\n  method: post\n  operationId: OrchestrationsOpenApiController_requestRun\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reverse_etl_failed_records\n  method: get\n  operationId: ReverseEtlFailedRecordsOpenApiController_getReverseEtlSyncFailedRecordErrors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse_etl_failed_records/count\n  method: get\n  operationId: ReverseEtlFailedRecordsOpenApiController_getReverseEtlSyncFailedRecordCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse_etl_failed_records/retry\n  method: post\n  operationId: ReverseEtlFailedRecordsOpenApiController_retryReverseEtlSyncFailedRecords\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reverse_etl_failed_records/retry_all\n  method: post\n  operationId: ReverseEtlFailedRecordsOpenApiController_retryAllReverseEtlSyncFailedRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reverse_etl_sync_runs/{id}\n  method: get\n  operationId: ReverseEtlSyncRunsOpenApiController_getReverseEtlSyncRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse_etl_sync_runs\n  method: get\n  operationId: ReverseEtlSyncRunsOpenApiController_getReverseEtlSyncRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse_etl_syncs\n  method: get\n  operationId: ReverseEtlSyncsOpenApiController_getReverseEtlSyncs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse_etl_syncs\n  method: post\n  operationId: ReverseEtlSyncsOpenApiController_createReverseEtlSync\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /reverse_etl_syncs/destination_schema\n  method: get\n  operationId: ReverseEtlSyncsOpenApiController_getReverseEtlDestinationSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse_etl_syncs/available_operations\n  method: get\n  operationId: ReverseEtlSyncsOpenApiController_getReverseEtlAvailableOperations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse_etl_syncs/object_types\n  method: get\n  operationId: ReverseEtlSyncsOpenApiController_getReverseEtlObjectTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse_etl_syncs/settings_schema\n  method: post\n  operationId: ReverseEtlSyncsOpenApiController_getReverseEtlSettingsSchema\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reverse_etl_syncs/{id}\n  method: get\n  operationId: ReverseEtlSyncsOpenApiController_getReverseEtlSync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse_etl_syncs/{id}\n  method: post\n  operationId: ReverseEtlSyncsOpenApiController_updateReverseEtlSync\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reverse_etl_syncs/{id}\n\
  \  method: delete\n  operationId: ReverseEtlSyncsOpenApiController_deleteReverseEtlSync\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reverse_etl_syncs/{id}/activate\n  method: post\n  operationId: ReverseEtlSyncsOpenApiController_activateReverseEtlSync\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reverse_etl_syncs/{id}/deactivate\n  method: post\n  operationId: ReverseEtlSyncsOpenApiController_deactivateReverseEtlSync\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reverse_etl_syncs/{id}/request_run\n  method: post\n  operationId: ReverseEtlSyncsOpenApiController_requestRun\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /transforms\n  method: get\n  operationId: TransformOpenApiController_listTransforms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transforms\n  method:\
  \ post\n  operationId: TransformOpenApiController_createTransform\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /transforms/available_references\n  method: get\n  operationId: TransformOpenApiController_getAvailableReferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transforms/{id}\n  method: get\n  operationId: TransformOpenApiController_getTransform\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transforms/{id}\n  method: patch\n  operationId: TransformOpenApiController_updateTransform\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /transforms/{id}\n  method: delete\n  operationId: TransformOpenApiController_deleteTransform\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /transforms/{id}/schema\n  method: get\n  operationId: TransformOpenApiController_getTransformSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transforms/{id}/orchestration\n\
  \  method: post\n  operationId: TransformOpenApiController_attachOrchestration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /transforms/{id}/orchestration\n  method: delete\n  operationId: TransformOpenApiController_detachOrchestration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /transforms/bulk\n  method: post\n  operationId: TransformOpenApiController_bulkCreateTransforms\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /transforms/{id}/versions\n  method: get\n  operationId: TransformOpenApiController_listVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transforms/{id}/publish\n  method: post\n  operationId: TransformOpenApiController_publishTransform\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /transforms/query_previews\n  method: post\n  operationId: TransformOpenApiController_createQueryPreview\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /transforms/query_previews/{queryExecutionId}/status\n  method: get\n  operationId: TransformOpenApiController_getQueryPreviewStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transforms/query_previews/{queryExecutionId}/result\n  method: get\n  operationId: TransformOpenApiController_getQueryPreviewResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/agentic-access/weld-agentic-access.yml
summary_line: 65 operations · 33 acting · 33 human-in-the-loop
tags:
- Company
- Data
- ETL
- ELT
- Reverse ETL
- Data Pipelines
- Data Integration
- Change Data Capture
- Transformations
- Analytics
- MCP
- AI Agents
---
