---
acting_count: 72
action_class_counts:
  acting: 72
  connected: 33
api_specs:
- filename: tray-ai-authentication-api-openapi.yml
  format: yaml
  label: Tray.ai Authentication API
  slug: tray-ai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-authentication-api-openapi.yml
- filename: tray-ai-authentications-api-openapi.yml
  format: yaml
  label: Tray.ai Authentications API
  slug: tray-ai-authentications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-authentications-api-openapi.yml
- filename: tray-ai-call-connector-api-openapi.yml
  format: yaml
  label: Tray.ai Call Connector API
  slug: tray-ai-call-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-call-connector-api-openapi.yml
- filename: tray-ai-connectors-api-openapi.yml
  format: yaml
  label: Tray.ai Connectors API
  slug: tray-ai-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-connectors-api-openapi.yml
- filename: tray-ai-deployments-api-openapi.yml
  format: yaml
  label: Tray.ai Deployments API
  slug: tray-ai-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-deployments-api-openapi.yml
- filename: tray-ai-projects-api-openapi.yml
  format: yaml
  label: Tray.ai Projects API
  slug: tray-ai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-projects-api-openapi.yml
- filename: tray-ai-solution-instances-api-openapi.yml
  format: yaml
  label: Tray.ai Solution Instances API
  slug: tray-ai-solution-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-solution-instances-api-openapi.yml
- filename: tray-ai-solutions-api-openapi.yml
  format: yaml
  label: Tray.ai Solutions API
  slug: tray-ai-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-solutions-api-openapi.yml
- filename: tray-ai-triggers-api-openapi.yml
  format: yaml
  label: Tray.ai Triggers API
  slug: tray-ai-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-triggers-api-openapi.yml
- filename: tray-ai-users-api-openapi.yml
  format: yaml
  label: Tray.ai Users API
  slug: tray-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-users-api-openapi.yml
- filename: tray-ai-workflows-api-openapi.yml
  format: yaml
  label: Tray.ai Workflows API
  slug: tray-ai-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-workflows-api-openapi.yml
- filename: tray-ai-workspaces-api-openapi.yml
  format: yaml
  label: Tray.ai Workspaces API
  slug: tray-ai-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-workspaces-api-openapi.yml
- filename: tray-ai-agent-groups-api-openapi.yml
  format: yaml
  label: Tray.ai Agent Groups API
  slug: tray-ai-agent-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-agent-groups-api-openapi.yml
- filename: tray-ai-agent-instances-api-openapi.yml
  format: yaml
  label: Tray.ai Agent Instances API
  slug: tray-ai-agent-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-agent-instances-api-openapi.yml
- filename: tray-ai-permissions-api-openapi.yml
  format: yaml
  label: Tray.ai Permissions API
  slug: tray-ai-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/openapi/tray-ai-permissions-api-openapi.yml
