---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 30
api_specs:
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Scripts API
  slug: windmill-dev-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Flows API
  slug: windmill-dev-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Apps API
  slug: windmill-dev-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Jobs API
  slug: windmill-dev-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Schedules API
  slug: windmill-dev-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Variables API
  slug: windmill-dev-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Resources API
  slug: windmill-dev-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Workspaces API
  slug: windmill-dev-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Users API
  slug: windmill-dev-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Groups API
  slug: windmill-dev-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Folders API
  slug: windmill-dev-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Audit Logs API
  slug: windmill-dev-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Workers API
  slug: windmill-dev-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Triggers API
  slug: windmill-dev-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill OIDC API
  slug: windmill-dev-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
consequence_counts:
  read: 30
  safety-critical: 1
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Windmill Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /w/{workspace}/schedules/setenabled/{path}
operation_count: 49
overview: 'Windmill exposes 49 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 18 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Windmill
provider_slug: windmill-dev
slug: windmill-dev-agentic-access
source_filename: windmill-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/windmill-dev-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    connected: 30\n    acting: 19\n  by_consequence:\n    read: 30\n    write: 18\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/scripts/list\n  method: get\n  operationId: listScripts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/scripts/create\n\
  \  method: post\n  operationId: createScript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/scripts/get/p/{path}\n  method: get\n  operationId: getScriptByPath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/scripts/archive/p/{path}\n  method: post\n  operationId: archiveScriptByPath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/flows/list\n  method: get\n  operationId:\
  \ listFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/flows/create\n  method: post\n  operationId: createFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/flows/get/p/{path}\n  method: get\n  operationId: getFlowByPath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/apps/list\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/apps/get/p/{path}\n\
  \  method: get\n  operationId: getAppByPath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/jobs/run/p/{path}\n  method: post\n  operationId: runScriptByPath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/jobs/run_wait_result/p/{path}\n  method: post\n  operationId: runScriptByPathAndWaitResult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/jobs/run/f/{path}\n  method:\
  \ post\n  operationId: runFlowByPath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/jobs/list\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/jobs_u/get/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/jobs_u/completed/get_result/{id}\n  method: get\n  operationId: getCompletedJobResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /w/{workspace}/jobs_u/queue/cancel/{id}\n  method: post\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/schedules/list\n  method: get\n  operationId: listSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/schedules/create\n  method: post\n  operationId: createSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/schedules/setenabled/{path}\n\
  \  method: post\n  operationId: setScheduleEnabled\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /w/{workspace}/variables/list\n  method: get\n  operationId: listVariables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/variables/create\n  method: post\n  operationId: createVariable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/variables/get/{path}\n\
  \  method: get\n  operationId: getVariable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/variables/delete/{path}\n  method: delete\n  operationId: deleteVariable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/resources/list\n  method: get\n  operationId: listResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/resources/create\n  method: post\n  operationId: createResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/resources/type/list\n  method: get\n  operationId: listResourceTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/list\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/create\n  method: post\n  operationId: createWorkspace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/workspaces/get_settings\n\
  \  method: get\n  operationId: getWorkspaceSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/whoami\n  method: get\n  operationId: globalWhoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/users/whoami\n  method: get\n  operationId: whoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/users/list\n  method: get\n  operationId: listWorkspaceUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/tokens/create\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/groups/list\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/groups/create\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/groups/adduser/{name}\n  method: post\n  operationId: addUserToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/folders/list\n  method: get\n  operationId: listFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/folders/create\n  method: post\n  operationId: createFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/audit/list\n  method: get\n  operationId: listAuditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/audit/get/{id}\n\
  \  method: get\n  operationId: getAuditLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/list\n  method: get\n  operationId: listWorkers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/queue/count\n  method: get\n  operationId: getQueueCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/http_triggers/list\n  method: get\n  operationId: listHttpTriggers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/websocket_triggers/list\n  method: get\n  operationId: listWebsocketTriggers\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/websocket_triggers/create\n  method: post\n  operationId: createWebsocketTrigger\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /w/{workspace}/kafka_triggers/list\n  method: get\n  operationId: listKafkaTriggers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/postgres_triggers/list\n  method: get\n  operationId: listPostgresTriggers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /w/{workspace}/oidc/token\n\
  \  method: post\n  operationId: generateOidcToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/agentic-access/windmill-dev-agentic-access.yml
summary_line: 49 operations · 19 acting · 1 human-in-the-loop
tags:
- Developer Platform
- Workflows
- Internal Tools
- Job Orchestration
- Cron
- Open Source
---
