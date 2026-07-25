---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 10
api_specs:
- filename: customerio-broadcasts-api-openapi.yml
  format: yaml
  label: Customer.io Broadcasts API
  slug: customerio-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-broadcasts-api-openapi.yml
- filename: customerio-campaigns-api-openapi.yml
  format: yaml
  label: Customer.io Campaigns API
  slug: customerio-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-campaigns-api-openapi.yml
- filename: customerio-collections-api-openapi.yml
  format: yaml
  label: Customer.io Collections API
  slug: customerio-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-collections-api-openapi.yml
- filename: customerio-customers-api-openapi.yml
  format: yaml
  label: Customer.io Customers API
  slug: customerio-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-customers-api-openapi.yml
- filename: customerio-devices-api-openapi.yml
  format: yaml
  label: Customer.io Devices API
  slug: customerio-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-devices-api-openapi.yml
- filename: customerio-events-api-openapi.yml
  format: yaml
  label: Customer.io Events API
  slug: customerio-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-events-api-openapi.yml
- filename: customerio-exports-api-openapi.yml
  format: yaml
  label: Customer.io Exports API
  slug: customerio-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-exports-api-openapi.yml
- filename: customerio-messages-api-openapi.yml
  format: yaml
  label: Customer.io Messages API
  slug: customerio-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-messages-api-openapi.yml
- filename: customerio-people-api-openapi.yml
  format: yaml
  label: Customer.io People API
  slug: customerio-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-people-api-openapi.yml
- filename: customerio-pipelines-api-openapi.yml
  format: yaml
  label: Customer.io Pipelines API
  slug: customerio-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-pipelines-api-openapi.yml
- filename: customerio-segments-api-openapi.yml
  format: yaml
  label: Customer.io Segments API
  slug: customerio-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-segments-api-openapi.yml
- filename: customerio-track-v2-api-openapi.yml
  format: yaml
  label: Customer.io Track v2 API
  slug: customerio-track-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-track-v2-api-openapi.yml
- filename: customerio-transactional-api-openapi.yml
  format: yaml
  label: Customer.io Transactional API
  slug: customerio-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-transactional-api-openapi.yml
consequence_counts:
  physical: 4
  read: 10
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Customerio Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/send/broadcast
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/send/email
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/send/push
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/send/sms
operation_count: 35
overview: 'Customer.io exposes 35 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 21 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Customer.io
provider_slug: customerio
slug: customerio-agentic-access
source_filename: customerio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/customerio-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    acting: 25\n    connected: 10\n  by_consequence:\n    write: 21\n    physical: 4\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/customers/{identifier}\n  method: put\n  operationId: identifyCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{identifier}\n  method: delete\n  operationId: deleteCustomer\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/events\n  method: post\n  operationId: trackAnonymousEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{identifier}/events\n  method: post\n  operationId: trackCustomerEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/customers/{identifier}/devices\n  method: put\n  operationId: addDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customers/{identifier}/devices/{device_id}\n  method: delete\n  operationId: deleteDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/segments/{segment_id}/add_customers\n  method: post\n  operationId: addCustomersToSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/segments/{segment_id}/remove_customers\n  method: post\n  operationId: removeCustomersFromSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/entity\n  method: post\n  operationId: trackEntityV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/batch\n  method: post\n  operationId: trackBatchV2\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/send/email\n  method: post\n  operationId: sendTransactionalEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/send/push\n  method: post\n  operationId: sendTransactionalPush\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /v1/send/sms\n  method: post\n  operationId: sendTransactionalSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/send/broadcast\n  method: post\n  operationId: triggerBroadcast\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers\n  method: post\n  operationId: searchCustomers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer_id}/attributes\n  method: get\n  operationId: getCustomerAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customer_id}/segments\n  method: get\n  operationId: getCustomerSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customer_id}/messages\n  method: get\n  operationId: getCustomerMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/segments\n  method: get\n  operationId: listSegments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/segments\n  method: post\n  operationId: createSegment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns/{campaign_id}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns/{campaign_id}/metrics\n  method: get\n  operationId: getCampaignMetrics\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exports/customers\n  method: post\n  operationId: exportCustomers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/exports\n  method: get\n  operationId: listExports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collections\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/collections\n  method: post\n  operationId: createCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/identify\n  method: post\n  operationId: pipelinesIdentify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/track\n  method: post\n  operationId: pipelinesTrack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/page\n  method: post\n  operationId: pipelinesPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/screen\n  method: post\n  operationId: pipelinesScreen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/group\n  method: post\n  operationId: pipelinesGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alias\n  method: post\n  operationId: pipelinesAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch\n  method: post\n  operationId: pipelinesBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/agentic-access/customerio-agentic-access.yml
summary_line: 35 operations · 25 acting
tags:
- Customer Messaging
- Marketing Automation
- Email
- CDP
- Transactional
---
