---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 20
api_specs:
- filename: schoology-assignments-api-openapi.yml
  format: yaml
  label: Schoology Assignments API
  slug: schoology-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-assignments-api-openapi.yml
- filename: schoology-courses-api-openapi.yml
  format: yaml
  label: Schoology Courses API
  slug: schoology-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-courses-api-openapi.yml
- filename: schoology-enrollments-api-openapi.yml
  format: yaml
  label: Schoology Enrollments API
  slug: schoology-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-enrollments-api-openapi.yml
- filename: schoology-grades-api-openapi.yml
  format: yaml
  label: Schoology Grades API
  slug: schoology-grades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-grades-api-openapi.yml
- filename: schoology-groups-api-openapi.yml
  format: yaml
  label: Schoology Groups API
  slug: schoology-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-groups-api-openapi.yml
- filename: schoology-multi-call-api-openapi.yml
  format: yaml
  label: Schoology Multi-Call API
  slug: schoology-multi-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-multi-call-api-openapi.yml
- filename: schoology-sections-api-openapi.yml
  format: yaml
  label: Schoology Sections API
  slug: schoology-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-sections-api-openapi.yml
- filename: schoology-submissions-api-openapi.yml
  format: yaml
  label: Schoology Submissions API
  slug: schoology-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-submissions-api-openapi.yml
- filename: schoology-subscriptions-api-openapi.yml
  format: yaml
  label: Schoology Subscriptions API
  slug: schoology-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-subscriptions-api-openapi.yml
- filename: schoology-targets-api-openapi.yml
  format: yaml
  label: Schoology Targets API
  slug: schoology-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-targets-api-openapi.yml
- filename: schoology-users-api-openapi.yml
  format: yaml
  label: Schoology Users API
  slug: schoology-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-users-api-openapi.yml
- filename: schoology-events-api-openapi.yml
  format: yaml
  label: Schoology Events API
  slug: schoology-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/openapi/schoology-events-api-openapi.yml
consequence_counts:
  read: 20
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Schoology Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'Schoology exposes 28 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Schoology
provider_slug: schoology
slug: schoology-agentic-access
source_filename: schoology-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/schoology-openapi.yml, openapi/schoology-webhooks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 20\n    acting: 8\n  by_consequence:\n    read: 20\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/ext/{external_id}\n\
  \  method: get\n  operationId: getUserByExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/sections\n  method: get\n  operationId: listUserSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/groups\n  method: get\n  operationId: listUserGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/grades\n  method: get\n  operationId: getUserGrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses\n  method: get\n  operationId: listCourses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/{id}\n  method: get\n  operationId: getCourse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections\n  method: get\n  operationId: listSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/{id}\n  method: get\n  operationId: getSection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/ext/{external_id}\n  method: get\n  operationId: getSectionByExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/{section_id}/enrollments\n  method: get\n  operationId:\
  \ listSectionEnrollments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/{section_id}/enrollments\n  method: post\n  operationId: createSectionEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/enrollments\n  method: get\n  operationId: listGroupEnrollments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/{section_id}/assignments\n  method: get\n  operationId: listAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /sections/{section_id}/assignments\n  method: post\n  operationId: createAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sections/{section_id}/assignments/{id}\n  method: get\n  operationId: getAssignment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/{section_id}/grades\n  method: get\n  operationId: listSectionGrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/{section_id}/submissions/{grade_item_id}\n  method: get\n  operationId: listSubmissions\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections/{section_id}/submissions/{grade_item_id}/{user_id}\n  method: get\n  operationId: getSubmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /multiget\n  method: post\n  operationId: multiget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /multioptions\n  method: post\n  operationId: multioptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /triggers/targets\n  method: get\n  operationId: listTriggerTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /triggers/targets\n  method: post\n  operationId: createTriggerTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /triggers/targets/{target_id}\n  method: put\n  operationId: updateTriggerTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /triggers/targets/{target_id}\n  method: delete\n  operationId: deleteTriggerTarget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /triggers/subscriptions\n  method: get\n  operationId: listTriggerSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /triggers/subscriptions\n  method: put\n  operationId: upsertTriggerSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schoology/refs/heads/main/agentic-access/schoology-agentic-access.yml
summary_line: 28 operations · 8 acting
tags:
- EdTech
- LMS
- K-12
---
