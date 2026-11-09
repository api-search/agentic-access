---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 15
api_specs:
- filename: coverwhaleinsurancesolutions-authentication-api-openapi.yml
  format: yaml
  label: Cover Whale Authentication API
  slug: coverwhaleinsurancesolutions-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-authentication-api-openapi.yml
- filename: coverwhaleinsurancesolutions-binding-api-openapi.yml
  format: yaml
  label: Cover Whale Binding API
  slug: coverwhaleinsurancesolutions-binding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-binding-api-openapi.yml
- filename: coverwhaleinsurancesolutions-policy-lifecycle-api-openapi.yml
  format: yaml
  label: Cover Whale Policy Lifecycle API
  slug: coverwhaleinsurancesolutions-policy-lifecycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-policy-lifecycle-api-openapi.yml
- filename: coverwhaleinsurancesolutions-quoting-api-openapi.yml
  format: yaml
  label: Cover Whale Quoting API
  slug: coverwhaleinsurancesolutions-quoting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-quoting-api-openapi.yml
- filename: coverwhaleinsurancesolutions-reference-data-api-openapi.yml
  format: yaml
  label: Cover Whale Reference Data API
  slug: coverwhaleinsurancesolutions-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-reference-data-api-openapi.yml
- filename: coverwhaleinsurancesolutions-submission-data-api-openapi.yml
  format: yaml
  label: Cover Whale Submission Data API
  slug: coverwhaleinsurancesolutions-submission-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-submission-data-api-openapi.yml
- filename: coverwhaleinsurancesolutions-submissions-api-openapi.yml
  format: yaml
  label: Cover Whale Submissions API
  slug: coverwhaleinsurancesolutions-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-submissions-api-openapi.yml
- filename: coverwhaleinsurancesolutions-webhooks-api-openapi.yml
  format: yaml
  label: Cover Whale Webhooks API
  slug: coverwhaleinsurancesolutions-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 15
  safety-critical: 1
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Coverwhaleinsurancesolutions Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /password-reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sendQuoteRequest
operation_count: 43
overview: 'Cover Whale exposes 43 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 26 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cover Whale
provider_slug: coverwhaleinsurancesolutions
slug: coverwhaleinsurancesolutions-agentic-access
source_filename: coverwhaleinsurancesolutions-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/coverwhaleinsurancesolutions-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 15\n    acting: 28\n  by_consequence:\n    read: 15\n    physical: 1\n    write: 26\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sendQuoteRequest\n  method: post\n  operationId: sendQuoteRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authentication\n  method: post\n  operationId: authentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /password-reset\n  method: get\n  operationId: getPasswordReset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /password-reset\n  method: post\n  operationId: postPasswordReset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /commodityList\n  method: get\n  operationId: getCommodityList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coverage/guidelines\n  method: get\n  operationId: getCoverageGuidelines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quote\n  method: post\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indication\n  method: post\n  operationId: getIndication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /submission/pre-screen/{dotNumber}\n  method: get\n  operationId: preScreenDot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submission/{displayId}\n  method: get\n  operationId: getSubmissionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submission/tax-calculations\n  method: post\n  operationId: calculateTaxesAndFees\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/transactions\n  method: get\n  operationId: getSubmissionTransactions\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submission/{displayId}/public-reply\n  method: post\n  operationId: postSubmissionPublicReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-subscriptions\n  method: get\n  operationId: listWebhookSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook-subscriptions\n  method: post\n  operationId: createWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-subscriptions/{id}\n  method: get\n  operationId: getWebhookSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook-subscriptions/{id}\n  method: put\n  operationId: updateWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-subscriptions/{id}\n  method: delete\n  operationId: deleteWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-subscriptions/{id}/rotate-secret\n  method: post\n  operationId: rotateWebhookSubscriptionSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bind/{displayId}\n  method: put\n  operationId: bindRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/notes/{id}\n  method: get\n  operationId: getSubmissionNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /submission/{displayId}/{transactionId}\n  method: put\n  operationId: updateSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/details\n  method: get\n  operationId: getSubmissionDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submission/{displayId}/{transactionId}/documents/{type}\n  method: get\n  operationId: downloadDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submission/{displayId}/{transactionId}/recalculate-rates\n\
  \  method: post\n  operationId: recalculateRates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/taxes-fees\n  method: get\n  operationId: getTaxesAndFees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submission/{displayId}/{transactionId}/vehicle\n  method: post\n  operationId: addVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/vehicle/{vehicleId}\n\
  \  method: put\n  operationId: updateVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/vehicle/{vehicleId}\n  method: delete\n  operationId: removeVehicle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/driver\n  method: post\n  operationId: addDriver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/driver/{driverId}\n  method: put\n  operationId: updateDriver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/driver/{driverId}\n  method: delete\n  operationId: removeDriver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/trailer\n  method: post\n  operationId: addTrailer\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/trailer/{trailerId}\n  method: delete\n  operationId: removeTrailer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/quote-endorsement\n  method: post\n  operationId: quoteEndorsement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /submission/{displayId}/{transactionId}/endorsement\n  method: post\n  operationId: createEndorsement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/cancel-request\n  method: post\n  operationId: cancelRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/cancel-approve\n  method: post\n  operationId: cancelApprove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/cancel\n  method: post\n  operationId: cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/reinstatement\n  method: post\n  operationId: reinstatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/non-renewal\n  method: post\n\
  \  operationId: nonRenewal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{displayId}/{transactionId}/decline\n  method: post\n  operationId: declineSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/coverwhaleinsurancesolutions/agentic-access/coverwhaleinsurancesolutions-agentic-access.yml
summary_line: 43 operations · 28 acting · 1 human-in-the-loop
tags:
- Insurance
- Commercial Auto Insurance
- Insurtech
- Underwriting
- Telematics
- Risk Management
- Fleet Safety
- Policy Lifecycle
- Webhook
- Company
---
