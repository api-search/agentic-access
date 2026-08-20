---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 13
api_specs:
- filename: boomi-atoms-api-openapi.yml
  format: yaml
  label: Boomi Atoms API
  slug: boomi-atoms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-atoms-api-openapi.yml
- filename: boomi-components-api-openapi.yml
  format: yaml
  label: Boomi Components API
  slug: boomi-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-components-api-openapi.yml
- filename: boomi-deployments-api-openapi.yml
  format: yaml
  label: Boomi Deployments API
  slug: boomi-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-deployments-api-openapi.yml
- filename: boomi-environments-api-openapi.yml
  format: yaml
  label: Boomi Environments API
  slug: boomi-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-environments-api-openapi.yml
- filename: boomi-execution-api-openapi.yml
  format: yaml
  label: Boomi Execution API
  slug: boomi-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-execution-api-openapi.yml
- filename: boomi-golden-records-api-openapi.yml
  format: yaml
  label: Boomi Golden Records API
  slug: boomi-golden-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-golden-records-api-openapi.yml
- filename: boomi-messages-api-openapi.yml
  format: yaml
  label: Boomi Messages API
  slug: boomi-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-messages-api-openapi.yml
- filename: boomi-models-api-openapi.yml
  format: yaml
  label: Boomi Models API
  slug: boomi-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-models-api-openapi.yml
- filename: boomi-processes-api-openapi.yml
  format: yaml
  label: Boomi Processes API
  slug: boomi-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-processes-api-openapi.yml
- filename: boomi-quarantine-api-openapi.yml
  format: yaml
  label: Boomi Quarantine API
  slug: boomi-quarantine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-quarantine-api-openapi.yml
- filename: boomi-repositories-api-openapi.yml
  format: yaml
  label: Boomi Repositories API
  slug: boomi-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-repositories-api-openapi.yml
- filename: boomi-sources-api-openapi.yml
  format: yaml
  label: Boomi Sources API
  slug: boomi-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/openapi/boomi-sources-api-openapi.yml
consequence_counts:
  physical: 3
  read: 13
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Boomi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /DeployedPackage
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /DeployedPackage/query
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /DeployedPackage/{id}
operation_count: 37
overview: 'Boomi exposes 37 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 21 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Boomi
provider_slug: boomi
slug: boomi-agentic-access
source_filename: boomi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/boomi-datahub-api-openapi.yml, openapi/boomi-event-streams-openapi.yml, openapi/boomi-platform-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 13\n    acting: 24\n  by_consequence:\n    read: 13\n    write: 21\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /repositories\n  method: get\n  operationId: listRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repositories\n  method: post\n  operationId: createRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repositories/{repositoryId}\n  method: get\n  operationId: getRepository\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repositories/{repositoryId}\n  method: delete\n  operationId: deleteRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repositories/{repositoryId}/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /repositories/{repositoryId}/models\n  method: post\n  operationId: createModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repositories/{repositoryId}/models/{modelId}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repositories/{repositoryId}/models/{modelId}\n  method: delete\n  operationId: deleteModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /repositories/{repositoryId}/models/{modelId}/publish\n  method: post\n  operationId: publishModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repositories/{repositoryId}/sources\n  method: get\n  operationId: listSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repositories/{repositoryId}/sources\n  method: post\n  operationId: createSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /repositories/{repositoryId}/universes/{universeId}/records\n  method: get\n  operationId: listGoldenRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repositories/{repositoryId}/universes/{universeId}/quarantine\n  method: get\n  operationId: listQuarantineEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: post\n  operationId: publishMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Process\n  method: post\n  operationId: createProcess\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Process/{id}\n  method: get\n  operationId: getProcess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Process/{id}\n  method: post\n  operationId: updateProcess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Process/{id}\n  method: delete\n  operationId: deleteProcess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Process/query\n  method: post\n  operationId: queryProcesses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ExecutionRequest\n  method: post\n  operationId: executeProcess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ExecutionRecord/query\n  method: post\n  operationId: queryExecutionRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Environment\n  method: post\n  operationId: createEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Environment/{id}\n  method: get\n  operationId: getEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Environment/{id}\n  method: delete\n  operationId: deleteEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Environment/query\n  method: post\n  operationId: queryEnvironments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /DeployedPackage\n  method: post\n  operationId: createDeployedPackage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /DeployedPackage/{id}\n  method: get\n  operationId: getDeployedPackage\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DeployedPackage/{id}\n  method: delete\n  operationId: deleteDeployedPackage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /DeployedPackage/query\n  method: post\n  operationId: queryDeployedPackages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Atom/{id}\n  method: get\n  operationId: getAtom\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Atom/{id}\n  method: post\n  operationId: updateAtom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Atom/{id}\n  method: delete\n  operationId: deleteAtom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Atom/query\n  method: post\n  operationId: queryAtoms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PackagedComponent\n  method: post\n  operationId: createPackagedComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /PackagedComponent/{id}\n  method: get\n  operationId: getPackagedComponent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ProcessSchedules/{id}\n  method: get\n  operationId: getProcessSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ProcessSchedules/{id}\n\
  \  method: post\n  operationId: updateProcessSchedules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boomi/refs/heads/main/agentic-access/boomi-agentic-access.yml
summary_line: 37 operations · 24 acting
tags:
- AI Agents
- Automation
- B2B
- Data Integration
- EDI
- Integration
- Management
- MFT
- Platform
- Workflows
---
