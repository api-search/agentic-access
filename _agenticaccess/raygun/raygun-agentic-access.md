---
acting_count: 44
action_class_counts:
  acting: 44
  connected: 60
api_specs:
- filename: raygun-applications-api-openapi.yml
  format: yaml
  label: Raygun Applications API
  slug: raygun-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-applications-api-openapi.yml
- filename: raygun-errors-api-openapi.yml
  format: yaml
  label: Raygun Errors API
  slug: raygun-errors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-errors-api-openapi.yml
- filename: raygun-deployments-api-openapi.yml
  format: yaml
  label: Raygun Deployments API
  slug: raygun-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-deployments-api-openapi.yml
- filename: raygun-source-maps-api-openapi.yml
  format: yaml
  label: Raygun Source Maps API
  slug: raygun-source-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-source-maps-api-openapi.yml
- filename: raygun-sessions-api-openapi.yml
  format: yaml
  label: Raygun Sessions API
  slug: raygun-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-sessions-api-openapi.yml
- filename: raygun-pages-api-openapi.yml
  format: yaml
  label: Raygun Pages API
  slug: raygun-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-pages-api-openapi.yml
- filename: raygun-customers-api-openapi.yml
  format: yaml
  label: Raygun Customers API
  slug: raygun-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-customers-api-openapi.yml
- filename: raygun-metrics-api-openapi.yml
  format: yaml
  label: Raygun Metrics API
  slug: raygun-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-metrics-api-openapi.yml
- filename: raygun-flutter-symbols-api-openapi.yml
  format: yaml
  label: Raygun Flutter Symbols API
  slug: raygun-flutter-symbols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-flutter-symbols-api-openapi.yml
- filename: raygun-teams-api-openapi.yml
  format: yaml
  label: Raygun Teams API
  slug: raygun-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-teams-api-openapi.yml
- filename: raygun-invitations-api-openapi.yml
  format: yaml
  label: Raygun Invitations API
  slug: raygun-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-invitations-api-openapi.yml
- filename: raygun-plans-api-openapi.yml
  format: yaml
  label: Raygun Plans API
  slug: raygun-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-plans-api-openapi.yml
- filename: raygun-webhooks-asyncapi.yml
  format: yaml
  label: Raygun Outbound Webhooks
  slug: raygun-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/openapi/raygun-webhooks-asyncapi.yml
consequence_counts:
  physical: 12
  read: 60
  safety-critical: 2
  write: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Raygun Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /invitations/{invitation-identifier}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /invitations/{invitation-identifier}/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/api-key/{api-key}/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/api-key/{api-key}/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/{application-identifier}/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/{application-identifier}/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /applications/{application-identifier}/deployments/{deployment-identifier}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /applications/{application-identifier}/deployments/{deployment-identifier}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /applications/{application-identifier}/deployments/{deployment-identifier}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /applications/{application-identifier}/deployments/{deployment-identifier}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/{application-identifier}/deployments/{deployment-identifier}/reprocess-commits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/{application-identifier}/deployments/{deployment-identifier}/reprocess-commits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invitations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invitations
