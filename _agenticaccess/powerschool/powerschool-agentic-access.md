---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 13
api_specs:
- filename: powerschool-powerschool-sis-api-openapi.yml
  format: yaml
  label: PowerSchool SIS REST API
  slug: powerschool-sis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerschool/refs/heads/main/openapi/powerschool-powerschool-sis-api-openapi.yml
consequence_counts:
  read: 13
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Powerschool Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'PowerSchool exposes 15 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PowerSchool
provider_slug: powerschool
slug: powerschool-agentic-access
source_filename: powerschool-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/powerschool-powerschool-sis-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 2\n    connected: 13\n  by_consequence:\n    write: 2\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/access_token/\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/v1/metadata\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/v1/district/school\n  method: get\n  operationId: getSchools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/v1/district/school/count\n  method: get\n  operationId: getSchoolsCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/v1/district/student\n  method: get\n  operationId: getStudentsInDistrict\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/v1/district/student/count\n  method: get\n  operationId: getStudentsInDistrictCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /ws/v1/district/student/{studentDcid}\n  method: get\n  operationId: getStudent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/v1/school/{schoolDcid}\n  method: get\n  operationId: getSchool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/v1/school/{schoolDcid}/course\n  method: get\n  operationId: getCoursesForSchool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/v1/school/{schoolDcid}/course/count\n  method: get\n  operationId: getCoursesCountForSchool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/v1/school/{schoolDcid}/section\n\
  \  method: get\n  operationId: getSectionsForSchool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/v1/school/{schoolDcid}/section/count\n  method: get\n  operationId: getSectionsCountForSchool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/schema/query/{queryName}\n  method: post\n  operationId: executePowerQuery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ws/schema/table/{tableName}\n  method: get\n  operationId: getSchemaTable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/schema/table/{tableName}/count\n  method: get\n  operationId: getSchemaTableCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powerschool/refs/heads/main/agentic-access/powerschool-agentic-access.yml
summary_line: 15 operations · 2 acting
tags:
- K-12
- Education
- Student Information System
- SIS
- Students
- Grades
- Attendance
- Enrollment
- Scheduling
- EdTech
---
