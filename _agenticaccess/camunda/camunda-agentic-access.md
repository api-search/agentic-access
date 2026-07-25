---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 4
api_specs:
- filename: camunda-cluster-api-openapi.yml
  format: yaml
  label: Camunda Cluster API
  slug: camunda-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-cluster-api-openapi.yml
- filename: camunda-decisions-api-openapi.yml
  format: yaml
  label: Camunda Decisions API
  slug: camunda-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-decisions-api-openapi.yml
- filename: camunda-deployments-api-openapi.yml
  format: yaml
  label: Camunda Deployments API
  slug: camunda-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-deployments-api-openapi.yml
- filename: camunda-incidents-api-openapi.yml
  format: yaml
  label: Camunda Incidents API
  slug: camunda-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-incidents-api-openapi.yml
- filename: camunda-jobs-api-openapi.yml
  format: yaml
  label: Camunda Jobs API
  slug: camunda-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-jobs-api-openapi.yml
- filename: camunda-messages-api-openapi.yml
  format: yaml
  label: Camunda Messages API
  slug: camunda-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-messages-api-openapi.yml
- filename: camunda-process-definitions-api-openapi.yml
  format: yaml
  label: Camunda Process Definitions API
  slug: camunda-process-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-process-definitions-api-openapi.yml
- filename: camunda-process-instances-api-openapi.yml
  format: yaml
  label: Camunda Process Instances API
  slug: camunda-process-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-process-instances-api-openapi.yml
- filename: camunda-signals-api-openapi.yml
  format: yaml
  label: Camunda Signals API
  slug: camunda-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-signals-api-openapi.yml
- filename: camunda-user-tasks-api-openapi.yml
  format: yaml
  label: Camunda User Tasks API
  slug: camunda-user-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/openapi/camunda-user-tasks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 4
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Camunda Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deployments/search
operation_count: 23
overview: 'Camunda exposes 23 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 17 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Camunda
provider_slug: camunda
slug: camunda-agentic-access
source_filename: camunda-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/camunda-8-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 4\n    acting: 19\n  by_consequence:\n    read: 4\n    write: 17\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /topology\n  method: get\n  operationId: getTopology\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /process-definitions/search\n  method: post\n  operationId: searchProcessDefinitions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /process-definitions/{processDefinitionKey}\n  method: get\n  operationId: getProcessDefinition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /process-definitions/{processDefinitionKey}/xml\n  method: get\n  operationId: getProcessDefinitionXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /process-instances\n  method: post\n  operationId: createProcessInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /process-instances/search\n\
  \  method: post\n  operationId: searchProcessInstances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /process-instances/{processInstanceKey}\n  method: get\n  operationId: getProcessInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /process-instances/{processInstanceKey}\n  method: delete\n  operationId: cancelProcessInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/activation\n  method: post\n\
  \  operationId: activateJobs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{jobKey}/completion\n  method: post\n  operationId: completeJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{jobKey}/failure\n  method: post\n  operationId: failJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /jobs/{jobKey}/error\n  method: post\n  operationId: throwError\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments\n  method: post\n  operationId: createDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deployments/search\n  method: post\n  operationId: searchDeployments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /decision-definitions/search\n  method: post\n  operationId: searchDecisionDefinitions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /decision-definitions/{decisionKey}/evaluation\n  method: post\n  operationId: evaluateDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user-tasks/search\n  method: post\n  operationId: searchUserTasks\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user-tasks/{userTaskKey}/assignment\n  method: post\n  operationId: assignUserTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user-tasks/{userTaskKey}/completion\n  method: post\n  operationId: completeUserTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /messages/publication\n  method: post\n  operationId: publishMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signals/broadcast\n  method: post\n  operationId: broadcastSignal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /incidents/search\n  method: post\n  operationId: searchIncidents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /incidents/{incidentKey}/resolution\n  method: post\n  operationId: resolveIncident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camunda/refs/heads/main/agentic-access/camunda-agentic-access.yml
summary_line: 23 operations · 19 acting
tags:
- BPMN
- Business Process Management
- Process Automation
- Workflow
---
