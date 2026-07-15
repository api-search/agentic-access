---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 18
api_specs:
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Projects API
  slug: flyteadmin-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Workflows API
  slug: flyteadmin-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Tasks API
  slug: flyteadmin-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Launch Plans API
  slug: flyteadmin-launch-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union FlyteAdmin Executions API
  slug: flyteadmin-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
- filename: unionai-openapi.yml
  format: yaml
  label: Union Serverless
  slug: union-serverless
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/openapi/unionai-openapi.yml
consequence_counts:
  read: 18
  safety-critical: 1
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Unionai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/executions/{project}/{domain}/{name}
operation_count: 29
overview: 'Union.ai exposes 29 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 10 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Union.ai
provider_slug: unionai
slug: unionai-agentic-access
source_filename: unionai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/unionai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 18\n    acting: 11\n  by_consequence:\n    read: 18\n    write: 10\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/projects\n  method: post\n  operationId: registerProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - all\n- path: /api/v1/projects/{id}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/projects/{id}\n  method: put\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - all\n- path: /api/v1/domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n\
  \    - all\n- path: /api/v1/tasks\n  method: post\n  operationId: createTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - all\n- path: /api/v1/task_ids/{project}/{domain}\n  method: get\n  operationId: listTaskIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/tasks/{project}/{domain}/{name}\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/tasks/{project}/{domain}/{name}/{version}\n  method: get\n  operationId: getTask\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/workflows\n  method: post\n  operationId: createWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - all\n- path: /api/v1/workflow_ids/{project}/{domain}\n  method: get\n  operationId: listWorkflowIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/workflows/{project}/{domain}/{name}\n  method: get\n  operationId: listWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/workflows/{project}/{domain}/{name}/{version}\n  method: get\n  operationId: getWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/launch_plans\n  method: post\n  operationId: createLaunchPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - all\n- path: /api/v1/launch_plan_ids/{project}/{domain}\n  method: get\n  operationId: listLaunchPlanIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/launch_plans/{project}/{domain}/{name}\n\
  \  method: get\n  operationId: listLaunchPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/launch_plans/{project}/{domain}/{name}/{version}\n  method: get\n  operationId: getLaunchPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/launch_plans/{project}/{domain}/{name}/{version}\n  method: put\n  operationId: updateLaunchPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - all\n- path: /api/v1/active_launch_plans/{project}/{domain}\n  method: get\n  operationId: listActiveLaunchPlans\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/executions\n  method: post\n  operationId: createExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - all\n- path: /api/v1/executions/relaunch\n  method: post\n  operationId: relaunchExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - all\n- path: /api/v1/executions/recover\n  method: post\n  operationId:\
  \ recoverExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - all\n- path: /api/v1/executions/{project}/{domain}\n  method: get\n  operationId: listExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/executions/{project}/{domain}/{name}\n  method: get\n  operationId: getExecution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/executions/{project}/{domain}/{name}\n  method: put\n  operationId: updateExecution\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - all\n- path: /api/v1/executions/{project}/{domain}/{name}\n  method: delete\n  operationId: terminateExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - all\n- path: /api/v1/data/executions/{project}/{domain}/{name}\n  method: get\n  operationId: getExecutionData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/node_executions/{project}/{domain}/{name}\n\
  \  method: get\n  operationId: listNodeExecutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n- path: /api/v1/version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - all\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unionai/refs/heads/main/agentic-access/unionai-agentic-access.yml
summary_line: 29 operations · 11 acting · 1 human-in-the-loop
tags:
- AI
- ML
- Orchestration
- Workflows
- MLOps
- Flyte
- Serverless
---
