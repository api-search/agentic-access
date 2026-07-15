---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: rest
  format: yaml
  label: Android Management API
  slug: android-management-api
  spec_type: OpenAPI
  url: https://androidmanagement.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Play Developer API
  slug: google-play-developer-api
  spec_type: OpenAPI
  url: https://androidpublisher.googleapis.com/$discovery/rest?version=v3
- filename: rest
  format: yaml
  label: Firebase Cloud Messaging API
  slug: firebase-cloud-messaging-api
  spec_type: OpenAPI
  url: https://fcm.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Play Games Services API
  slug: google-play-games-services-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/games/v1/rest
- filename: rest
  format: yaml
  label: Android Over the Air API
  slug: android-over-the-air-api
  spec_type: OpenAPI
  url: https://androidovertheair.googleapis.com/$discovery/rest?version=v1
consequence_counts:
  read: 8
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Android Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Google Android exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Android
provider_slug: google-android
slug: google-android-agentic-access
source_filename: google-android-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-android-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 7\n    connected: 8\n  by_consequence:\n    write: 7\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/enterprises\n  method: post\n  operationId: createEnterprise\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidmanagement\n- path: /v1/enterprises\n  method: get\n  operationId: listEnterprises\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidmanagement\n- path: /v1/{name}\n  method: get\n  operationId: getEnterprise\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidmanagement\n- path: /v1/{name}\n  method: patch\n  operationId: patchEnterprise\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidmanagement\n- path: /v1/{name}\n  method: delete\n  operationId: deleteEnterprise\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidmanagement\n- path: /v1/{parent}/devices\n  method: get\n  operationId: listDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidmanagement\n- path: /v1/{name}/device\n  method: get\n  operationId: getDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidmanagement\n- path: /v1/{name}:issueCommand\n  method: post\n  operationId: issueDeviceCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n    scope:\n    - androidmanagement\n- path: /v1/{parent}/policies\n  method: get\n  operationId: listPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidmanagement\n- path: /v1/{name}/policy\n  method: get\n  operationId: getPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidmanagement\n- path: /v1/{name}/policy\n  method: patch\n  operationId: patchPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidmanagement\n- path: /v1/{parent}/enrollmentTokens\n\
  \  method: post\n  operationId: createEnrollmentToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - androidmanagement\n- path: /v1/{parent}/enrollmentTokens\n  method: get\n  operationId: listEnrollmentTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidmanagement\n- path: /v1/{parent}/webApps\n  method: post\n  operationId: createWebApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n\
  \    - androidmanagement\n- path: /v1/{parent}/webApps\n  method: get\n  operationId: listWebApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - androidmanagement\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-android/refs/heads/main/agentic-access/google-android-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Android
- Google
- Mobile Development
- Mobile Operating System
- Open Source
---
