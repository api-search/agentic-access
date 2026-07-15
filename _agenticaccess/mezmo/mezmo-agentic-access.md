---
acting_count: 37
action_class_counts:
  acting: 37
  connected: 25
api_specs:
- filename: mezmo-log-ingestion-api-openapi.yml
  format: yaml
  label: Mezmo Log Ingestion API
  slug: mezmo-log-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-log-ingestion-api-openapi.yml
- filename: mezmo-log-export-api-openapi.yml
  format: yaml
  label: Mezmo Log Export API
  slug: mezmo-log-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-log-export-api-openapi.yml
- filename: mezmo-views-api-openapi.yml
  format: yaml
  label: Mezmo Views API
  slug: mezmo-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-views-api-openapi.yml
- filename: mezmo-alerts-api-openapi.yml
  format: yaml
  label: Mezmo Alerts API
  slug: mezmo-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-alerts-api-openapi.yml
- filename: mezmo-archiving-api-openapi.yml
  format: yaml
  label: Mezmo Archiving API
  slug: mezmo-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-archiving-api-openapi.yml
- filename: mezmo-ingestion-control-api-openapi.yml
  format: yaml
  label: Mezmo Ingestion Control API
  slug: mezmo-ingestion-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-ingestion-control-api-openapi.yml
- filename: mezmo-usage-api-openapi.yml
  format: yaml
  label: Mezmo Usage API
  slug: mezmo-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-usage-api-openapi.yml
- filename: mezmo-pipeline-api-openapi.yml
  format: yaml
  label: Mezmo Pipeline API
  slug: mezmo-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-pipeline-api-openapi.yml
- filename: mezmo-pipeline-classification-api-openapi.yml
  format: yaml
  label: Mezmo Pipeline Classification API
  slug: mezmo-pipeline-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-pipeline-classification-api-openapi.yml
- filename: mezmo-edge-api-openapi.yml
  format: yaml
  label: Mezmo Edge API
  slug: mezmo-edge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/openapi/mezmo-edge-api-openapi.yml
