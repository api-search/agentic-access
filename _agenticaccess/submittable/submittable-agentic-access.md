---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 14
api_specs:
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Submissions API
  slug: submittable-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Entries API
  slug: submittable-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Projects and Forms API
  slug: submittable-projects-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Users (Submitters) API
  slug: submittable-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Teams and Reviews API
  slug: submittable-teams-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Labels API
  slug: submittable-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
- filename: submittable-openapi.yml
  format: yaml
  label: Submittable Funds and Payments API
  slug: submittable-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/openapi/submittable-openapi.yml
consequence_counts:
  read: 14
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Submittable Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Submittable exposes 19 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Submittable
provider_slug: submittable
slug: submittable-agentic-access
source_filename: submittable-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/submittable-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 14\n    acting: 5\n  by_consequence:\n    read: 14\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /submissions\n  method: get\n  operationId: listSubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions/{submissionId}\n  method: get\n  operationId: getSubmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions/{submissionId}\n\
  \  method: patch\n  operationId: updateSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entries\n  method: get\n  operationId: listEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entries/{entryId}\n  method: get\n  operationId: getEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entries/submissions/{submissionId}\n  method: get\n  operationId: getSubmissionEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}\n  method: patch\n  operationId: updateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/team\n  method: get\n  operationId: listTeamMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions/team/assignment\n  method: post\n  operationId: assignSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labels\n  method: get\n  operationId: listLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labels\n  method: post\n  operationId: createLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /funds\n  method: get\n  operationId: listFunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/{messageId}/files\n  method: get\n  operationId: getMessageFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/submittable/refs/heads/main/agentic-access/submittable-agentic-access.yml
summary_line: 19 operations · 5 acting
tags:
- Submission Management
- Grants Management
- Applications
- Forms
- Nonprofit
- Corporate Social Responsibility
- Workflow
---
