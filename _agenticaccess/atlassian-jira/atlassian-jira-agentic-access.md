---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: swagger-v3.v3.json
  format: json
  label: Jira Cloud Platform REST API
  slug: jira-cloud-platform-rest-api
  spec_type: OpenAPI
  url: https://developer.atlassian.com/cloud/jira/platform/swagger-v3.v3.json
- filename: swagger.v3.json
  format: json
  label: Jira Software Cloud REST API
  slug: jira-software-cloud-rest-api
  spec_type: OpenAPI
  url: https://developer.atlassian.com/cloud/jira/software/swagger.v3.json
- filename: swagger.v3.json
  format: json
  label: Jira Service Management REST API
  slug: jira-service-management-rest-api
  spec_type: OpenAPI
  url: https://developer.atlassian.com/cloud/jira/service-desk/swagger.v3.json
consequence_counts:
  read: 8
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Atlassian Jira Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Atlassian Jira exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Atlassian Jira
provider_slug: atlassian-jira
slug: atlassian-jira-agentic-access
source_filename: atlassian-jira-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/atlassian-jira-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 8\n    acting: 7\n  by_consequence:\n    read: 8\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /rest/api/3/issue/{issueIdOrKey}\n  method: get\n  operationId: getIssue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/api/3/issue/{issueIdOrKey}\n  method: put\n  operationId: editIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/api/3/issue/{issueIdOrKey}\n  method: delete\n  operationId: deleteIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/api/3/issues\n  method: post\n  operationId: createIssues\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/api/3/search\n  method: get\n  operationId: searchForIssuesUsingJql\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/api/3/project\n  method: get\n  operationId: getAllProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/api/3/project\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/api/3/project/{projectIdOrKey}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/api/3/user\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/api/3/issue/{issueIdOrKey}/comment\n  method: get\n  operationId: getComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/api/3/issue/{issueIdOrKey}/comment\n  method: post\n  operationId: addComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/api/3/issue/{issueIdOrKey}/comment/{id}\n  method: put\n  operationId: updateComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /rest/api/3/field\n  method: get\n  operationId: getFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/api/3/issue/{issueIdOrKey}/worklog\n  method: post\n  operationId: addWorklog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/api/3/issue/{issueIdOrKey}/transitions\n  method: get\n  operationId: getTransitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-jira/refs/heads/main/agentic-access/atlassian-jira-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Agile
- Atlassian
- Bug Tracking
- Issue Tracking
- ITSM
- Kanban
- Project Management
- Scrum
- Service Desk
---