consequence_counts:
  physical: 3
  read: 25
  safety-critical: 3
  write: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Mezmo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/config/presetalert
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/config/presetalert/{presetid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/config/presetalert/{presetid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /edge/clients/{clientId}/heartbeat
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pipelines/{pipelineId}/publish
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pipelines/{pipelineId}/revert
operation_count: 62
overview: 'Mezmo exposes 62 API operations that an AI agent could call, of which 37 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 31 write, 3 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mezmo
provider_slug: mezmo
slug: mezmo-agentic-access
source_filename: mezmo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mezmo-alerts-api-openapi.yml, openapi/mezmo-archiving-api-openapi.yml, openapi/mezmo-edge-api-openapi.yml,\n  openapi/mezmo-ingestion-control-api-openapi.yml, openapi/mezmo-log-export-api-openapi.yml,\n  openapi/mezmo-log-ingestion-api-openapi.yml, openapi/mezmo-pipeline-api-openapi.yml, openapi/mezmo-pipeline-classification-api-openapi.yml,\n  openapi/mezmo-usage-api-openapi.yml, openapi/mezmo-views-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 62\n  by_action_class:\n    connected: 25\n    acting: 37\n  by_consequence:\n    read: 25\n    safety-critical: 3\n    write: 31\n    physical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/config/presetalert\n\
  \  method: get\n  operationId: listPresetAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/presetalert\n  method: post\n  operationId: createPresetAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/config/presetalert/{presetid}\n  method: get\n  operationId: getPresetAlert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/presetalert/{presetid}\n  method: put\n  operationId: updatePresetAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/config/presetalert/{presetid}\n  method: delete\n  operationId: deletePresetAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/config/archiving\n  method: get\n  operationId: getArchiveConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/archiving\n  method: post\n  operationId: createArchiveConfig\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config/archiving\n  method: put\n  operationId: updateArchiveConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config/archiving\n  method: delete\n  operationId: deleteArchiveConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edge/clients\n  method: get\n  operationId:\
  \ listEdgeClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edge/clients\n  method: post\n  operationId: registerEdgeClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edge/clients/{clientId}\n  method: get\n  operationId: getEdgeClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edge/clients/{clientId}\n  method: delete\n  operationId: deregisterEdgeClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edge/clients/{clientId}/heartbeat\n  method: post\n  operationId: sendHeartbeat\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /edge/clients/{clientId}/tasks\n  method: get\n  operationId: listEdgeTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edge/clients/{clientId}/tasks/{taskId}/result\n  method: post\n  operationId: submitTaskResult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config/ingestion/exclusions\n  method: get\n  operationId: listExclusions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/ingestion/exclusions\n  method: post\n  operationId: createExclusion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config/ingestion/exclusions/{ruleid}\n  method: patch\n  operationId: updateExclusion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config/ingestion/exclusions/{ruleid}\n  method: delete\n  operationId: deleteExclusion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config/ingestion/status\n  method: get\n  operationId: getIngestionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/ingestion/suspend\n  method: post\n  operationId: suspendIngestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config/ingestion/suspend/confirm\n  method: post\n  operationId: confirmSuspendIngestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config/ingestion/resume\n  method: post\n  operationId: resumeIngestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/export\n  method: get\n  operationId: exportLogsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/export\n  method: get\n  operationId: exportLogsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logs/ingest\n  method: post\n  operationId: ingestLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines\n  method: get\n  operationId: listPipelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines\n  method: post\n  operationId: createPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}\n  method: get\n  operationId: getPipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{pipelineId}\n  method: put\n  operationId: updatePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}\n  method: delete\n  operationId: deletePipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}/publish\n  method: post\n  operationId: publishPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}/revert\n  method: post\n  operationId: revertPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}/sources\n  method: get\n  operationId: listSources\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{pipelineId}/sources\n  method: post\n  operationId: createSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}/sources/{nodeId}\n  method: get\n  operationId: getSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{pipelineId}/sources/{nodeId}\n  method: put\n  operationId: updateSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}/sources/{nodeId}\n  method: delete\n  operationId: deleteSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}/processors\n  method: get\n  operationId: listProcessors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{pipelineId}/processors\n  method: post\n  operationId: createProcessor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}/processors/{nodeId}\n  method: get\n  operationId: getProcessor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{pipelineId}/processors/{nodeId}\n  method: put\n  operationId: updateProcessor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}/processors/{nodeId}\n  method: delete\n  operationId: deleteProcessor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}/destinations\n  method: get\n  operationId: listDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{pipelineId}/destinations\n  method: post\n  operationId: createDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}/destinations/{nodeId}\n  method: get\n  operationId: getDestination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{pipelineId}/destinations/{nodeId}\n  method: put\n\
  \  operationId: updateDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}/destinations/{nodeId}\n  method: delete\n  operationId: deleteDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pipelines/{pipelineId}/audit\n  method: get\n  operationId: listAuditEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pipelines/{pipelineId}/health\n  method: get\n  operationId: getPipelineHealth\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/events\n  method: get\n  operationId: getEventMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classification/profile\n  method: post\n  operationId: profileSample\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /classification/parse\n  method: post\n  operationId: suggestParser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /classification/regex\n  method: post\n  operationId: generateRegex\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage/{type}\n  method: get\n  operationId: getUsageByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/usage\n  method: get\n  operationId: getUsageDetailed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/view\n  method: get\n  operationId: listViews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/view\n  method: post\n  operationId: createView\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config/view/{viewid}\n  method: get\n  operationId: getView\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/config/view/{viewid}\n  method: put\n  operationId: updateView\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/config/view/{viewid}\n\
  \  method: delete\n  operationId: deleteView\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/agentic-access/mezmo-agentic-access.yml
summary_line: 62 operations · 37 acting · 3 human-in-the-loop
tags:
- Observability
- Logs
- Telemetry
- Telemetry Pipeline
- Log Management
- AI
- SRE
- OpenTelemetry
- DevOps
---
