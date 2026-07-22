---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 30
api_specs:
- filename: overflow-openapi-original.json
  format: json
  label: Overflow Open API
  slug: overflow-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/openapi/overflow-openapi-original.json
consequence_counts:
  read: 30
  safety-critical: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 8
kind: agentic-access
layout: agentic-access
method: generated
name: Overflow Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v3/contributions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v3/contributions/{contributionId}/initiate-refund
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v3/donors
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v3/donors/{donorId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v3/payments/authorize
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v3/subscriptions/{donorId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v3/subscriptions/{donorId}/{subscriptionId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v3/subscriptions/{donorId}/{subscriptionId}
operation_count: 38
overview: 'Overflow exposes 38 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read and 8 safety-critical.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Overflow
provider_slug: overflow
slug: overflow-agentic-access
source_filename: overflow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/overflow-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 30\n    acting: 8\n  by_consequence:\n    read: 30\n    safety-critical: 8\n  human_in_the_loop_required: 8\noperations:\n- path: /api/v3/contributions\n  method: get\n  operationId: OpenApiContributionsController_getContributions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/contributions\n  method: post\n  operationId: OpenApiContributionsController_chargeCashPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v3/contributions/{contributionId}\n  method: get\n  operationId: OpenApiContributionsController_getContributionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/contributions/{contributionId}/initiate-refund\n  method: post\n  operationId: OpenApiContributionsController_initiateRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v3/deposits\n  method:\
  \ get\n  operationId: OpenApiDepositsController_getDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/deposits/{depositId}\n  method: get\n  operationId: OpenApiDepositsController_getDepositById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/deposits/{depositId}/summary\n  method: get\n  operationId: OpenApiDepositsController_getDepositSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/refunds\n  method: get\n  operationId: OpenApiRefundsController_getRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/refunds/{refundId}\n\
  \  method: get\n  operationId: OpenApiRefundsController_getRefundById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/chargebacks\n  method: get\n  operationId: OpenApiChargebacksController_getChargebacks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/chargebacks/{chargebackId}\n  method: get\n  operationId: OpenApiChargebacksController_getChargebackById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/webhooks\n  method: get\n  operationId: OpenApiWebhooksController_getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/webhooks/{webhookId}\n\
  \  method: get\n  operationId: OpenApiWebhooksController_getWebhookById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/webhooks/{webhookId}/event-logs\n  method: get\n  operationId: OpenApiWebhooksController_getWebhookEventLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/donors\n  method: get\n  operationId: OpenApiDonorProfilesController_getDonorProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/donors\n  method: post\n  operationId: OpenApiDonorProfilesController_createDonorProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n\
  \      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v3/donors/{donorId}\n  method: get\n  operationId: OpenApiDonorProfilesController_getDonorProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/donors/{donorId}\n  method: patch\n  operationId: OpenApiDonorProfilesController_updateDonorProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v3/subscriptions/{donorId}\n  method: post\n  operationId: OpenApiSubscriptionsController_createSubscription\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v3/subscriptions/{donorId}\n  method: get\n  operationId: OpenApiSubscriptionsController_getSubscriptionsByDonorProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/subscriptions\n  method: get\n  operationId: OpenApiSubscriptionsController_getSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/subscriptions/{donorId}/{subscriptionId}\n  method: get\n  operationId: OpenApiSubscriptionsController_getSubscriptionById\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/subscriptions/{donorId}/{subscriptionId}\n  method: patch\n  operationId: OpenApiSubscriptionsController_updateSubscriptionById\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v3/subscriptions/{donorId}/{subscriptionId}\n  method: delete\n  operationId: OpenApiSubscriptionsController_cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /api/v3/payment-methods/{donorId}\n  method: get\n  operationId: OpenApiPaymentMethodsController_getPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/campaigns\n  method: get\n  operationId: OpenApiCampaignsController_getCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/campaigns/{campaignId}\n  method: get\n  operationId: OpenApiCampaignsController_getCampaignById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/locations\n  method: get\n  operationId: OpenApiLocationsController_getLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v3/locations/{locationId}\n  method: get\n  operationId: OpenApiLocationsController_getLocationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/payments/authorize\n  method: post\n  operationId: OpenApiPaymentsController_authorizePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v3/tap/destinations\n  method: get\n  operationId: OpenApiTapDestinationsController_getDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/tap/destinations/{destinationId}\n\
  \  method: get\n  operationId: OpenApiTapDestinationsController_getDestinationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/tap/devices\n  method: get\n  operationId: OpenApiTapDevicesController_getDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/tap/devices/{deviceId}\n  method: get\n  operationId: OpenApiTapDevicesController_getDeviceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/tap/events\n  method: get\n  operationId: OpenApiTapEventsController_getEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/tap/groups\n\
  \  method: get\n  operationId: OpenApiTapGroupsController_getGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/tap/groups/{groupId}\n  method: get\n  operationId: OpenApiTapGroupsController_getGroupById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/health\n  method: get\n  operationId: OpenApiController_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overflow/refs/heads/main/agentic-access/overflow-agentic-access.yml
summary_line: 38 operations · 8 acting · 8 human-in-the-loop
tags:
- Company
- Fintech
- Payments
- Donations
- Fundraising
- Nonprofit
- Giving
- Recurring Payments
- Webhooks
- Cryptocurrency
---
