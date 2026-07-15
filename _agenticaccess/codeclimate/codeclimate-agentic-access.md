---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 11
api_specs:
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Repos API
  slug: repos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Issues API
  slug: issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Test Coverage API
  slug: test-coverage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Snapshots API
  slug: snapshots
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
- filename: codeclimate-openapi.yml
  format: yaml
  label: Code Climate Velocity API
  slug: velocity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/openapi/codeclimate-openapi.yml
consequence_counts:
  read: 11
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Codeclimate Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Code Climate exposes 15 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Code Climate
provider_slug: codeclimate
slug: codeclimate-agentic-access
source_filename: codeclimate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/codeclimate-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 11\n    acting: 4\n  by_consequence:\n    read: 11\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /user\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs\n  method: get\n  operationId: listOrgs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/repos\n  method: get\n  operationId:\
  \ listOrgRepos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/repos\n  method: post\n  operationId: createRepo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/repos/{repo_id}\n  method: put\n  operationId: updateRepo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos\n  method: get\n  operationId: getRepoBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{repo_id}\n  method: get\n  operationId: getRepo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{repo_id}/services\n  method: get\n  operationId: listRepoServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{repo_id}/snapshots/{snapshot_id}\n  method: get\n  operationId: getSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{repo_id}/snapshots/{snapshot_id}/issues\n  method: get\n  operationId: listSnapshotIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /test_reports\n  method: post\n  operationId: createTestReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{repo_id}/test_reports\n  method: get\n  operationId: listTestReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{repo_id}/test_reports/{test_report_id}\n  method: get\n  operationId: getTestReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{repo_id}/test_reports/{test_report_id}/test_file_reports\n  method: get\n  operationId: listTestFileReports\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{repo_id}/test_reports/{test_report_id}/test_file_reports/batch\n  method: post\n  operationId: createTestFileReportsBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codeclimate/refs/heads/main/agentic-access/codeclimate-agentic-access.yml
summary_line: 15 operations · 4 acting
tags:
- Code Quality
- Static Analysis
- Test Coverage
- Engineering Analytics
- DevOps
---
