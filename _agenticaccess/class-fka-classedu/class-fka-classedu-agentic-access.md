---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 8
api_specs:
- filename: class-fka-classedu-openapi.yml
  format: yaml
  label: Class Developer API
  slug: class-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/class-fka-classedu/refs/heads/main/openapi/class-fka-classedu-openapi.yml
consequence_counts:
  read: 8
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Class Fka Classedu Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'Class (fka ClassEDU) exposes 21 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Class (fka ClassEDU)
provider_slug: class-fka-classedu
slug: class-fka-classedu-agentic-access
source_filename: class-fka-classedu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/class-fka-classedu-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 13\n    connected: 8\n  by_consequence:\n    write: 13\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/classes\n  method: post\n  operationId: createClass\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - class:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/classes\n  method: get\n  operationId: getClasses\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - class:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/classes\n  method: patch\n  operationId: updateClass\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - class:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/classes\n  method: delete\n  operationId: deleteClass\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - class:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/class/enrollments\n  method: post\n  operationId: createEnrollment\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - enrollment:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/class/enrollments\n  method: get\n  operationId: getEnrollments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - enrollment:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/class/enrollments\n  method: put\n  operationId: updateEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - enrollment:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/class/enrollments\n  method: delete\n\
  \  operationId: deleteEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - enrollment:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/class/enrollments/launch\n  method: get\n  operationId: getLaunchLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - enrollment:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reporting/attendance\n  method: get\n  operationId: getAttendance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - attendance:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reporting/metrics\n  method: get\n  operationId: getMetrics\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - metrics:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/schedules\n  method: post\n  operationId: addClassDate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - schedule:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/schedules\n  method: get\n  operationId: getClassDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - schedule:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/schedules\n  method: delete\n  operationId: removeClassDate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - schedule:write\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates\n  method: post\n  operationId: createTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - template:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates\n  method: get\n  operationId: getTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - template:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates\n  method: patch\n  operationId: updateTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - template:write\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates\n  method: delete\n  operationId: deleteTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - template:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users\n  method: put\n  operationId: upsertUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - user:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/class-fka-classedu/refs/heads/main/agentic-access/class-fka-classedu-agentic-access.yml
summary_line: 21 operations · 13 acting
tags:
- Company
- Education
- EdTech
- Virtual Classroom
- Learning Management
- Online Learning
- Training
- Zoom
- Microsoft Teams
- Attendance
---
