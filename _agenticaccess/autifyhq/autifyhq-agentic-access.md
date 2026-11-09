---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 8
api_specs:
- filename: autifyhq-autify-cli-api-openapi.yml
  format: yaml
  label: Autifyhq Autify Cli API
  slug: autifyhq-autify-cli-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autifyhq/openapi/autifyhq-autify-cli-api-openapi.yml
- filename: autifyhq-default-api-openapi.yml
  format: yaml
  label: Autifyhq ~ API
  slug: autifyhq-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autifyhq/openapi/autifyhq-default-api-openapi.yml
- filename: autifyhq-payload-api-openapi.yml
  format: yaml
  label: Autifyhq Payload API
  slug: autifyhq-payload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autifyhq/openapi/autifyhq-payload-api-openapi.yml
- filename: autifyhq-projects-api-openapi.yml
  format: yaml
  label: Autifyhq Projects API
  slug: autifyhq-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autifyhq/openapi/autifyhq-projects-api-openapi.yml
- filename: autifyhq-workspaces-api-openapi.yml
  format: yaml
  label: Autifyhq Workspaces API
  slug: autifyhq-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autifyhq/openapi/autifyhq-workspaces-api-openapi.yml
consequence_counts:
  read: 8
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Autifyhq Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Autifyhq exposes 10 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Autifyhq
provider_slug: autifyhq
slug: autifyhq-agentic-access
source_filename: autifyhq-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/autifyhq-autify-cli-api-openapi.yml, openapi/autifyhq-default-api-openapi.yml,\n  openapi/autifyhq-payload-api-openapi.yml, openapi/autifyhq-projects-api-openapi.yml, openapi/autifyhq-workspaces-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 8\n    acting: 2\n  by_consequence:\n    read: 8\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /autify-cli/channels/stable/{stableid}\n  method: get\n  operationId: get_autify_cli_channels_stable_stableid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autify-cli/versions/0.2.0/b03bec6/autify-v0.2.0-b03bec6-darwin-arm64.tar.gz\n\
  \  method: get\n  operationId: get_autify_cli_versions_0_2_0_b03bec6_autify_v0_2_0_b03bec6_darwin_arm64_tar_gz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/~\n  method: get\n  operationId: get_api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payload\n  method: post\n  operationId: post_payload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/projects/{projectid}\n  method: get\n  operationId: get_api_v1_projects_projectid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /projects/0/results/{resultid}\n  method: get\n  operationId: get_projects_0_results_resultid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/workspaces\n  method: get\n  operationId: get_api_workspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/workspaces/{workspaceid}/testPlans/{testplanid}/{id}\n  method: post\n  operationId: post_api_workspaces_workspaceid_testPlans_testplanid_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/workspaces/{workspaceid}/testResults/{executionresultid}/status\n\
  \  method: get\n  operationId: get_api_workspaces_workspaceid_testResults_executionresultid_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/workspaces/{workspaceid}/{id}\n  method: get\n  operationId: get_api_workspaces_workspaceid_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/autifyhq/agentic-access/autifyhq-agentic-access.yml
summary_line: 10 operations · 2 acting
tags:
- Company
- Artificial Intelligence
- Testing
- Automation
- Software-as-a-Service
---
