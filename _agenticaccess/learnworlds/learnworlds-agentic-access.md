---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 10
api_specs:
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Users API
  slug: learnworlds-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Courses API
  slug: learnworlds-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Enrollments API
  slug: learnworlds-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Payments API
  slug: learnworlds-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Progress API
  slug: learnworlds-progress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Tags API
  slug: learnworlds-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Webhooks API
  slug: learnworlds-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
consequence_counts:
  read: 10
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Learnworlds Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'LearnWorlds exposes 18 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LearnWorlds
provider_slug: learnworlds
slug: learnworlds-agentic-access
source_filename: learnworlds-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/learnworlds-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 10\n    acting: 8\n  by_consequence:\n    read: 10\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method: put\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}/enrollment\n  method: post\n  operationId: enrollUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}/enrollment\n\
  \  method: delete\n  operationId: unenrollUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}/enrollments\n  method: get\n  operationId: listUserEnrollments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/progress\n  method: get\n  operationId: getUserProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}/tags\n  method: post\n  operationId: attachUserTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}/tags\n  method: delete\n  operationId: detachUserTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /courses\n  method: get\n  operationId: listCourses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/{id}\n  method: get\n  operationId: getCourse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/{id}/contents\n  method: get\n  operationId: getCourseContents\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/agentic-access/learnworlds-agentic-access.yml
summary_line: 18 operations · 8 acting
tags:
- Online Courses
- LMS
- eLearning
- Education
- Course Platform
- Creator Economy
---
