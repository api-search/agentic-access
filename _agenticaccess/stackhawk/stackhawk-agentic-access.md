---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 29
api_specs:
- filename: stackhawk-api-authentication-api-openapi.yml
  format: yaml
  label: StackHawk Api Authentication API
  slug: stackhawk-api-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-api-authentication-api-openapi.yml
- filename: stackhawk-applications-api-openapi.yml
  format: yaml
  label: StackHawk Applications API
  slug: stackhawk-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-applications-api-openapi.yml
- filename: stackhawk-global-configuration-api-openapi.yml
  format: yaml
  label: StackHawk Global Configuration API
  slug: stackhawk-global-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-global-configuration-api-openapi.yml
- filename: stackhawk-hosted-oas-api-openapi.yml
  format: yaml
  label: StackHawk Hosted OAS API
  slug: stackhawk-hosted-oas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-hosted-oas-api-openapi.yml
- filename: stackhawk-organization-teams-api-openapi.yml
  format: yaml
  label: StackHawk Organization Teams API
  slug: stackhawk-organization-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-organization-teams-api-openapi.yml
- filename: stackhawk-organizations-api-openapi.yml
  format: yaml
  label: StackHawk Organizations API
  slug: stackhawk-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-organizations-api-openapi.yml
- filename: stackhawk-perch-api-openapi.yml
  format: yaml
  label: StackHawk Perch API
  slug: stackhawk-perch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-perch-api-openapi.yml
- filename: stackhawk-profile-scans-api-openapi.yml
  format: yaml
  label: StackHawk Profile Scans API
  slug: stackhawk-profile-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-profile-scans-api-openapi.yml
- filename: stackhawk-reports-api-openapi.yml
  format: yaml
  label: StackHawk Reports API
  slug: stackhawk-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-reports-api-openapi.yml
- filename: stackhawk-repositories-api-openapi.yml
  format: yaml
  label: StackHawk Repositories API
  slug: stackhawk-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-repositories-api-openapi.yml
- filename: stackhawk-scan-configuration-api-openapi.yml
  format: yaml
  label: StackHawk Scan Configuration API
  slug: stackhawk-scan-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-scan-configuration-api-openapi.yml
- filename: stackhawk-scan-policies-api-openapi.yml
  format: yaml
  label: StackHawk Scan Policies API
  slug: stackhawk-scan-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-scan-policies-api-openapi.yml
- filename: stackhawk-scan-results-api-openapi.yml
  format: yaml
  label: StackHawk Scan Results API
  slug: stackhawk-scan-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-scan-results-api-openapi.yml
- filename: stackhawk-user-api-openapi.yml
  format: yaml
  label: StackHawk User API
  slug: stackhawk-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-user-api-openapi.yml
consequence_counts:
  read: 29
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Stackhawk Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 54
overview: 'StackHawk exposes 54 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read and 25 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: StackHawk
provider_slug: stackhawk
slug: stackhawk-agentic-access
source_filename: stackhawk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/stackhawk-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    connected: 29\n    acting: 25\n  by_consequence:\n    read: 29\n    write: 25\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/auth/login\n  method: get\n  operationId: login\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auth/refresh-token\n  method: get\n  operationId: refreshToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user\n  method:\
  \ get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/user\n  method: post\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/org/{orgId}/app\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/{orgId}/list\n  method: get\n  operationId: listApplications\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/org/{orgId}/apps\n  method: get\n  operationId: listApplicationsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/{appId}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/{appId}\n  method: post\n  operationId: updateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/{appId}\n  method: delete\n  operationId: deleteApplication\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/{appId}/env\n  method: post\n  operationId: createEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/{appId}/env/list\n  method: get\n  operationId: listEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/org/{orgId}/envs\n  method: get\n  operationId: listEnvironmentsV2\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/{appId}/env/{envId}\n  method: post\n  operationId: updateEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/{appId}/env/{envId}\n  method: delete\n  operationId: deleteEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/{appId}/config/{configHash}\n  method: get\n  operationId: getApplicationConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/{appId}/scan-config\n  method: get\n  operationId: getScanConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/{appId}/scan-config\n  method: post\n  operationId: updateScanConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/org/{orgId}/scan-config\n  method: get\n  operationId: listOrgScanConfigurations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/org/{orgId}/scan-config\n  method: post\n  operationId: createOrgScanConfiguration\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/{appId}/env/{envId}/scan\n  method: get\n  operationId: listScans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/{appId}/env/{envId}/scan/{scanId}\n  method: get\n  operationId: getScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/{appId}/env/{envId}/scan/{scanId}\n  method: delete\n  operationId: deleteScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/{appId}/env/{envId}/scan/{scanId}/finding\n  method: get\n  operationId: listFindings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/{appId}/env/{envId}/scan/{scanId}/finding/{findingId}\n  method: get\n  operationId: getFinding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/{appId}/env/{envId}/scan/{scanId}/report\n  method: get\n  operationId: getScanReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/{appId}/env/{envId}/scan/{scanId}/report\n  method: post\n  operationId: requestReport\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/app/{appId}/env/{envId}/profile\n  method: get\n  operationId: getProfileScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/app/{appId}/env/{envId}/profile\n  method: post\n  operationId: requestProfileAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/oas/{appId}/upload\n  method: post\n  operationId: uploadOpenAPISpec\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/oas/{appId}/mapping\n  method: get\n  operationId: getOASMapping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/oas/{appId}/mapping\n  method: post\n  operationId: mapOASSpec\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/global-configuration/{configName}\n  method: get\n  operationId: getGlobalConfiguration\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/org/{orgId}/repository\n  method: get\n  operationId: listRepositories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/org/{orgId}/repository\n  method: post\n  operationId: createRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/org/{orgId}/repository/{repoId}\n  method: get\n  operationId: getRepository\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/org/{orgId}/repository/{repoId}\n  method: post\n\
  \  operationId: updateRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/org/{orgId}/repository/{repoId}\n  method: delete\n  operationId: deleteRepository\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/org/{orgId}/team\n  method: post\n  operationId: createTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/org/{orgId}/teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/org/{orgId}/team/{teamId}\n  method: get\n  operationId: getTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/org/{orgId}/team/{teamId}\n  method: put\n  operationId: updateTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/org/{orgId}/team/{teamId}\n  method: delete\n  operationId: deleteTeam\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/org/{orgId}/team/{teamId}/application\n  method: put\n  operationId: updateTeamApplications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/org/{orgId}/user/{userId}/teams\n  method: get\n  operationId: findTeamsForUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/org/{orgId}/members\n  method: get\n  operationId: listMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/org/{orgId}/audit\n  method: get\n  operationId: getAuditHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/org/{orgId}/policy\n  method: get\n  operationId: listScanPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/org/{orgId}/policy\n  method: post\n  operationId: createScanPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/org/{orgId}/policy/{policyId}\n  method: get\n  operationId: getScanPolicy\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/org/{orgId}/policy/{policyId}\n  method: post\n  operationId: updateScanPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/org/{orgId}/policy/{policyId}\n  method: delete\n  operationId: deleteScanPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/perch/scan\n  method: post\n  operationId: requestPerchScan\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/perch/status/{scanId}\n  method: get\n  operationId: getPerchScanStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/agentic-access/stackhawk-agentic-access.yml
summary_line: 54 operations · 25 acting
tags:
- API Security
- Application Security
- DAST
- Security Testing
- Vulnerability Management
---
