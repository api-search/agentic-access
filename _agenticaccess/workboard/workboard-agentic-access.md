---
acting_count: 32
action_class_counts:
  acting: 32
  connected: 31
api_specs:
- filename: workboard-activity-action-items-api-openapi.yml
  format: yaml
  label: WorkBoard Activity (Action Items) API
  slug: workboard-activity-action-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-activity-action-items-api-openapi.yml
- filename: workboard-custom-attributes-api-openapi.yml
  format: yaml
  label: WorkBoard custom-attributes API
  slug: workboard-custom-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-custom-attributes-api-openapi.yml
- filename: workboard-datastream-api-openapi.yml
  format: yaml
  label: WorkBoard Datastream API
  slug: workboard-datastream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-datastream-api-openapi.yml
- filename: workboard-goal-objective-api-openapi.yml
  format: yaml
  label: WorkBoard Goal (Objective) API
  slug: workboard-goal-objective-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-goal-objective-api-openapi.yml
- filename: workboard-metric-key-result-api-openapi.yml
  format: yaml
  label: WorkBoard Metric (Key Result) API
  slug: workboard-metric-key-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-metric-key-result-api-openapi.yml
- filename: workboard-tags-api-openapi.yml
  format: yaml
  label: WorkBoard Tags API
  slug: workboard-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-tags-api-openapi.yml
- filename: workboard-team-api-openapi.yml
  format: yaml
  label: WorkBoard Team API
  slug: workboard-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-team-api-openapi.yml
- filename: workboard-user-api-openapi.yml
  format: yaml
  label: WorkBoard User API
  slug: workboard-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-user-api-openapi.yml
- filename: workboard-user-goals-user-objectives-api-openapi.yml
  format: yaml
  label: WorkBoard User Goals (User Objectives) API
  slug: workboard-user-goals-user-objectives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-user-goals-user-objectives-api-openapi.yml
- filename: workboard-webhook-api-openapi.yml
  format: yaml
  label: WorkBoard Webhook API
  slug: workboard-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-webhook-api-openapi.yml
- filename: workboard-workstream-api-openapi.yml
  format: yaml
  label: WorkBoard Workstream API
  slug: workboard-workstream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/openapi/workboard-workstream-api-openapi.yml
consequence_counts:
  read: 31
  safety-critical: 12
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 12
kind: agentic-access
layout: agentic-access
method: generated
name: Workboard Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /attributes/key-results/{id}/{attributeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /attributes/key-results/{id}/{attributeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /attributes/key-results/{id}/{attributeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /attributes/objectives/{id}/{attributeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /attributes/objectives/{id}/{attributeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /attributes/objectives/{id}/{attributeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /attributes/users/{id}/{attributeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /attributes/users/{id}/{attributeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /attributes/users/{id}/{attributeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /attributes/work-items/{id}/{attributeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /attributes/work-items/{id}/{attributeId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /attributes/work-items/{id}/{attributeId}
operation_count: 63
overview: 'WorkBoard exposes 63 API operations that an AI agent could call, of which 32 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read, 20 write, and 12 safety-critical.


  12 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WorkBoard
provider_slug: workboard
slug: workboard-agentic-access
source_filename: workboard-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/external-v1-openapi-original.yml, openapi/public-v2-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 63\n  by_action_class:\n    connected: 31\n    acting: 32\n  by_consequence:\n    read: 31\n    write: 20\n    safety-critical: 12\n  human_in_the_loop_required: 12\noperations:\n- path: /user\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{user_id_path}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{user_id_path}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{user_id_path}/goal\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{user_id_path}/goal/{goal_id_path}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/{team_id_path}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/{team_id_path}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/{team_id_path}/workstream\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /team/{team_id_path}/activity\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /goal\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /goal\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /goal/{goal_id_path}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /goal/{goal_id_path}/metric/{metric_id_path}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /goal/{goal_id_path}/pillars\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /goal/{goal_id_path}/alignment\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metric\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metric/{metric_id_path}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metric/{metric_id_path}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /metric/{metric_id_path}/confidence\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metric/{metric_id_path}/tags\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metric/{metric_id_path}/tags\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metric/{metric_id_path}/tags\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metric/krtags\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metric/tags\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metric/tags\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/{tag_id_path}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activity\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activity\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activity/{ai_id_path}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activity/{ai_id_path}\n  method: put\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workstream\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workstream\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workstream/{ws_id_path}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workstream/{ws_id_path}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workstream/{ws_id_path}/activity\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stream\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stream\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stream/{stream_id}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hook/{webhook_hash}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attributes/definitions\n  method: get\n  operationId: CustomAttributesController_getDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attributes/{attributeId}/objects\n\
  \  method: get\n  operationId: CustomAttributesController_getObjectsForAttribute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attributes/objectives/{id}\n  method: get\n  operationId: CustomAttributesController_getObjectiveAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attributes/objectives/{id}/{attributeId}\n  method: post\n  operationId: CustomAttributesController_createObjectiveAttributeValue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /attributes/objectives/{id}/{attributeId}\n  method:\
  \ put\n  operationId: CustomAttributesController_setObjectiveAttributeValue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /attributes/objectives/{id}/{attributeId}\n  method: delete\n  operationId: CustomAttributesController_deleteObjectiveAttributeValue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /attributes/key-results/{id}\n  method: get\n  operationId: CustomAttributesController_getKeyResultAttributes\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attributes/key-results/{id}/{attributeId}\n  method: post\n  operationId: CustomAttributesController_createKeyResultAttributeValue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /attributes/key-results/{id}/{attributeId}\n  method: put\n  operationId: CustomAttributesController_setKeyResultAttributeValue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /attributes/key-results/{id}/{attributeId}\n  method: delete\n  operationId: CustomAttributesController_deleteKeyResultAttributeValue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /attributes/work-items/{id}\n  method: get\n  operationId: CustomAttributesController_getWorkItemAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attributes/work-items/{id}/{attributeId}\n  method: post\n  operationId: CustomAttributesController_createWorkItemAttributeValue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /attributes/work-items/{id}/{attributeId}\n  method: put\n  operationId: CustomAttributesController_setWorkItemAttributeValue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /attributes/work-items/{id}/{attributeId}\n  method: delete\n  operationId: CustomAttributesController_deleteWorkItemAttributeValue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /attributes/users/{id}\n  method: get\n  operationId: CustomAttributesController_getUserAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attributes/users/{id}/{attributeId}\n  method: post\n  operationId: CustomAttributesController_createUserAttributeValue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /attributes/users/{id}/{attributeId}\n  method: put\n  operationId: CustomAttributesController_setUserAttributeValue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /attributes/users/{id}/{attributeId}\n  method: delete\n  operationId: CustomAttributesController_deleteUserAttributeValue\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workboard/refs/heads/main/agentic-access/workboard-agentic-access.yml
summary_line: 63 operations · 32 acting · 12 human-in-the-loop
tags:
- OKRs
- Strategy Execution
- Goals
- Key Results
- Enterprise
- AI Agents
- Performance Management
- Strategic Portfolio Management
---
