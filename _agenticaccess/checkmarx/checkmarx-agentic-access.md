---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 36
api_specs:
- filename: checkmarx-applications-api-openapi.yml
  format: yaml
  label: Checkmarx Applications API
  slug: checkmarx-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-applications-api-openapi.yml
- filename: checkmarx-authentication-api-openapi.yml
  format: yaml
  label: Checkmarx Authentication API
  slug: checkmarx-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-authentication-api-openapi.yml
- filename: checkmarx-configuration-api-openapi.yml
  format: yaml
  label: Checkmarx Configuration API
  slug: checkmarx-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-configuration-api-openapi.yml
- filename: checkmarx-engines-api-openapi.yml
  format: yaml
  label: Checkmarx Engines API
  slug: checkmarx-engines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-engines-api-openapi.yml
- filename: checkmarx-groups-api-openapi.yml
  format: yaml
  label: Checkmarx Groups API
  slug: checkmarx-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-groups-api-openapi.yml
- filename: checkmarx-packages-api-openapi.yml
  format: yaml
  label: Checkmarx Packages API
  slug: checkmarx-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-packages-api-openapi.yml
- filename: checkmarx-presets-api-openapi.yml
  format: yaml
  label: Checkmarx Presets API
  slug: checkmarx-presets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-presets-api-openapi.yml
- filename: checkmarx-projects-api-openapi.yml
  format: yaml
  label: Checkmarx Projects API
  slug: checkmarx-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-projects-api-openapi.yml
- filename: checkmarx-queries-api-openapi.yml
  format: yaml
  label: Checkmarx Queries API
  slug: checkmarx-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-queries-api-openapi.yml
- filename: checkmarx-reports-api-openapi.yml
  format: yaml
  label: Checkmarx Reports API
  slug: checkmarx-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-reports-api-openapi.yml
- filename: checkmarx-results-api-openapi.yml
  format: yaml
  label: Checkmarx Results API
  slug: checkmarx-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-results-api-openapi.yml
- filename: checkmarx-risk-reports-api-openapi.yml
  format: yaml
  label: Checkmarx Risk Reports API
  slug: checkmarx-risk-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-risk-reports-api-openapi.yml
- filename: checkmarx-scans-api-openapi.yml
  format: yaml
  label: Checkmarx Scans API
  slug: checkmarx-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-scans-api-openapi.yml
- filename: checkmarx-settings-api-openapi.yml
  format: yaml
  label: Checkmarx Settings API
  slug: checkmarx-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-settings-api-openapi.yml
- filename: checkmarx-teams-api-openapi.yml
  format: yaml
  label: Checkmarx Teams API
  slug: checkmarx-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-teams-api-openapi.yml
consequence_counts:
  read: 36
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Checkmarx Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 61
overview: 'Checkmarx exposes 61 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 read and 25 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Checkmarx
provider_slug: checkmarx
slug: checkmarx-agentic-access
source_filename: checkmarx-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/checkmarx-one-openapi.yml, openapi/checkmarx-sast-openapi.yml, openapi/checkmarx-sca-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 61\n  by_action_class:\n    acting: 25\n    connected: 36\n  by_consequence:\n    write: 25\n    read: 36\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/realms/{realm}/protocol/openid-connect/token\n  method: post\n  operationId: authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications\n\
  \  method: get\n  operationId: listApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}\n  method: put\n  operationId: updateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}\n  method: delete\n  operationId: deleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}\n  method: put\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scans\n\
  \  method: get\n  operationId: listScans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans\n  method: post\n  operationId: createScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scans/{scanId}\n  method: get\n  operationId: getScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scans/{scanId}\n  method: delete\n  operationId: cancelScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /results\n  method: get\n  operationId: listResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results/{resultId}\n  method: get\n  operationId: getResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results/{resultId}\n  method: patch\n  operationId: updateResult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /results/summary\n  method: get\n  operationId: getResultsSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries\n  method: get\n  operationId: listQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /presets\n  method: get\n  operationId: listPresets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /presets/{presetId}\n  method: get\n  operationId: getPreset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/project\n  method: get\n  operationId: getProjectConfiguration\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /configuration/project\n  method: patch\n  operationId: updateProjectConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/identity/connect/token\n  method: post\n  operationId: authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}\n  method: put\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}\n\
  \  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/sourceCode/remoteSettings/git\n  method: get\n  operationId: getProjectGitSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/sourceCode/remoteSettings/git\n  method: post\n  operationId: setProjectGitSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sast/scans\n\
  \  method: get\n  operationId: listScans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sast/scans\n  method: post\n  operationId: createScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sast/scans/{scanId}\n  method: get\n  operationId: getScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sast/scans/{scanId}\n  method: patch\n  operationId: updateScanStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sast/scans/{scanId}/resultsStatistics\n  method: get\n  operationId: getScanResultsStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/sastScan\n  method: post\n  operationId: createReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/sastScan/{reportId}\n  method: get\n  operationId: getReportById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/sastScan/{reportId}/status\n  method: get\n  operationId: getReportStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sast/engineServers\n  method: get\n  operationId: listEngineServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sast/presets\n  method: get\n  operationId: listPresets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sast/presets/{presetId}\n  method: get\n  operationId: getPreset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /identity/connect/token\n  method: post\n  operationId: authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk-management/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /risk-management/projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk-management/projects/{projectId}\n  method:\
  \ get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /risk-management/projects/{projectId}\n  method: put\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk-management/projects/{projectId}\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk-management/scans\n  method: get\n  operationId: listScans\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /risk-management/scans\n  method: post\n  operationId: createScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk-management/scans/{scanId}\n  method: get\n  operationId: getScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /risk-management/risk-reports/{projectId}\n  method: get\n  operationId: getRiskReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /risk-management/risk-reports/{projectId}/vulnerabilities\n\
  \  method: get\n  operationId: listProjectVulnerabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /risk-management/risk-reports/{projectId}/packages\n  method: get\n  operationId: listProjectPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /risk-management/risk-reports/{projectId}/licenses\n  method: get\n  operationId: listProjectLicenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages/{packageType}/{packageName}/{version}\n  method: get\n  operationId: getPackageDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/projects/{projectId}\n\
  \  method: get\n  operationId: getProjectSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings/projects/{projectId}\n  method: put\n  operationId: updateProjectSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/agentic-access/checkmarx-agentic-access.yml
summary_line: 61 operations · 25 acting
tags:
- Application Security
- Code Analysis
- DevSecOps
- SAST
- Security Testing
- Vulnerability Scanning
---
