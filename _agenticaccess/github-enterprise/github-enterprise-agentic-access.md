---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 12
api_specs:
- filename: rest-api-description
  format: yaml
  label: GitHub Enterprise Cloud REST API
  slug: cloud-rest-api
  spec_type: OpenAPI
  url: https://github.com/github/rest-api-description
- filename: rest-api-description
  format: yaml
  label: GitHub Enterprise Server REST API
  slug: server-rest-api
  spec_type: OpenAPI
  url: https://github.com/github/rest-api-description
consequence_counts:
  physical: 1
  read: 12
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Github Enterprise Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /scim/v2/enterprises/{enterprise}/Users
operation_count: 17
overview: 'GitHub Enterprise exposes 17 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GitHub Enterprise
provider_slug: github-enterprise
slug: github-enterprise-agentic-access
source_filename: github-enterprise-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/github-enterprise-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 12\n    acting: 5\n  by_consequence:\n    read: 12\n    write: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /user\n  method: get\n  operationId: getAuthenticatedUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{username}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}\n\
  \  method: get\n  operationId: getOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/repos\n  method: get\n  operationId: listOrgRepos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org}/repos\n  method: post\n  operationId: createOrgRepo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}\n  method: get\n  operationId: getRepo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}\n\
  \  method: delete\n  operationId: deleteRepo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/issues\n  method: get\n  operationId: listIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/issues\n  method: post\n  operationId: createIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/pulls\n  method: get\n  operationId: listPullRequests\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/pulls\n  method: post\n  operationId: createPullRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /repos/{owner}/{repo}/actions/workflows\n  method: get\n  operationId: listWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/actions/runs\n  method: get\n  operationId: listWorkflowRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /repos/{owner}/{repo}/code-scanning/alerts\n\
  \  method: get\n  operationId: listCodeScanningAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enterprises/{enterprise}/audit-log\n  method: get\n  operationId: getEnterpriseAuditLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/enterprises/{enterprise}/Users\n  method: get\n  operationId: listScimUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/enterprises/{enterprise}/Users\n  method: post\n  operationId: createScimUser\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-enterprise/refs/heads/main/agentic-access/github-enterprise-agentic-access.yml
summary_line: 17 operations · 5 acting
tags:
- Source Control
- DevOps
- CI/CD
- Code Hosting
- Enterprise
- Self-Hosted
- SAML SSO
- SCIM
- Advanced Security
---
