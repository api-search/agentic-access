---
acting_count: 34
action_class_counts:
  acting: 34
  connected: 29
api_specs:
- filename: integration-app-actions-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Actions API
  slug: integration-app-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-actions-api-openapi.yml
- filename: integration-app-app-event-subscriptions-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) App Event Subscriptions API
  slug: integration-app-app-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-app-event-subscriptions-api-openapi.yml
- filename: integration-app-connections-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Connections API
  slug: integration-app-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-connections-api-openapi.yml
- filename: integration-app-connectors-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Connectors API
  slug: integration-app-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-connectors-api-openapi.yml
- filename: integration-app-customers-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Customers API
  slug: integration-app-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-customers-api-openapi.yml
- filename: integration-app-data-collections-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Data Collections API
  slug: integration-app-data-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-data-collections-api-openapi.yml
- filename: integration-app-external-event-subscriptions-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) External Event Subscriptions API
  slug: integration-app-external-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-external-event-subscriptions-api-openapi.yml
- filename: integration-app-field-mappings-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Field Mappings API
  slug: integration-app-field-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-field-mappings-api-openapi.yml
- filename: integration-app-flow-runs-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Flow Runs API
  slug: integration-app-flow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-flow-runs-api-openapi.yml
- filename: integration-app-flows-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Flows API
  slug: integration-app-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-flows-api-openapi.yml
- filename: integration-app-integrations-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Integrations API
  slug: integration-app-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-integrations-api-openapi.yml
- filename: integration-app-logs-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Logs API
  slug: integration-app-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-logs-api-openapi.yml
- filename: integration-app-public-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Public API
  slug: integration-app-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-public-api-openapi.yml
- filename: integration-app-search-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Search API
  slug: integration-app-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-search-api-openapi.yml
- filename: integration-app-sessions-api-openapi.yml
  format: yaml
  label: Integration.app (Membrane) Sessions API
  slug: integration-app-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/openapi/integration-app-sessions-api-openapi.yml
consequence_counts:
  physical: 1
  read: 29
  safety-critical: 2
  write: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Integration App Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /flow-runs/{id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sessions/{id}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sessions/{id}/message
operation_count: 63
overview: 'Integration.app (Membrane) exposes 63 API operations that an AI agent could call, of which 34 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 31 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Integration.app (Membrane)
provider_slug: integration-app
slug: integration-app-agentic-access
source_filename: integration-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/integration-app-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 63\n  by_action_class:\n    connected: 29\n    acting: 34\n  by_consequence:\n    read: 29\n    write: 31\n    safety-critical: 2\n    physical: 1\n  human_in_the_loop_required: 2\noperations:\n- path: /connections\n  method: get\n  operationId: listConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections\n  method: post\n  operationId: createConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/{id}\n  method: get\n  operationId: getConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/{id}\n  method: put\n  operationId: replaceConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/{id}\n  method: patch\n  operationId: updateConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /connections/{id}/archive\n  method: post\n  operationId: archiveConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/{id}/restore\n  method: post\n  operationId: restoreConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/{id}/refresh-credentials\n  method: post\n  operationId: refreshConnectionCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/{id}/test\n  method: post\n  operationId: testConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/{id}/logs\n  method: get\n  operationId: getConnectionLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connectors\n  method: get\n  operationId: listConnectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connectors\n  method: post\n\
  \  operationId: createConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/{id}\n  method: get\n  operationId: getConnector\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connectors/{id}\n  method: put\n  operationId: replaceConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/{id}\n  method: patch\n  operationId: updateConnector\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/{id}\n  method: delete\n  operationId: deleteConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connectors/{id}/publish\n  method: post\n  operationId: publishConnector\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: listCustomers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: put\n  operationId: replaceCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}\n  method: patch\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}\n  method: delete\n  operationId: deleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations\n  method: get\n  operationId: listIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations\n  method:\
  \ post\n  operationId: createIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/{selector}\n  method: get\n  operationId: getIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions\n  method: get\n  operationId: listActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions\n  method: post\n  operationId: createAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/{selector}\n  method: get\n  operationId: getAction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /actions/{selector}\n  method: put\n  operationId: replaceAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /actions/{selector}\n  method: patch\n  operationId: updateAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /flows\n  method: get\n  operationId: listFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flows\n  method: post\n  operationId: createFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flows/{selector}\n  method: get\n  operationId: getFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flows/{selector}/run\n  method: post\n  operationId: runFlow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flow-runs\n  method: get\n  operationId: listFlowRuns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow-runs/{id}\n  method: get\n  operationId: getFlowRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow-runs/{id}/output\n  method: get\n  operationId: getFlowRunOutput\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flow-runs/{id}/stop\n  method: post\n  operationId: stopFlowRun\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /data-collections/{connectionId}/{collectionName}/records\n  method: get\n  operationId: listDataCollectionRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-collections/{connectionId}/{collectionName}/records\n  method: post\n  operationId: createDataCollectionRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-collections/{connectionId}/{collectionName}/records/{id}\n  method: get\n  operationId: getDataCollectionRecord\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-collections/{connectionId}/{collectionName}/records/{id}\n  method: put\n  operationId: updateDataCollectionRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-collections/{connectionId}/{collectionName}/records/{id}\n  method: delete\n  operationId: deleteDataCollectionRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /field-mappings\n  method: get\n  operationId: listFieldMappings\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /field-mappings\n  method: post\n  operationId: createFieldMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /field-mappings/{selector}\n  method: get\n  operationId: getFieldMapping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app-event-subscriptions\n  method: get\n  operationId: listAppEventSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app-event-subscriptions/{id}\n  method: get\n  operationId: getAppEventSubscription\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external-event-subscriptions/{id}/subscribe\n  method: post\n  operationId: subscribeExternalEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external-event-subscriptions/{id}/unsubscribe\n  method: post\n  operationId: unsubscribeExternalEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external-api-logs\n  method: get\n  operationId: listExternalApiLogs\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external-api-logs/{id}\n  method: get\n  operationId: getExternalApiLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{id}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{id}/message\n  method: post\n  operationId: sendSessionMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{id}/stop\n  method: post\n  operationId: stopSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /search/keyword\n  method: post\n  operationId: keywordSearch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/semantic\n  method: post\n  operationId: semanticSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/apps\n  method: get\n  operationId: listPublicApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/connectors\n  method: get\n  operationId: listPublicConnectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/packages\n  method: get\n  operationId: listPublicPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/integration-app/refs/heads/main/agentic-access/integration-app-agentic-access.yml
summary_line: 63 operations · 34 acting · 2 human-in-the-loop
tags:
- Agentic Integrations
- AI Agents
- Connectors
- Embedded Integrations
- Embedded iPaaS
- Integration Marketplace
- MCP
- Model Context Protocol
- Self-Hosting
- Unified API
---
