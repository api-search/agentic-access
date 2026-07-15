---
acting_count: 39
action_class_counts:
  acting: 39
  connected: 14
api_specs:
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Vulnerabilities API
  slug: armosec-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Posture and Compliance API
  slug: armosec-posture-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Clusters and Workloads API
  slug: armosec-clusters-workloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Runtime Incidents API
  slug: armosec-runtime-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Security Risks and Attack Chains API
  slug: armosec-security-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Network and Runtime Policies API
  slug: armosec-network-runtime-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Registry Scanning API
  slug: armosec-registry-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Integrations API
  slug: armosec-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Access Keys API
  slug: armosec-access-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
consequence_counts:
  read: 14
  safety-critical: 3
  write: 36
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Armosec Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /posture/controls
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /posture/controls/sections
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /repositoryPosture/failedControls
operation_count: 53
overview: 'ARMO exposes 53 API operations that an AI agent could call, of which 39 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 36 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ARMO
provider_slug: armosec
slug: armosec-agentic-access
source_filename: armosec-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/armosec-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    acting: 39\n    connected: 14\n  by_consequence:\n    write: 36\n    read: 14\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /vulnerability/scan\n  method: post\n  operationId: issueVulnerabilityScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerability/scanResults/summary\n  method: post\n  operationId: getVulnerabilityScanSummary\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerability/scanResults/details\n  method: post\n  operationId: getVulnerabilityScanDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerability/severity\n  method: post\n  operationId: getVulnerabilitySeverity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /vulnerability/topVulnerabilities\n  method: post\n  operationId: getTopVulnerabilities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerabilities/list\n  method: post\n  operationId: listVulnerabilities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerabilities/components/list\n  method: post\n  operationId: listVulnerabilitiesByComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerabilities/images/list\n  method: post\n  operationId: listVulnerabilitiesByImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerability/exception\n  method: get\n  operationId: listVulnerabilityExceptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vulnerability/exception\n  method: post\n  operationId: createVulnerabilityException\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerability/exception\n  method: put\n  operationId: updateVulnerabilityException\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerability/exception\n  method: delete\n  operationId: deleteVulnerabilityException\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posture/frameworks\n  method: post\n  operationId: getPostureFrameworks\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posture/controls\n  method: post\n  operationId: getPostureControls\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /posture/controls/sections\n  method: post\n  operationId: getPostureControlSections\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /posture/resources\n  method: post\n  operationId: getPostureResources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posture/exception\n  method: get\n  operationId: listPostureExceptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /posture/exception\n  method: post\n  operationId: createPostureException\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posture/exception\n  method: put\n\
  \  operationId: updatePostureException\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posture/exception\n  method: delete\n  operationId: deletePostureException\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repositoryPosture/repositories\n  method: post\n  operationId: getRepositoryPostureRepositories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /repositoryPosture/failedControls\n  method: post\n  operationId: getRepositoryPostureFailedControls\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /clusters/overtime\n  method: post\n  operationId: getClustersOvertime\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workload/list\n  method: post\n  operationId: listWorkloads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /security/risks\n  method: get\n  operationId: listSecurityRisks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/risks/resources\n  method: get\n  operationId: listSecurityRiskResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/risks/severities\n  method: get\n  operationId: getSecurityRiskSeverities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attack/chains\n  method: get\n  operationId: getAttackChains\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runtime/incidents\n  method: get\n  operationId: listRuntimeIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runtime/incidents/severity\n  method: get\n  operationId: getRuntimeIncidentsSeverity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runtime/incidents/{incidentGUID}/alerts\n  method: get\n  operationId: getRuntimeIncidentAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runtime/incidents/{incidentGUID}/explain\n  method: post\n  operationId: explainRuntimeIncident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runtime/incidents/{incidentGUID}/resolve\n  method: post\n  operationId: resolveRuntimeIncident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runtime/incidents/{incidentGUID}/unresolve\n  method: post\n  operationId: unresolveRuntimeIncident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/policies\n  method:\
  \ get\n  operationId: listNetworkPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/policies/generate\n  method: post\n  operationId: generateNetworkPolicies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runtime/seccomp/list\n  method: get\n  operationId: listSeccompProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runtime/seccomp/generate\n  method: post\n  operationId: generateSeccompProfiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runtime/policy/create\n  method: post\n  operationId: createRuntimePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runtime/policy/exception/create\n  method: post\n  operationId: createRuntimePolicyException\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registry/scan\n  method: post\n  operationId: issueRegistryScan\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registry/scan\n  method: put\n  operationId: updateRegistryScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registry/scan\n  method: delete\n  operationId: deleteRegistryScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/jira/config\n  method: get\n  operationId:\
  \ getJiraConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/jira/config\n  method: post\n  operationId: saveJiraConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/jira/issueV2\n  method: post\n  operationId: createJiraIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collaboration/config\n  method: post\n  operationId: createCollaborationConfig\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collaboration/share\n  method: post\n  operationId: shareCollaboration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authentication/accessKeys\n  method: get\n  operationId: listAccessKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authentication/accessKeys\n  method: post\n  operationId: createAccessKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authentication/accessKeys\n  method: put\n  operationId: updateAccessKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authentication/accessKeys/{guid}\n  method: get\n  operationId: getAccessKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authentication/accessKeys/{guid}\n  method: delete\n  operationId: deleteAccessKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/agentic-access/armosec-agentic-access.yml
summary_line: 53 operations · 39 acting · 3 human-in-the-loop
tags:
- Kubernetes Security
- Cloud Native Security
- CNAPP
- DevSecOps
- KSPM
- Vulnerability Management
- Compliance
- Runtime Security
- CADR
- Kubescape
- Container Security
---
