---
acting_count: 32
action_class_counts:
  acting: 32
  connected: 24
api_specs:
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Test Runs API
  slug: testrail-test-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Test Results API
  slug: testrail-test-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Test Cases API
  slug: testrail-test-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Tests API
  slug: testrail-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Test Plans API
  slug: testrail-test-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Projects API
  slug: testrail-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Test Suites API
  slug: testrail-test-suites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Sections API
  slug: testrail-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Milestones API
  slug: testrail-milestones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Configurations API
  slug: testrail-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
- filename: testrail-openapi.yml
  format: yaml
  label: TestRail Users API
  slug: testrail-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/openapi/testrail-openapi.yml
consequence_counts:
  read: 24
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Testrail Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 56
overview: 'TestRail exposes 56 API operations that an AI agent could call, of which 32 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 32 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TestRail
provider_slug: testrail
slug: testrail-agentic-access
source_filename: testrail-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/testrail-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 56\n  by_action_class:\n    connected: 24\n    acting: 32\n  by_consequence:\n    read: 24\n    write: 32\n  human_in_the_loop_required: 0\noperations:\n- path: /get_projects\n  method: get\n  operationId: getProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_project/{project_id}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /add_project\n  method: post\n\
  \  operationId: addProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update_project/{project_id}\n  method: post\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete_project/{project_id}\n  method: post\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /get_suites/{project_id}\n  method: get\n  operationId: getSuites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_suite/{suite_id}\n  method: get\n  operationId: getSuite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /add_suite/{project_id}\n  method: post\n  operationId: addSuite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update_suite/{suite_id}\n  method: post\n  operationId: updateSuite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete_suite/{suite_id}\n  method: post\n  operationId: deleteSuite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_sections/{project_id}\n  method: get\n  operationId: getSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /add_section/{project_id}\n  method: post\n  operationId: addSection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update_section/{section_id}\n  method: post\n  operationId: updateSection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete_section/{section_id}\n  method: post\n  operationId: deleteSection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_cases/{project_id}\n  method: get\n  operationId: getCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /get_case/{case_id}\n  method: get\n  operationId: getCase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /add_case/{section_id}\n  method: post\n  operationId: addCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update_case/{case_id}\n  method: post\n  operationId: updateCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete_case/{case_id}\n  method: post\n  operationId:\
  \ deleteCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_case_fields\n  method: get\n  operationId: getCaseFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_case_types\n  method: get\n  operationId: getCaseTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_runs/{project_id}\n  method: get\n  operationId: getRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_run/{run_id}\n  method: get\n  operationId: getRun\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /add_run/{project_id}\n  method: post\n  operationId: addRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update_run/{run_id}\n  method: post\n  operationId: updateRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /close_run/{run_id}\n  method: post\n  operationId: closeRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete_run/{run_id}\n  method: post\n  operationId: deleteRun\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_tests/{run_id}\n  method: get\n  operationId: getTests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_test/{test_id}\n  method: get\n  operationId: getTest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_results/{test_id}\n  method:\
  \ get\n  operationId: getResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_results_for_case/{run_id}/{case_id}\n  method: get\n  operationId: getResultsForCase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_results_for_run/{run_id}\n  method: get\n  operationId: getResultsForRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /add_result/{test_id}\n  method: post\n  operationId: addResult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /add_result_for_case/{run_id}/{case_id}\n  method: post\n  operationId: addResultForCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /add_results/{run_id}\n  method: post\n  operationId: addResults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /add_results_for_cases/{run_id}\n  method: post\n  operationId: addResultsForCases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_plans/{project_id}\n  method: get\n  operationId: getPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_plan/{plan_id}\n  method: get\n  operationId: getPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /add_plan/{project_id}\n  method: post\n  operationId: addPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update_plan/{plan_id}\n  method: post\n  operationId: updatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /add_plan_entry/{plan_id}\n  method: post\n  operationId: addPlanEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update_plan_entry/{plan_id}/{entry_id}\n  method: post\n  operationId: updatePlanEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete_plan_entry/{plan_id}/{entry_id}\n  method:\
  \ post\n  operationId: deletePlanEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /close_plan/{plan_id}\n  method: post\n  operationId: closePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete_plan/{plan_id}\n  method: post\n  operationId: deletePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /get_milestones/{project_id}\n  method: get\n  operationId: getMilestones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_milestone/{milestone_id}\n  method: get\n  operationId: getMilestone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /add_milestone/{project_id}\n  method: post\n  operationId: addMilestone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update_milestone/{milestone_id}\n  method: post\n  operationId: updateMilestone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delete_milestone/{milestone_id}\n  method: post\n  operationId: deleteMilestone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_configs/{project_id}\n  method: get\n  operationId: getConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /add_config_group/{project_id}\n  method: post\n  operationId: addConfigGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /add_config/{config_group_id}\n  method: post\n  operationId: addConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get_users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_user/{user_id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get_user_by_email\n  method: get\n  operationId: getUserByEmail\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testrail/refs/heads/main/agentic-access/testrail-agentic-access.yml
summary_line: 56 operations · 32 acting
tags:
- Test Runs
- Test Management
- QA
- Test Cases
- Test Results
- Test Plans
- Testing
- Test Automation
---
