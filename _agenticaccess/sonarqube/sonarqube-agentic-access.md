---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 9
api_specs:
- filename: sonarqube-issues-api-openapi.yml
  format: yaml
  label: SonarQube Issues API
  slug: sonarqube-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-issues-api-openapi.yml
- filename: sonarqube-measures-api-openapi.yml
  format: yaml
  label: SonarQube Measures API
  slug: sonarqube-measures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-measures-api-openapi.yml
- filename: sonarqube-projects-api-openapi.yml
  format: yaml
  label: SonarQube Projects API
  slug: sonarqube-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-projects-api-openapi.yml
- filename: sonarqube-quality-gates-api-openapi.yml
  format: yaml
  label: SonarQube Quality Gates API
  slug: sonarqube-quality-gates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-quality-gates-api-openapi.yml
- filename: sonarqube-rules-api-openapi.yml
  format: yaml
  label: SonarQube Rules API
  slug: sonarqube-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-rules-api-openapi.yml
- filename: sonarqube-system-api-openapi.yml
  format: yaml
  label: SonarQube System API
  slug: sonarqube-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-system-api-openapi.yml
- filename: sonarqube-users-api-openapi.yml
  format: yaml
  label: SonarQube Users API
  slug: sonarqube-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-users-api-openapi.yml
consequence_counts:
  read: 9
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sonarqube Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'SonarQube exposes 11 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SonarQube
provider_slug: sonarqube
slug: sonarqube-agentic-access
source_filename: sonarqube-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/sonarqube-issues-api-openapi.yml, openapi/sonarqube-measures-api-openapi.yml,\n  openapi/sonarqube-projects-api-openapi.yml, openapi/sonarqube-quality-gates-api-openapi.yml,\n  openapi/sonarqube-rules-api-openapi.yml, openapi/sonarqube-system-api-openapi.yml, openapi/sonarqube-users-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 9\n    acting: 2\n  by_consequence:\n    read: 9\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /issues/search\n  method: get\n  operationId: searchIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /measures/component\n  method: get\n  operationId: getComponentMeasures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/search\n  method: get\n  operationId: searchProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/create\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/delete\n  method: post\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /qualitygates/list\n  method: get\n  operationId: listQualityGates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /qualitygates/project_status\n  method: get\n  operationId: getQualityGateStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rules/search\n  method: get\n  operationId: searchRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/status\n  method: get\n  operationId: getSystemStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/health\n  method: get\n  operationId: getSystemHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/search\n  method: get\n  operationId: searchUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/sonarqube/agentic-access/sonarqube-agentic-access.yml
summary_line: 11 operations · 2 acting
tags:
- Code Quality
- Developer Tools
- DevOps
- Security
- Static Analysis
- Code Security
- SAST
---
