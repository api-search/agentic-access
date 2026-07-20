---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 8
api_specs:
- filename: augment-openapi-original.json
  format: json
  label: Augment API
  slug: augment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/openapi/augment-openapi-original.json
consequence_counts:
  read: 8
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Augment Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Augment exposes 23 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Augment
provider_slug: augment
slug: augment-agentic-access
source_filename: augment-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/augment-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 15\n    connected: 8\n  by_consequence:\n    write: 15\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/auth-check\n  method: post\n  operationId: verifyApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/loads\n  method: get\n  operationId: getLoad\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/loads\n  method: post\n  operationId: createOrUpdateLoad\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/loads\n  method: patch\n  operationId: patchLoad\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/loads/tracking\n  method: post\n  operationId: addTrackingEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carrier-issues/external-ref\n  method: post\n  operationId: reportCarrierIssueExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/carriers\n  method: post\n  operationId: createOrUpdateCarrier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/carriers\n  method: get\n  operationId: getCarrierByIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n   \
  \ subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/carriers/bulk\n  method: post\n  operationId: bulkUpsertCarriers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/carriers/{carrierId}\n  method: get\n  operationId: getCarrierById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/carriers/{carrierId}\n  method: delete\n  operationId: archiveCarrier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v2/webhook-endpoints\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhook-endpoints\n  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhook-endpoints/{webhookEndpointId}\n  method: get\n  operationId: getWebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhook-endpoints/{webhookEndpointId}\n  method: patch\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhook-endpoints/{webhookEndpointId}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhook-event-types\n  method: get\n  operationId: listWebhookEventTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhook-subscriptions\n  method: get\n  operationId: listWebhookSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhook-subscriptions\n  method: post\n  operationId: createWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhook-subscriptions/{subscriptionId}\n  method: get\n  operationId: getWebhookSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhook-subscriptions/{subscriptionId}\n  method: patch\n  operationId: updateWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhook-subscriptions/{subscriptionId}\n  method: delete\n  operationId: deleteWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhook-subscriptions/{subscriptionId}/test\n  method: post\n  operationId: testWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/agentic-access/augment-agentic-access.yml
summary_line: 23 operations · 15 acting
tags:
- Company
- Logistics
- Freight
- Supply Chain
- Transportation
- Webhooks
- Artificial Intelligence
- Automation
---
