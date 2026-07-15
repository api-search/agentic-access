---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 25
api_specs:
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Projects
  slug: dpc-projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Environments
  slug: dpc-environments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Pipeline Executions
  slug: dpc-pipeline-executions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Schedules
  slug: dpc-schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: DPC Agents
  slug: dpc-agents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: ETL Groups & Projects (legacy)
  slug: etl-groups-projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: ETL Jobs & Runs (legacy)
  slug: etl-jobs-runs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: ETL Tasks (legacy)
  slug: etl-tasks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
- filename: matillion-openapi.yml
  format: yaml
  label: ETL Schedules (legacy)
  slug: etl-schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/openapi/matillion-openapi.yml
consequence_counts:
  read: 25
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Matillion Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 44
overview: 'Matillion exposes 44 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Matillion
provider_slug: matillion
slug: matillion-agentic-access
source_filename: matillion-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/matillion-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 25\n    acting: 19\n  by_consequence:\n    read: 25\n    write: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/environments\n  method: get\n  operationId: listEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/environments\n  method: post\n  operationId: createEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/pipeline-executions\n  method: post\n  operationId: createPipelineExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pipeline-executions\n  method: get\n  operationId: listPipelineExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/pipeline-executions/{id}/status\n  method: get\n  operationId: getPipelineExecutionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/pipeline-executions/{id}/steps\n\
  \  method: get\n  operationId: getPipelineExecutionSteps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/pipeline-executions/{id}\n  method: patch\n  operationId: cancelPipelineExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/schedules\n  method: get\n  operationId: listSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/schedules\n  method: post\n  operationId: createSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/schedules/{scheduleId}\n  method: get\n  operationId: getSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/schedules/{scheduleId}\n  method: patch\n  operationId: updateSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/schedules/{scheduleId}\n  method: delete\n  operationId: deleteSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents\n  method: post\n  operationId: createAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agents/{agentId}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agents/{agentId}/credentials\n\
  \  method: get\n  operationId: getAgentCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/group\n  method: get\n  operationId: listEtlGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/group\n  method: post\n  operationId: importEtlGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v1/group/name/{group}\n  method: get\n  operationId: getEtlGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/group/name/{group}/export\n\
  \  method: get\n  operationId: exportEtlGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/group/name/{group}/project\n  method: get\n  operationId: listEtlProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/group/name/{group}/project/name/{project}\n  method: get\n  operationId: getEtlProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/group/name/{group}/project/name/{project}/export\n  method: get\n  operationId: exportEtlProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/group/name/{group}/project/name/{project}/delete\n\
  \  method: post\n  operationId: deleteEtlProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v1/group/name/{group}/project/name/{project}/version/name/{version}\n  method: get\n  operationId: getEtlVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/group/name/{group}/project/name/{project}/version/name/{version}/export\n  method: get\n  operationId: exportEtlVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/group/name/{group}/project/name/{project}/version/name/{version}/orchestration\n  method: get\n  operationId:\
  \ listEtlOrchestrationJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/group/name/{group}/project/name/{project}/version/name/{version}/transformation\n  method: get\n  operationId: listEtlTransformationJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/group/name/{group}/project/name/{project}/version/name/{version}/create\n  method: post\n  operationId: createEtlVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v1/group/name/{group}/project/name/{project}/version/name/{version}/delete\n  method: post\n  operationId:\
  \ deleteEtlVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v1/group/name/{group}/project/name/{project}/version/name/{version}/job/name/{job}/run\n  method: post\n  operationId: runEtlJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v1/group/name/{group}/project/name/{project}/version/name/{version}/job/name/{job}/validate\n  method: post\n  operationId: validateEtlJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v1/task/running\n  method: get\n  operationId: listEtlRunningTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/task/id/{taskId}\n  method: get\n  operationId: getEtlTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/task/id/{taskId}/cancel\n  method: post\n  operationId: cancelEtlTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v1/task/history\n \
  \ method: get\n  operationId: listEtlTaskHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/schedule/name/{schedule}\n  method: get\n  operationId: getEtlSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/schedule/name/{schedule}/export\n  method: get\n  operationId: exportEtlSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/schedule/import\n  method: post\n  operationId: importEtlSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /rest/v1/schedule/name/{schedule}/update\n  method: post\n  operationId: updateEtlSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v1/schedule/name/{schedule}/delete\n  method: post\n  operationId: deleteEtlSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matillion/refs/heads/main/agentic-access/matillion-agentic-access.yml
summary_line: 44 operations · 19 acting
tags:
- Data Integration
- ETL
- ELT
- Data Pipelines
- Cloud Data Warehouse
---
