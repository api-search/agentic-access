---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 1
api_specs:
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Send API
  slug: notificationapi-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Schedule API
  slug: notificationapi-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Users Identify API
  slug: notificationapi-users-identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI User Preferences API
  slug: notificationapi-user-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Notifications Config API
  slug: notificationapi-notifications-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI In-App Inbox API
  slug: notificationapi-in-app-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Logs API
  slug: notificationapi-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
consequence_counts:
  physical: 2
  read: 1
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Notificationapi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sender
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sender/retract
operation_count: 12
overview: 'NotificationAPI exposes 12 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 9 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NotificationAPI
provider_slug: notificationapi
slug: notificationapi-agentic-access
source_filename: notificationapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/notificationapi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 11\n    connected: 1\n  by_consequence:\n    physical: 2\n    write: 9\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /sender\n  method: post\n  operationId: send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sender/retract\n  method: post\n  operationId: retract\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedule/{trackingId}\n  method: patch\n  operationId: updateSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedule/{trackingId}\n  method: delete\n  operationId: deleteSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /users/{userId}\n  method: post\n  operationId: identifyUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/preferences\n  method: delete\n  operationId: deleteUserPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user_preferences/{userId}\n  method: post\n  operationId: setUserPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications/{notificationId}/subNotifications/{subNotificationId}\n  method: put\n  operationId: createSubNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications/{notificationId}/subNotifications/{subNotificationId}\n  method: delete\n  operationId: deleteSubNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/notifications/INAPP_WEB\n  method: get\n \
  \ operationId: getInAppNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/notifications/INAPP_WEB\n  method: patch\n  operationId: updateInAppNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logs/query\n  method: post\n  operationId: queryLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/agentic-access/notificationapi-agentic-access.yml
summary_line: 12 operations · 11 acting
tags:
- Notifications
- Messaging
- Email
- SMS
- Push
- In-App Inbox
---