operation_count: 104
overview: 'Raygun exposes 104 API operations that an AI agent could call, of which 44 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 60 read, 30 write, 12 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Raygun
provider_slug: raygun
slug: raygun-agentic-access
source_filename: raygun-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/raygun-applications-api-openapi.yml, openapi/raygun-customers-api-openapi.yml,\n  openapi/raygun-deployments-api-openapi.yml, openapi/raygun-errors-api-openapi.yml, openapi/raygun-flutter-symbols-api-openapi.yml,\n  openapi/raygun-invitations-api-openapi.yml, openapi/raygun-metrics-api-openapi.yml, openapi/raygun-pages-api-openapi.yml,\n  openapi/raygun-plans-api-openapi.yml, openapi/raygun-public-api-openapi.yml, openapi/raygun-sessions-api-openapi.yml,\n  openapi/raygun-source-maps-api-openapi.yml, openapi/raygun-teams-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 104\n  by_action_class:\n    connected: 60\n    acting: 44\n  by_consequence:\n    read: 60\n    write:\
  \ 30\n    physical: 12\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /applications\n  method: get\n  operationId: list-applications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - applications:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}\n  method: get\n  operationId: get-application-by-identifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - applications:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/api-key/{api-key}\n  method: get\n  operationId: get-application-by-apikey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - applications:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/regenerate-api-key\n  method: post\n\
  \  operationId: regenerate-application-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - applications:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/customers\n  method: get\n  operationId: list-customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customers:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/customers/{customer-identifier}\n  method: get\n  operationId: get-customer-by-identifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customers:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/deployments\n\
  \  method: get\n  operationId: list-deployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - deployments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/deployments\n  method: post\n  operationId: create-deployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - deployments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/deployments/latest\n  method: get\n  operationId: get-latest-deployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - deployments:read\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /applications/{application-identifier}/deployments/{deployment-identifier}\n  method: get\n  operationId: get-deployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - deployments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/deployments/{deployment-identifier}\n  method: delete\n  operationId: delete-deployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - deployments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/deployments/{deployment-identifier}\n  method: patch\n  operationId: update-deployment\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    scope:\n    - deployments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/deployments/latest/error-groups\n  method: get\n  operationId: list-error-groups-from-latest-deployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/deployments/{deployment-identifier}/error-groups\n  method: get\n  operationId: list-error-groups-from-deployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /applications/api-key/{api-key}/deployments\n  method: post\n  operationId: create-deployment-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - deployments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/deployments/{deployment-identifier}/reprocess-commits\n  method: post\n  operationId: reprocess-deployment-commits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - deployments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /applications/{application-identifier}/error-groups\n  method: get\n  operationId: list-error-groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/deployments/latest/error-groups\n  method: get\n  operationId: list-error-groups-from-latest-deployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/deployments/{deployment-identifier}/error-groups\n  method: get\n  operationId: list-error-groups-from-deployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}\n\
  \  method: get\n  operationId: get-error-group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/resolve\n  method: post\n  operationId: error-group-resolve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.errors:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/activate\n  method: post\n  operationId: error-group-activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.errors:write\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/ignore\n  method: post\n  operationId: error-group-ignore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.errors:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/permanently-ignore\n  method: post\n  operationId: error-group-permanently-ignore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.errors:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/comment\n  method: post\n  operationId: error-group-create-comment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.errors:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/instances\n  method: get\n  operationId: list-error-instances-by-error-group-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/instance/latest\n  method:\
  \ get\n  operationId: get-latest-error-instance-by-error-group-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/instance/{error-instance-identifier}\n  method: get\n  operationId: get-error-instance-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/flutter-symbols\n  method: get\n  operationId: list-flutter-symbols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.flutter-symbols:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/flutter-symbols\n  method: post\n  operationId:\
  \ upload-flutter-symbol\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.flutter-symbols:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/flutter-symbols/{flutter-symbol-identifier}\n  method: get\n  operationId: get-flutter-symbol\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.flutter-symbols:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/flutter-symbols/{flutter-symbol-identifier}\n  method: delete\n  operationId: delete-flutter-symbol\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.flutter-symbols:write\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/flutter-symbols/{flutter-symbol-identifier}/content\n  method: get\n  operationId: get-flutter-symbol-content\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.flutter-symbols:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invitations\n  method: get\n  operationId: list-invitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - invitations:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invitations\n  method: post\n  operationId: send-invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - invitations:write\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invitations/{invitation-identifier}\n  method: get\n  operationId: get-invitation-by-identifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - invitations:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invitations/{invitation-identifier}/revoke\n  method: post\n  operationId: revoke-invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - invitations:write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /metrics/{application-identifier}/pages/time-series\n  method: post\n\
  \  operationId: metrics-pages-time-series\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - metrics:pages\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metrics/{application-identifier}/pages/histogram\n  method: post\n  operationId: metrics-pages-histogram\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - metrics:pages\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metrics/{application-identifier}/errors/time-series\n  method: post\n  operationId: metrics-errors-time-series\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - metrics:errors\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/pages\n  method: get\n  operationId: list-pages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - rum.pages:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/pages/{page-identifier}\n  method: get\n  operationId: get-page\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - rum.pages:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans\n  method: get\n  operationId: list-plans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications\n\
  \  method: get\n  operationId: list-applications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - applications:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}\n  method: get\n  operationId: get-application-by-identifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - applications:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/deployments\n  method: get\n  operationId: list-deployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - deployments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/deployments\n  method: post\n  operationId: create-deployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    scope:\n    - deployments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/deployments/latest\n  method: get\n  operationId: get-latest-deployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - deployments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/source-maps/{source-map-identifier}\n  method: patch\n  operationId: source-map-uri\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.source-maps:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /applications/{application-identifier}/source-maps/{source-map-identifier}\n  method: delete\n  operationId: delete-source-map\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.source-maps:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/source-maps/{source-map-identifier}\n  method: get\n  operationId: source-map\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.source-maps:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/source-maps\n  method: get\n  operationId: list-source-maps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - cr.source-maps:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/source-maps\n  method: put\n  operationId: upload-source-map\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.source-maps:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/source-maps\n  method: delete\n  operationId: delete-all-source-maps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.source-maps:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/deployments/{deployment-identifier}\n\
  \  method: get\n  operationId: get-deployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - deployments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/deployments/{deployment-identifier}\n  method: delete\n  operationId: delete-deployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - deployments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/deployments/{deployment-identifier}\n  method: patch\n  operationId: update-deployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - deployments:write\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/error-groups\n  method: get\n  operationId: list-error-groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/deployments/latest/error-groups\n  method: get\n  operationId: list-error-groups-from-latest-deployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/deployments/{deployment-identifier}/error-groups\n  method: get\n  operationId: list-error-groups-from-deployment\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}\n  method: get\n  operationId: get-error-group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/resolve\n  method: post\n  operationId: error-group-resolve\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.errors:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/activate\n\
  \  method: post\n  operationId: error-group-activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.errors:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/ignore\n  method: post\n  operationId: error-group-ignore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.errors:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/permanently-ignore\n  method: post\n  operationId: error-group-permanently-ignore\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.errors:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/comment\n  method: post\n  operationId: error-group-create-comment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - cr.errors:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/instances\n  method: get\n  operationId: list-error-instances-by-error-group-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/instance/latest\n  method: get\n  operationId: get-latest-error-instance-by-error-group-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/error-groups/{error-group-identifier}/instance/{error-instance-identifier}\n  method: get\n  operationId: get-error-instance-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - cr.errors:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/api-key/{api-key}\n  method: get\n  operationId: get-application-by-apikey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - applications:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/api-key/{api-key}/deployments\n  method: post\n  operationId: create-deployment-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - deployments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/regenerate-api-key\n  method: post\n  operationId: regenerate-application-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - applications:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /invitations\n  method: get\n  operationId: list-invitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - invitations:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invitations\n  method: post\n  operationId: send-invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - invitations:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invitations/{invitation-identifier}\n  method: get\n  operationId: get-invitation-by-identifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - invitations:read\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /invitations/{invitation-identifier}/revoke\n  method: post\n  operationId: revoke-invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - invitations:write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /applications/{application-identifier}/deployments/{deployment-identifier}/reprocess-commits\n  method: post\n  operationId: reprocess-deployment-commits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - deployments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans\n\
  \  method: get\n  operationId: list-plans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams\n  method: get\n  operationId: list-teams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - teams:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams/{team-identifier}\n  method: get\n  operationId: get-team-by-identifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - teams:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/pages\n  method: get\n  operationId: list-pages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - rum.pages:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/pages/{page-identifier}\n\
  \  method: get\n  operationId: get-page\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - rum.pages:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/customers\n  method: get\n  operationId: list-customers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customers:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/customers/{customer-identifier}\n  method: get\n  operationId: get-customer-by-identifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - customers:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/sessions\n  method: get\n  operationId: list-sessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    scope:\n    - rum.sessions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application-identifier}/sessions/{session-identifier}\n  method: get\n  operationId: get-session-by-identifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - rum.sessions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics/{application-identifier}/pages/time-series\n  method: post\n  operationId: metrics-pages-time-series\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - metrics:pages\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metrics/{application-identifier}/pages/histogram\n  method: post\n  operationId: metrics-pages-histogram\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - metrics:pages\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metrics/{application-identifier}/errors/time-series\n  method: post\n  operationId: metrics-errors-time-series\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - metrics:errors\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application-identifier}/flutter-symbols\n  method: get\n  operationId: list-flutter-symbols\n  x-agentic-access:\n\n# --- truncated at 32 KB (36 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/agentic-access/raygun-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raygun/refs/heads/main/agentic-access/raygun-agentic-access.yml
summary_line: 104 operations · 44 acting · 2 human-in-the-loop
tags:
- Observability
- Crash Reporting
- Real User Monitoring
- Application Performance Monitoring
- Error Tracking
- Errors
- Monitoring
- DevOps
- Source Maps
- Deployments
---
