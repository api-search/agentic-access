---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 21
api_specs:
- filename: onfleet-tasks-api-openapi.yml
  format: yaml
  label: Onfleet Tasks API
  slug: onfleet-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-tasks-api-openapi.yml
- filename: onfleet-workers-api-openapi.yml
  format: yaml
  label: Onfleet Workers API
  slug: onfleet-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-workers-api-openapi.yml
- filename: onfleet-route-plans-api-openapi.yml
  format: yaml
  label: Onfleet Route Plans API
  slug: onfleet-route-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-route-plans-api-openapi.yml
- filename: onfleet-orders-api-openapi.yml
  format: yaml
  label: Onfleet Orders API
  slug: onfleet-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-orders-api-openapi.yml
- filename: onfleet-organizations-api-openapi.yml
  format: yaml
  label: Onfleet Organizations & Teams API
  slug: onfleet-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-organizations-api-openapi.yml
- filename: onfleet-recipients-api-openapi.yml
  format: yaml
  label: Onfleet Recipients API
  slug: onfleet-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-recipients-api-openapi.yml
- filename: onfleet-destinations-api-openapi.yml
  format: yaml
  label: Onfleet Destinations API
  slug: onfleet-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-destinations-api-openapi.yml
- filename: onfleet-webhooks-api-openapi.yml
  format: yaml
  label: Onfleet Webhooks API
  slug: onfleet-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/openapi/onfleet-webhooks-api-openapi.yml
consequence_counts:
  physical: 6
  read: 21
  safety-critical: 1
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Onfleet Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /teams/dispatch/{teamId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /taskOrders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /taskOrders/clone
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /taskOrders/quote
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /taskOrders/{orderShortId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /taskOrders/{orderShortId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /taskOrders/{orderShortId}/reject
operation_count: 54
overview: 'Onfleet exposes 54 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 26 write, 6 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Onfleet
provider_slug: onfleet
slug: onfleet-agentic-access
source_filename: onfleet-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/onfleet-destinations-api-openapi.yml, openapi/onfleet-orders-api-openapi.yml,\n  openapi/onfleet-organizations-api-openapi.yml, openapi/onfleet-recipients-api-openapi.yml,\n  openapi/onfleet-route-plans-api-openapi.yml, openapi/onfleet-tasks-api-openapi.yml, openapi/onfleet-webhooks-api-openapi.yml,\n  openapi/onfleet-workers-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    acting: 33\n    connected: 21\n  by_consequence:\n    write: 26\n    read: 21\n    physical: 6\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /destinations\n  method: post\n  operationId: createDestination\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /destinations/{destinationId}\n  method: get\n  operationId: getDestination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /taskOrders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /taskOrders/{orderShortId}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /taskOrders/{orderShortId}\n  method: put\n  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /taskOrders/{orderShortId}/cancel\n  method: post\n  operationId: cancelOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /taskOrders/{orderShortId}/reject\n  method: post\n  operationId: rejectOrder\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /taskOrders/clone\n  method: post\n  operationId: cloneOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /taskOrders/quote\n  method: post\n  operationId: quoteOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization\n  method: get\n  operationId: getOwnOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}\n  method: get\n  operationId: getDelegateeOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admins\n  method: get\n  operationId: listAdmins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admins\n  method: post\n  operationId: createAdmin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /teams\n  method: post\n  operationId: createTeam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /teams/dispatch/{teamId}\n  method: post\n  operationId: teamAutoDispatch\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /recipients\n  method: post\n  operationId: createRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recipients/{recipientId}\n  method: get\n  operationId: getRecipient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipients/{recipientId}\n  method: put\n  operationId: updateRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /recipients/name/{name}\n  method: get\n  operationId: getRecipientByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recipients/phone/{phone}\n  method: get\n  operationId: getRecipientByPhone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routePlans\n  method: get\n  operationId: listRoutePlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routePlans\n  method: post\n  operationId: createRoutePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /routePlans/{routePlanId}\n  method: get\n  operationId: getRoutePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routePlans/{routePlanId}\n  method: put\n  operationId: updateRoutePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /routePlans/{routePlanId}\n  method: delete\n  operationId: deleteRoutePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /routePlans/{routePlanId}/tasks\n\
  \  method: put\n  operationId: addTasksToRoutePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /optimizations/scheduled\n  method: post\n  operationId: initializeOptimization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /optimizations/{optimizationId}/start\n  method: post\n  operationId: startOptimization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /optimizations/{optimizationId}/status\n  method: get\n  operationId: getOptimizationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /optimizations/{optimizationId}/apply\n  method: post\n  operationId: applyOptimization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /optimizations/{optimizationId}/abort\n  method: post\n  operationId: abortOptimization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /tasks\n  method: post\n  operationId: createTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/batch\n  method: post\n  operationId: createTaskBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/all\n  method: get\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{taskId}\n  method: get\n  operationId:\
  \ getTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{taskId}\n  method: put\n  operationId: updateTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{taskId}\n  method: delete\n  operationId: deleteTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/shortId/{shortId}\n  method: get\n  operationId: getTaskByShortId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{taskId}/clone\n  method: post\n  operationId: cloneTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{taskId}/complete\n  method: post\n  operationId: forceCompleteTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /containers/workers/{workerId}\n  method: put\n  operationId: assignTasksToWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/secret\n  method: get\n  operationId: getWebhookSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers\n  method: get\n  operationId: listWorkers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers\n  method: post\n  operationId: createWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{workerId}\n  method: get\n  operationId: getWorker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{workerId}\n  method: put\n  operationId: updateWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{workerId}\n  method: delete\n  operationId: deleteWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{workerId}/tasks\n  method: get\n  operationId: listWorkerAssignedTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{workerId}/deliveryManifest\n  method: get\n  operationId: getDeliveryManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onfleet/refs/heads/main/agentic-access/onfleet-agentic-access.yml
summary_line: 54 operations · 33 acting · 1 human-in-the-loop
tags:
- Last Mile Delivery
- Logistics
- Fleet Management
- Dispatch
- Route Optimization
- Courier
- Drivers
- Tracking
- Geocoding
- Webhooks
- AI
- SaaS
---
