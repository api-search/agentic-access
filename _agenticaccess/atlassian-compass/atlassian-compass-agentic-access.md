---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 2
api_specs:
- filename: atlassian-compass-events-api-openapi.yml
  format: yaml
  label: Atlassian Compass Events API
  slug: atlassian-compass-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-events-api-openapi.yml
- filename: atlassian-compass-metrics-api-openapi.yml
  format: yaml
  label: Atlassian Compass Metrics API
  slug: atlassian-compass-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-metrics-api-openapi.yml
- filename: atlassian-compass-attachment-rest-controller-api-openapi.yml
  format: yaml
  label: Atlassian Compass Attachment Rest Controller API
  slug: atlassian-compass-attachment-rest-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-attachment-rest-controller-api-openapi.yml
- filename: atlassian-compass-entitlement-rest-controller-api-openapi.yml
  format: yaml
  label: Atlassian Compass Entitlement Rest Controller API
  slug: atlassian-compass-entitlement-rest-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-entitlement-rest-controller-api-openapi.yml
- filename: atlassian-compass-incoming-webhooks-rest-controller-api-openapi.yml
  format: yaml
  label: Atlassian Compass Incoming Webhooks Rest Controller API
  slug: atlassian-compass-incoming-webhooks-rest-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-incoming-webhooks-rest-controller-api-openapi.yml
- filename: atlassian-compass-package-dependencies-api-openapi.yml
  format: yaml
  label: Atlassian Compass Package Dependencies API
  slug: atlassian-compass-package-dependencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/openapi/atlassian-compass-package-dependencies-api-openapi.yml
consequence_counts:
  physical: 2
  read: 2
  safety-critical: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Atlassian Compass Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /compass/v1/component/{componentId}/api_specs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /compass/v1/component/{componentId}/api_specs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /compass/v1/component/{componentId}/app/{forgeAppId}/attachment/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /compass/v1/component/{componentId}/app/{forgeAppId}/attachment/{key}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /compass/v1/webhooks/{webhookId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /compass/v1/events
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /compass/v1/metrics
operation_count: 11
overview: 'Atlassian Compass exposes 11 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 2 write, 2 physical, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Atlassian Compass
provider_slug: atlassian-compass
slug: atlassian-compass-agentic-access
source_filename: atlassian-compass-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/atlassian-compass-attachment-rest-controller-api-openapi.yml, openapi/atlassian-compass-entitlement-rest-controller-api-openapi.yml,\n  openapi/atlassian-compass-events-api-openapi.yml, openapi/atlassian-compass-incoming-webhooks-rest-controller-api-openapi.yml,\n  openapi/atlassian-compass-metrics-api-openapi.yml, openapi/atlassian-compass-package-dependencies-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 2\n    acting: 9\n  by_consequence:\n    read: 2\n    safety-critical: 5\n    physical: 2\n    write: 2\n  human_in_the_loop_required: 5\noperations:\n- path: /compass/v1/component/{componentId}/app/{forgeAppId}/attachment/{key}\n\
  \  method: get\n  operationId: getAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compass/v1/component/{componentId}/app/{forgeAppId}/attachment/{key}\n  method: put\n  operationId: uploadAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /compass/v1/component/{componentId}/app/{forgeAppId}/attachment/{key}\n  method: delete\n  operationId: deleteAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /compass/v1/component/{componentId}/api_specs\n  method: put\n  operationId: uploadAPISpec\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /compass/v1/component/{componentId}/api_specs\n  method: delete\n  operationId: deleteAPISpec\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /compass/v1/entitlements\n  method: post\n  operationId: evaluateEntitlements\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compass/v1/events\n  method: post\n  operationId: createCompassEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compass/v1/webhooks/{webhookId}\n  method: post\n  operationId: handleWebhookInvocation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /compass/v1/metrics\n  method: post\n  operationId:\
  \ insertMetricValue\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compass/v1/package_dependencies/lock_file\n  method: put\n  operationId: uploadLockFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compass/v1/package_dependencies/lock_file/{componentId}/{sourceId}\n  method: delete\n  operationId: deleteLockFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlassian-compass/refs/heads/main/agentic-access/atlassian-compass-agentic-access.yml
summary_line: 11 operations · 9 acting · 5 human-in-the-loop
tags:
- Atlassian
- Component Management
- Developer Experience
- Software Catalog
- GraphQL
---
