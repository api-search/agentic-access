---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 5
api_specs:
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Posture & Compliance API
  slug: kubescape-posture-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Vulnerabilities API
  slug: kubescape-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Runtime Security API
  slug: kubescape-runtime-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Network Policies API
  slug: kubescape-network-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Registry & Repository Scanning API
  slug: kubescape-registry-repository-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Access Keys API
  slug: kubescape-access-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
consequence_counts:
  read: 5
  safety-critical: 4
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Kubescape Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /authentication/accessKeys/{guid}
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
operation_count: 23
overview: 'Kubescape exposes 23 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 14 write, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kubescape
provider_slug: kubescape
slug: kubescape-agentic-access
source_filename: kubescape-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kubescape-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 18\n    connected: 5\n  by_consequence:\n    write: 14\n    safety-critical: 4\n    read: 5\n  human_in_the_loop_required: 4\noperations:\n- path: /posture/frameworks\n  method: post\n  operationId: getPostureFrameworks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /posture/controls\n  method: post\n  operationId: getPostureControls\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /posture/controls/sections\n  method: post\n  operationId: getPostureControlSections\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /posture/resources\n  method: post\n  operationId: getPostureResources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerability/scan\n  method: post\n  operationId: startVulnerabilityScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerability/scanResults/summary\n  method: post\n  operationId: getVulnerabilityScanSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerability/scanResults/details\n  method: post\n  operationId: getVulnerabilityScanDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerability/severity\n  method: post\n  operationId: getVulnerabilitySeverity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vulnerabilities/list\n  method: post\n  operationId: listVulnerabilities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/list\n  method: post\n  operationId: listImages\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /runtimeIncidents\n  method: get\n  operationId: listRuntimeIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runtimeIncidents/{guid}/alerts\n  method: get\n  operationId: getRuntimeIncidentAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runtimeIncidents/{guid}/resolve\n  method: post\n  operationId: resolveRuntimeIncident\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attackChains\n  method: post\n  operationId: getAttackChains\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /securityRisks\n  method: get\n  operationId: getSecurityRisks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networkPolicies\n  method: get\n  operationId: getNetworkPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /networkPolicies/generate\n  method: post\n  operationId: generateNetworkPolicies\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /seccompProfiles/generate\n  method: post\n  operationId: generateSeccompProfiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registry/scan\n  method: post\n  operationId: scheduleRegistryScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repositoryPosture/failedControls\n\
  \  method: post\n  operationId: getRepositoryFailedControls\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /authentication/accessKeys\n  method: get\n  operationId: listAccessKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authentication/accessKeys\n  method: post\n  operationId: createAccessKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authentication/accessKeys/{guid}\n\
  \  method: delete\n  operationId: deleteAccessKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/agentic-access/kubescape-agentic-access.yml
summary_line: 23 operations · 18 acting · 4 human-in-the-loop
tags:
- Kubernetes Security
- Cloud Native Security
- Container Security
- DevSecOps
- Kubernetes
- Vulnerability Scanning
- Compliance
- Runtime Security
- CNCF
- Open Source
---
