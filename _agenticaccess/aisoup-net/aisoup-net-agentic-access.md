---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 9
api_specs:
- filename: aisoup-net-commerce-api-openapi.yml
  format: yaml
  label: aisoup-net Commerce API
  slug: aisoup-net-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisoup-net/openapi/aisoup-net-commerce-api-openapi.yml
- filename: aisoup-net-contact-api-openapi.yml
  format: yaml
  label: aisoup-net Contact API
  slug: aisoup-net-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisoup-net/openapi/aisoup-net-contact-api-openapi.yml
- filename: aisoup-net-contractor-check-api-openapi.yml
  format: yaml
  label: aisoup-net Contractor Check API
  slug: aisoup-net-contractor-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisoup-net/openapi/aisoup-net-contractor-check-api-openapi.yml
- filename: aisoup-net-discovery-api-openapi.yml
  format: yaml
  label: aisoup-net Discovery API
  slug: aisoup-net-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisoup-net/openapi/aisoup-net-discovery-api-openapi.yml
- filename: aisoup-net-evidence-snapshots-api-openapi.yml
  format: yaml
  label: aisoup-net Evidence Snapshots API
  slug: aisoup-net-evidence-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisoup-net/openapi/aisoup-net-evidence-snapshots-api-openapi.yml
- filename: aisoup-net-photo-scout-api-openapi.yml
  format: yaml
  label: aisoup-net Photo Scout API
  slug: aisoup-net-photo-scout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisoup-net/openapi/aisoup-net-photo-scout-api-openapi.yml
- filename: aisoup-net-status-api-openapi.yml
  format: yaml
  label: aisoup-net Status API
  slug: aisoup-net-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisoup-net/openapi/aisoup-net-status-api-openapi.yml
- filename: aisoup-net-support-api-openapi.yml
  format: yaml
  label: aisoup-net Support API
  slug: aisoup-net-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisoup-net/openapi/aisoup-net-support-api-openapi.yml
- filename: aisoup-net-web-evidence-api-openapi.yml
  format: yaml
  label: aisoup-net Web Evidence API
  slug: aisoup-net-web-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisoup-net/openapi/aisoup-net-web-evidence-api-openapi.yml
consequence_counts:
  physical: 1
  read: 9
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aisoup Net Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/receipts/{order_id}/verify
operation_count: 22
overview: 'aisoup-net exposes 22 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: aisoup-net
provider_slug: aisoup-net
slug: aisoup-net-agentic-access
source_filename: aisoup-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/aisoup-net-contractor-check-openapi.json, openapi/aisoup-net-platform-openapi.json,\n  openapi/aisoup-net-web-evidence-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 13\n    connected: 9\n  by_consequence:\n    write: 12\n    read: 9\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /contractor-check/v1/check\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/contact/messages\n\
  \  method: post\n  operationId: create_contact_message_v1_contact_messages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /support/v1/tickets\n  method: post\n  operationId: create_support_ticket_support_v1_tickets_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /support/v1/tickets/{ticket_id}\n  method: get\n  operationId: get_support_ticket_support_v1_tickets__ticket_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /support/v1/tickets/{ticket_id}/messages\n  method: post\n  operationId: add_support_ticket_message_support_v1_tickets__ticket_id__messages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status/index.json\n  method: get\n  operationId: public_status_json_status_index_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/feed.rss\n  method: get\n  operationId: public_status_feed_status_feed_rss_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/v1/subscriptions\n  method: post\n  operationId:\
  \ create_status_subscription_status_v1_subscriptions_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/services\n  method: get\n  operationId: service_catalog_v1_services_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web-evidence/v1/claims/verify/quick\n  method: post\n  operationId: verifyClaimQuick\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web-evidence/v1/claims/verify\n  method: post\n  operationId:\
  \ verifyClaimStandard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web-evidence/v1/claims/verify/deep\n  method: post\n  operationId: verifyClaimDeep\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /web-evidence/v1/claims/verify/research\n  method: post\n  operationId: verifyClaimResearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /contractor-check/v1/check\n  method: post\n  operationId: checkC10ContractorLicense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /photo-scout/v1/discover\n  method: post\n  operationId: discoverPhotoSpots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/url-snapshots/{snapshot_id}\n  method: get\n  operationId: getEvidenceSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /v1/url-snapshots/{snapshot_id}/content\n  method: get\n  operationId: getEvidenceSnapshotContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/quotes\n  method: post\n  operationId: createVerificationQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{order_id}\n  method: get\n  operationId: getOrderByAccessToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer/orders\n  method: get\n  operationId: listCustomerOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer/orders/{order_id}\n  method: get\n  operationId: getCustomerOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/receipts/{order_id}/verify\n  method: post\n  operationId: verifyOrderReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/aisoup-net/agentic-access/aisoup-net-agentic-access.yml
summary_line: 22 operations · 13 acting
tags:
- Artificial Intelligence
- Agents
- Platform
- Workflows
- LLM
---
