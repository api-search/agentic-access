---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 16
api_specs:
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Test Runs API
  slug: testmo-test-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Automation Runs API
  slug: testmo-automation-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Automation Sources API
  slug: testmo-automation-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Sessions API
  slug: testmo-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Projects API
  slug: testmo-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Milestones API
  slug: testmo-milestones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Test Case Management API
  slug: testmo-test-case-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
consequence_counts:
  read: 16
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Testmo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Testmo exposes 23 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Testmo
provider_slug: testmo
slug: testmo-agentic-access
source_filename: testmo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/testmo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 16\n    acting: 7\n  by_consequence:\n    read: 16\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runs/{run_id}\n  method: get\n  operationId:\
  \ getRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/runs\n  method: get\n  operationId: listRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runs/{run_id}/results\n  method: get\n  operationId: listRunResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /automation/runs/{run_id}\n  method: get\n  operationId: getAutomationRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/automation/runs\n  method: get\n  operationId: listAutomationRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /automation/sources/{source_id}\n  method: get\n  operationId: getAutomationSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/automation/sources\n  method: get\n  operationId: listAutomationSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{session_id}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /milestones/{milestone_id}\n  method: get\n  operationId: getMilestone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/milestones\n  method: get\n  operationId: listMilestones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/cases\n  method: get\n  operationId: listCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/cases\n  method: post\n  operationId: createCases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/cases\n  method: patch\n  operationId: updateCases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/cases\n  method: delete\n  operationId: deleteCases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folders\n  method: get\n  operationId: listFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /folders\n\
  \  method: post\n  operationId: createFolders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folders\n  method: patch\n  operationId: updateFolders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /folders\n  method: delete\n  operationId: deleteFolders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /cases/{case_id}/attachments\n  method: get\n  operationId: listCaseAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cases/{case_id}/attachments\n  method: post\n  operationId: uploadCaseAttachments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/agentic-access/testmo-agentic-access.yml
summary_line: 23 operations · 7 acting
tags:
- Test Runs
- Test Management
- Test Automation
- QA
- Exploratory Testing
- CI/CD
- Quality Assurance
---
