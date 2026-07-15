---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 10
api_specs:
- filename: swagger-v3.v3.json
  format: json
  label: Jira Cloud Platform REST API
  slug: jira-cloud-platform-rest-api
  spec_type: OpenAPI
  url: https://dac-static.atlassian.com/cloud/jira/platform/swagger-v3.v3.json
- filename: swagger.v3.json
  format: json
  label: Jira Software Cloud REST API
  slug: jira-software-cloud-rest-api
  spec_type: OpenAPI
  url: https://dac-static.atlassian.com/cloud/jira/software/swagger.v3.json
- filename: swagger.v3.json
  format: json
  label: Jira Service Management REST API
  slug: jira-service-management-rest-api
  spec_type: OpenAPI
  url: https://dac-static.atlassian.com/cloud/jira/service-desk/swagger.v3.json
consequence_counts:
  read: 10
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Jira Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Jira exposes 16 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Jira
provider_slug: jira
slug: jira-agentic-access
source_filename: jira-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/jira-cloud-platform-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 6\n    connected: 10\n  by_consequence:\n    write: 6\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /issue\n  method: post\n  operationId: createIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issue/{issueIdOrKey}\n  method: get\n  operationId: getIssue\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issue/{issueIdOrKey}\n  method: put\n  operationId: editIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issue/{issueIdOrKey}\n  method: delete\n  operationId: deleteIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issue/{issueIdOrKey}/transitions\n  method: get\n  operationId: getTransitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /issue/{issueIdOrKey}/transitions\n  method: post\n  operationId: doTransition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issue/{issueIdOrKey}/comment\n  method: get\n  operationId: getComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /issue/{issueIdOrKey}/comment\n  method: post\n  operationId: addComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project\n\
  \  method: get\n  operationId: getAllProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/search\n  method: get\n  operationId: searchProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/{projectIdOrKey}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/{projectIdOrKey}/statuses\n  method: get\n  operationId: getAllStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: searchForIssuesUsingJql\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: post\n  operationId: searchForIssuesUsingJqlPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /issuetype\n  method: get\n  operationId: getIssueAllTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /priority\n  method: get\n  operationId: getPriorities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/agentic-access/jira-agentic-access.yml
summary_line: 16 operations · 6 acting
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
---
