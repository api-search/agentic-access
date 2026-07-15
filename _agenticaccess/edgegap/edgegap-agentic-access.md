---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 15
api_specs:
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Applications API
  slug: edgegap-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap App Versions API
  slug: edgegap-app-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Deployments API
  slug: edgegap-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Sessions API
  slug: edgegap-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Matchmaking API
  slug: edgegap-matchmaking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Relays API
  slug: edgegap-relays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Metrics API
  slug: edgegap-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
- filename: edgegap-openapi.yml
  format: yaml
  label: Edgegap Fleets API
  slug: edgegap-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/openapi/edgegap-openapi.yml
consequence_counts:
  physical: 3
  read: 15
  safety-critical: 3
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Edgegap Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/deployments/bulk-stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/relays/sessions:revoke-user
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/stop/{deployment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/deployments/{deployment_id}/tags
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/private-fleets/deployments
operation_count: 34
overview: 'Edgegap exposes 34 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 13 write, 3 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Edgegap
provider_slug: edgegap
slug: edgegap-agentic-access
source_filename: edgegap-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/edgegap-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 15\n    acting: 19\n  by_consequence:\n    read: 15\n    write: 13\n    physical: 3\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/app\n  method: get\n  operationId: listApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/{app_name}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/{app_name}\n  method: patch\n  operationId: updateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/{app_name}\n  method: delete\n  operationId: deleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/app/{app_name}/versions\n  method: get\n  operationId: listAppVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/{app_name}/version\n  method: post\n  operationId: createAppVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/{app_name}/version/{version_name}\n  method: get\n  operationId: getAppVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/app/{app_name}/version/{version_name}\n  method: patch\n  operationId: updateAppVersion\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/app/{app_name}/version/{version_name}\n  method: delete\n  operationId: deleteAppVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/deployments\n  method: post\n  operationId: createDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/deployments\n  method: get\n  operationId: listDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/status/{deployment_id}\n  method: get\n  operationId: getDeploymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stop/{deployment_id}\n  method: delete\n  operationId: stopDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/deployments/bulk-stop\n  method: post\n  operationId: bulkStopDeployments\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/deployment/{deployment_id}/container-logs\n  method: get\n  operationId: getContainerLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deployments/{deployment_id}/tags\n  method: get\n  operationId: listDeploymentTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deployments/{deployment_id}/tags\n  method: post\n  operationId: addDeploymentTag\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/session\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/session/{session_id}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/session/{session_id}\n  method: delete\n  operationId: deleteSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/session/{session_id}/users\n  method: get\n  operationId: listSessionUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickets\n  method: post\n  operationId: createMatchmakingTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tickets/{ticket_id}\n  method: get\n  operationId: getMatchmakingTicket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickets/{ticket_id}\n  method: delete\n\
  \  operationId: deleteMatchmakingTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/relays/sessions\n  method: get\n  operationId: listRelaySessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/relays/sessions\n  method: post\n  operationId: createRelaySession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/relays/sessions/{session_id}\n  method: get\n  operationId: getRelaySession\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/relays/sessions/{session_id}\n  method: delete\n  operationId: deleteRelaySession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/relays/sessions:authorize-user\n  method: post\n  operationId: authorizeRelayUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/relays/sessions:revoke-user\n  method: post\n  operationId: revokeRelayUser\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/metrics/deployment/{deployment_id}\n  method: get\n  operationId: getDeploymentMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/private-fleets/deployments\n  method: post\n  operationId: createPrivateFleetDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/private-fleets/{fleet_name}/hosts\n  method:\
  \ get\n  operationId: listPrivateFleetHosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edgegap/refs/heads/main/agentic-access/edgegap-agentic-access.yml
summary_line: 34 operations · 19 acting · 3 human-in-the-loop
tags:
- Game Servers
- Orchestration
- Edge Computing
- Matchmaking
- Hosting
---