consequence_counts:
  physical: 2
  read: 33
  safety-critical: 6
  write: 64
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Tray Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /core/v1/projects/{projectId}/imports
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /core/v1/projects/{projectId}/imports/previews
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /core/v1/projects/{projectId}/imports/requirements
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /core/v1/projects/{projectId}/versions/{versionNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /core/v1/solutions/{solutionId}/releases
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /core/v1/solutions/{solutionId}/releases/previews
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cdk/v1/deployments/connectors/{connector-name}/versions/{connector-version}/deploy-connector-from-source
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /connectors/{connectorName}/versions/{connectorVersion}/deploy
operation_count: 105
overview: 'Tray.ai exposes 105 API operations that an AI agent could call, of which 72 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 33 read, 64 write, 2 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tray.ai
provider_slug: tray-ai
slug: tray-ai-agentic-access
source_filename: tray-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/tray-ai-agent-groups-api-openapi.yml, openapi/tray-ai-agent-instances-api-openapi.yml,\n  openapi/tray-ai-authentication-api-openapi.yml, openapi/tray-ai-authentications-api-openapi.yml,\n  openapi/tray-ai-call-connector-api-openapi.yml, openapi/tray-ai-connectors-api-openapi.yml,\n  openapi/tray-ai-deployments-api-openapi.yml, openapi/tray-ai-permissions-api-openapi.yml,\n  openapi/tray-ai-projects-api-openapi.yml, openapi/tray-ai-solution-instances-api-openapi.yml,\n  openapi/tray-ai-solutions-api-openapi.yml, openapi/tray-ai-triggers-api-openapi.yml, openapi/tray-ai-users-api-openapi.yml,\n  openapi/tray-ai-workflows-api-openapi.yml, openapi/tray-ai-workspaces-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\n\
  summary:\n  operations: 105\n  by_action_class:\n    connected: 33\n    acting: 72\n  by_consequence:\n    read: 33\n    write: 64\n    physical: 2\n    safety-critical: 6\n  human_in_the_loop_required: 6\noperations:\n- path: /core/v1/workspaces/{workspace-id}/on-prem-agent-groups\n  method: get\n  operationId: getCoreV1WorkspacesWorkspace-idOn-prem-agent-groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/workspaces/{workspace-id}/on-prem-agent-groups\n  method: post\n  operationId: postCoreV1WorkspacesWorkspace-idOn-prem-agent-groups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/workspaces/{workspace-id}/on-prem-agent-groups/{agent-group-id}\n\
  \  method: delete\n  operationId: deleteCoreV1WorkspacesWorkspace-idOn-prem-agent-groupsAgent-group-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/workspaces/{workspace-id}/on-prem-agent-groups/{agent-group-id}/agents\n  method: get\n  operationId: getCoreV1WorkspacesWorkspace-idOn-prem-agent-groupsAgent-group-idAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/workspaces/{workspace-id}/on-prem-agent-groups/{agent-group-id}/agents\n  method: post\n  operationId: postCoreV1WorkspacesWorkspace-idOn-prem-agent-groupsAgent-group-idAgents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/workspaces/{workspace-id}/on-prem-agent-groups/{agent-group-id}/agents/{agent-id}\n  method: get\n  operationId: getCoreV1WorkspacesWorkspace-idOn-prem-agent-groupsAgent-group-idAgentsAgent-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/workspaces/{workspace-id}/on-prem-agent-groups/{agent-group-id}/agents/{agent-id}\n  method: patch\n  operationId: patchCoreV1WorkspacesWorkspace-idOn-prem-agent-groupsAgent-group-idAgentsAgent-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /core/v1/workspaces/{workspace-id}/on-prem-agent-groups/{agent-group-id}/agents/{agent-id}\n  method: delete\n  operationId: deleteCoreV1WorkspacesWorkspace-idOn-prem-agent-groupsAgent-group-idAgentsAgent-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: get\n  operationId: graphqlPlayground\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graphql#authorize\n  method: post\n  operationId: authorize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql#createUserAuthentication\n  method: post\n  operationId: createUserAuthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql#getAuthentications\n  method: post\n  operationId: getAuthentications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql#deleteAuthentication\n  method: post\n  operationId: deleteAuthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/      '\n  method: post\n  operationId: get-authentications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/       '\n  method: post\n  operationId: create-authentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/        '\n  method: post\n  operationId: delete-authentication\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authentications\n  method: get\n  operationId: listAuthentications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authentications\n  method: post\n  operationId: createAuthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authentications/{authenticationId}\n  method: get\n  operationId: getAuthentication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authentications/{authenticationId}\n  method: delete\n  operationId: deleteAuthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/authentications\n  method: post\n  operationId: create-user-authentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/authentications/{authentication-id}\n  method: get\n  operationId: get-user-authentication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/authentications/{authentication-id}\n  method: put\n  operationId: update-user-authentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/authentications/{authentication-id}\n  method: delete\n  operationId: delete-user-authentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/authentications/{authentication-id}/full\n  method: get\n  operationId: get-full-authentication\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/services/{service-name}/versions/{service-version}/environments\n  method: get\n  operationId: get-service-environments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /graphql#callConnector\n  method: post\n  operationId: callConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/                    '\n  method: post\n  operationId: call-connector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors\n  method: get\n  operationId: listConnectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connectors/{connectorName}/versions/{connectorVersion}\n  method: get\n  operationId: getConnectorVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connectors/{connectorName}/versions/{connectorVersion}/call\n  method: post\n  operationId: callConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/connectors\n  method: get\n\
  \  operationId: get-connectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/connectors/{connector-name}/versions/{connector-version}/operations\n  method: get\n  operationId: get-connector-operations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/connectors/{connector-name}/versions/{connector-version}/call\n  method: post\n  operationId: call-connector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/{connectorName}/versions/{connectorVersion}/deploy\n  method: post\n  operationId: deployConnector\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cdk/v1/deployments/connectors/{connector-name}/versions/{connector-version}/deploy-connector-from-source\n  method: post\n  operationId: create-deployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cdk/v1/deployments/connectors/{connector-name}/versions/{connector-version}/{id}\n  method: get\n  operationId: get-deployment-status\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cdk/v1/permissions/connectors/{connector-name}/versions/{connector-version}/share-with-emails\n  method: post\n  operationId: share-with-emails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/               '\n  method: post\n  operationId: import-project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/                '\n  method: post\n  operationId: export-project\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/                 '\n  method: post\n  operationId: export-project-config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/export\n  method: post\n  operationId: exportProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/import\n  method: post\n  operationId:\
  \ importProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/projects/{projectId}/versions/{versionNumber}\n  method: post\n  operationId: PublicApiProjectController.createProjectVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /core/v1/projects/{projectId}/versions\n  method: get\n  operationId: listProjectVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /core/v1/projects/{projectId}/versions/{versionNumber}/export\n  method: get\n  operationId: exportAProjectVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/projects/{projectId}/imports/requirements\n  method: post\n  operationId: PublicApiProjectController.getProjectImportRequirements\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /core/v1/projects/{projectId}/imports/previews\n  method: post\n  operationId: PublicApiProjectController.previewProjectImport\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /core/v1/projects/{projectId}/imports\n  method: post\n  operationId: PublicApiProjectController.importProject\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /graphql#createSolutionInstance\n  method: post\n  operationId: createSolutionInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql#getSolutionInstances\n\
  \  method: post\n  operationId: getSolutionInstances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql#updateSolutionInstance\n  method: post\n  operationId: updateSolutionInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql#deleteSolutionInstance\n  method: post\n  operationId: deleteSolutionInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/          '\n  method: post\n  operationId: get-solution-instances\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/           '\n  method: post\n  operationId: create-solution-instance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/            '\n  method: post\n  operationId: update-solution-instance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/             '\n  method: post\n  operationId: upgrade-solution-instance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/              '\n  method: post\n  operationId: delete-solution-instance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql#getSolutions\n  method: post\n  operationId: getSolutions\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/         '\n  method: post\n  operationId: get-solutions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/solutions/{solutionId}/releases/previews\n  method: post\n  operationId: PublicApiSolutionController.previewSolutionRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /core/v1/solutions/{solutionId}/releases\n  method: post\n  operationId: PublicApiSolutionController.createSolutionRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /triggers\n  method: get\n  operationId: listTriggers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /subscriptions/{subscriptionId}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/triggers\n  method: get\n  operationId: get-triggers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/triggers/{trigger-name}/versions/{trigger-version}/operations\n  method: get\n  operationId: get-trigger-operations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/subscriptions\n  method: post\n  operationId: create-subscription\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/subscriptions\n  method: get\n  operationId: get-subscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/subscriptions/{subscription-id}\n  method: get\n  operationId: get-subscription-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/subscriptions/{subscription-id}\n  method: delete\n  operationId: delete-connector-events-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql\n  method: post\n  operationId: createExternalUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql#getUsers\n  method: post\n  operationId: getUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql#updateExternalUser\n  method: post\n  operationId: updateExternalUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql#removeUser\n  method: post\n  operationId: removeUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: get-users\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/ '\n  method: post\n  operationId: create-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/  '\n  method: post\n  operationId: create-user-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/   '\n  method: post\n  operationId: create-config-wizard-auth-code\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/    '\n  method: post\n  operationId: update-user\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/     '\n  method: post\n  operationId: delete-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/invite\n  method: post\n  operationId: inviteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/invites\n  method: post\n  operationId: invite-user-to-organization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/roles\n  method: get\n  operationId: list-organization-roles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/users\n  method: get\n  operationId: list-users-in-organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/users\n  method: post\n  operationId: create-user\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/users/{userId}\n  method: get\n  operationId: get-user-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/users/{userId}\n  method: delete\n  operationId: delete-user-by-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/users/{userId}/roles\n  method: put\n  operationId: update-user-organization-role\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql#exportWorkflows\n  method: post\n  operationId: exportWorkflows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /graphql#importWorkflows\n  method: post\n  operationId: importWorkflows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/                  '\n  method: post\n  operationId: import-workflows\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/                   '\n  method: post\n  operationId: export-workflows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces\n  method: get\n  operationId: listWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (34 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/agentic-access/tray-ai-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/agentic-access/tray-ai-agentic-access.yml
summary_line: 105 operations · 72 acting · 6 human-in-the-loop
tags:
- Automation
- Integration
- iPaaS
- AI Agents
- MCP
- Orchestration
- Workflow-Automation
- Connectors
- Agent Gateway
- Embedded Integration
- Enterprise Automation
---
