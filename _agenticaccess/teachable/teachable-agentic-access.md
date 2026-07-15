---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 22
api_specs:
- filename: teachable-admin-openapi.yml
  format: yaml
  label: Teachable Admin API
  slug: teachable-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-admin-openapi.yml
- filename: teachable-oauth-openapi.yml
  format: yaml
  label: Teachable OAuth API
  slug: teachable-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-oauth-openapi.yml
consequence_counts:
  read: 22
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Teachable Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'Teachable exposes 28 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Teachable
provider_slug: teachable
slug: teachable-agentic-access
source_filename: teachable-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/teachable-admin-openapi.yml, openapi/teachable-oauth-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 22\n    acting: 6\n  by_consequence:\n    read: 22\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /courses\n  method: get\n  operationId: listCourses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/{course_id}\n  method: get\n  operationId: getCourse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /courses/{course_id}/enrollments\n  method: get\n  operationId: listCourseEnrollments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/{course_id}/progress\n  method: get\n  operationId: getCourseProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/{course_id}/lectures/{lecture_id}\n  method: get\n  operationId: getLecture\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/{course_id}/lectures/{lecture_id}/mark_complete\n  method: post\n  operationId: markLectureComplete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /courses/{course_id}/lectures/{lecture_id}/videos/{video_id}\n  method: get\n  operationId: getVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/{course_id}/lectures/{lecture_id}/quizzes\n  method: get\n  operationId: listQuizzes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/{course_id}/lectures/{lecture_id}/quizzes/{quiz_id}\n  method: get\n  operationId: getQuiz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/{course_id}/lectures/{lecture_id}/quizzes/{quiz_id}/responses\n  method: get\n  operationId: getQuizResponses\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enroll\n  method: post\n  operationId: enrollUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unenroll\n  method: post\n  operationId: unenrollUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{user_id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_id}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pricing_plans\n  method: get\n  operationId: listPricingPlans\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing_plans/{pricing_plan_id}\n  method: get\n  operationId: getPricingPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{webhook_id}/events\n  method: get\n  operationId: listWebhookEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /current_user/me\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - email:read\n    - name:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /current_user/courses\n  method: get\n  operationId: listCurrentUserCourses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - courses:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /current_user/courses/{course_id}\n  method: get\n  operationId: getCurrentUserCourse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - courses:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /current_user/courses/{course_id}/progress\n  method: get\n  operationId: getCurrentUserCourseProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - courses:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /current_user/courses/{course_id}/lectures/{lecture_id}\n  method: get\n  operationId: getCurrentUserLecture\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - courses:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /current_user/courses/{course_id}/lectures/{lecture_id}/mark_complete\n  method: post\n  operationId: markCurrentUserLectureComplete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - courses:read\n    - courses:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /current_user/courses/{course_id}/lectures/{lecture_id}/videos/{video_id}\n  method: get\n  operationId: getCurrentUserVideo\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - courses:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/agentic-access/teachable-agentic-access.yml
summary_line: 28 operations · 6 acting
tags:
- Online Courses
- E-Learning
- Education
- Course Management
- Enrollments
- Coaching
- Memberships
- Transactions
---
