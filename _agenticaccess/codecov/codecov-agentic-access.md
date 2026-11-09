---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 34
api_specs:
- filename: codecov-branches-api-openapi.yml
  format: yaml
  label: Codecov Branches API
  slug: codecov-branches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-branches-api-openapi.yml
- filename: codecov-commits-api-openapi.yml
  format: yaml
  label: Codecov Commits API
  slug: codecov-commits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-commits-api-openapi.yml
- filename: codecov-comparison-api-openapi.yml
  format: yaml
  label: Codecov Comparison API
  slug: codecov-comparison-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-comparison-api-openapi.yml
- filename: codecov-components-api-openapi.yml
  format: yaml
  label: Codecov Components API
  slug: codecov-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-components-api-openapi.yml
- filename: codecov-coverage-api-openapi.yml
  format: yaml
  label: Codecov Coverage API
  slug: codecov-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-coverage-api-openapi.yml
- filename: codecov-evaluations-api-openapi.yml
  format: yaml
  label: Codecov Evaluations API
  slug: codecov-evaluations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-evaluations-api-openapi.yml
- filename: codecov-flags-api-openapi.yml
  format: yaml
  label: Codecov Flags API
  slug: codecov-flags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-flags-api-openapi.yml
- filename: codecov-pulls-api-openapi.yml
  format: yaml
  label: Codecov Pulls API
  slug: codecov-pulls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-pulls-api-openapi.yml
- filename: codecov-repos-api-openapi.yml
  format: yaml
  label: Codecov Repos API
  slug: codecov-repos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-repos-api-openapi.yml
- filename: codecov-test-analytics-api-openapi.yml
  format: yaml
  label: Codecov Test Analytics API
  slug: codecov-test-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-test-analytics-api-openapi.yml
- filename: codecov-test-results-api-openapi.yml
  format: yaml
  label: Codecov Test Results API
  slug: codecov-test-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-test-results-api-openapi.yml
- filename: codecov-users-api-openapi.yml
  format: yaml
  label: Codecov Users API
  slug: codecov-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codecov/openapi/codecov-users-api-openapi.yml
consequence_counts:
  read: 34
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Codecov Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 35
overview: 'Codecov exposes 35 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Codecov
provider_slug: codecov
slug: codecov-agentic-access
source_filename: codecov-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/codecov-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 34\n    acting: 1\n  by_consequence:\n    read: 34\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /{service}/\n  method: get\n  operationId: root_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/\n  method: get\n  operationId: root_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/\n\
  \  method: get\n  operationId: repos_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/\n  method: get\n  operationId: repos_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/branches/\n  method: get\n  operationId: repos_branches_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/branches/{name}/\n  method: get\n  operationId: repos_branches_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/commits/\n\
  \  method: get\n  operationId: repos_commits_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/commits/{commitid}/\n  method: get\n  operationId: repos_commits_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/commits/{commitid}/uploads/\n  method: get\n  operationId: repos_commits_uploads_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/compare/\n  method: get\n  operationId: repos_compare_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/compare/components\n  method: get\n  operationId: repos_compare_components_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/compare/file/{file_path}\n  method: get\n  operationId: repos_compare_file_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/compare/flags\n  method: get\n  operationId: repos_compare_flags_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/compare/impacted_files\n  method: get\n  operationId: repos_compare_impacted_files_retrieve\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/compare/segments/{file_path}\n  method: get\n  operationId: repos_compare_segments_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/components/\n  method: get\n  operationId: repos_components_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/config/\n  method: get\n  operationId: repos_config_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/coverage/\n\
  \  method: get\n  operationId: repos_coverage_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/evals/compare/\n  method: get\n  operationId: repos_evals_compare_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/evals/summary/\n  method: get\n  operationId: repos_evals_summary_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/file_report/{path}/\n  method: get\n  operationId: repos_file_report_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/flags/\n  method: get\n  operationId: repos_flags_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/flags/{flag_name}/coverage/\n  method: get\n  operationId: repos_flags_coverage_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/pulls/\n  method: get\n  operationId: repos_pulls_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/pulls/{pullid}/\n  method: get\n  operationId: repos_pulls_retrieve\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/report/\n  method: get\n  operationId: repos_report_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/report/tree\n  method: get\n  operationId: repos_report_tree_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/test-analytics/\n  method: get\n  operationId: repos_test_analytics_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/test-results/\n  method: get\n  operationId:\
  \ repos_test_results_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/test-results/{id}/\n  method: get\n  operationId: repos_test_results_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/repos/{repo_name}/totals/\n  method: get\n  operationId: repos_totals_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/user-sessions/\n  method: get\n  operationId: user_sessions_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/users/\n\
  \  method: get\n  operationId: users_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/users/{user_username_or_ownerid}/\n  method: get\n  operationId: users_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{service}/{owner_username}/users/{user_username_or_ownerid}/\n  method: patch\n  operationId: users_partial_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/codecov/agentic-access/codecov-agentic-access.yml
summary_line: 35 operations · 1 acting
tags:
- Company
- Code Coverage
- CI/CD
- DevOps
- Testing
- Analytics
---
