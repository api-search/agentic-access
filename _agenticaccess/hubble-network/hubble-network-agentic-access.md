---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 20
api_specs:
- filename: hubble-network-api-keys-api-openapi.yml
  format: yaml
  label: Hubble Network API Keys API
  slug: hubble-network-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-api-keys-api-openapi.yml
- filename: hubble-network-billing-api-openapi.yml
  format: yaml
  label: Hubble Network Billing API
  slug: hubble-network-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-billing-api-openapi.yml
- filename: hubble-network-devices-api-openapi.yml
  format: yaml
  label: Hubble Network Devices API
  slug: hubble-network-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-devices-api-openapi.yml
- filename: hubble-network-organizations-api-openapi.yml
  format: yaml
  label: Hubble Network Organizations API
  slug: hubble-network-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-organizations-api-openapi.yml
- filename: hubble-network-packet-webhooks-api-openapi.yml
  format: yaml
  label: Hubble Network Packet Webhooks API
  slug: hubble-network-packet-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-packet-webhooks-api-openapi.yml
- filename: hubble-network-packets-api-openapi.yml
  format: yaml
  label: Hubble Network Packets API
  slug: hubble-network-packets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-packets-api-openapi.yml
- filename: hubble-network-platform-metrics-api-openapi.yml
  format: yaml
  label: Hubble Network Platform Metrics API
  slug: hubble-network-platform-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/openapi/hubble-network-platform-metrics-api-openapi.yml
consequence_counts:
  physical: 2
  read: 20
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hubble Network Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/org/{org_id}/key
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/org/{org_id}/webhooks/{webhook_id}/test
operation_count: 39
overview: 'Hubble Network exposes 39 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 17 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hubble Network
provider_slug: hubble-network
slug: hubble-network-agentic-access
source_filename: hubble-network-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: generated\nsource: openapi/hubble-network-platform-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    connected: 20\n    acting: 19\n  by_consequence:\n    read: 20\n    physical: 2\n    write: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/org/{org_id}/check\n  method: get\n  operationId: validate-api-key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/key\n  method: post\n  operationId: provision-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/key\n  method: get\n  operationId: list-api-keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/key/{key_id}\n  method: delete\n  operationId: delete-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/key/{key_id}\n  method: patch\n  operationId: update-api-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/key_scopes\n  method: get\n  operationId: list-key-scopes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}\n  method: patch\n  operationId: update-organization-metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}\n  method: get\n  operationId: retrieve-organization-metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/org/{org_id}/devices\n\
  \  method: post\n  operationId: register-new-devices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/devices\n  method: get\n  operationId: list-devices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/devices\n  method: patch\n  operationId: batch-update-devices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/devices\n  method: delete\n  operationId: batch-delete-devices\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/devices/{device_id}\n  method: get\n  operationId: get-device\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/devices/{device_id}\n  method: patch\n  operationId: update-device\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/devices/{device_id}\n  method: delete\n  operationId: delete-device\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/packets\n  method: get\n  operationId: retrieve-organization-packets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhook/testBatch\n  method: post\n  operationId: packet-webhook-example\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/api_metrics\n  method: get\n  operationId: get-api-metrics\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/packet_metrics\n  method: get\n  operationId: get-packet-metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/webhook_metrics\n  method: get\n  operationId: get-webhook-metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/device_metrics\n  method: get\n  operationId: get-device-metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/users\n  method: get\n  operationId: list-users-in-organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/org/{org_id}/users\n  method: post\n  operationId: add-user-to-organization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/users/{user_id}\n  method: patch\n  operationId: update-user-in-organization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/users/{user_id}\n  method: delete\n  operationId: delete-user-from-organization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/invitations\n  method: get\n  operationId: list-pending-invites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/invitations\n  method: post\n  operationId: invite-user-to-organization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/invitations\n  method: delete\n  operationId: delete-invitation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/webhooks\n  method: post\n  operationId: create-webhook-endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/webhooks\n  method: get\n  operationId: list-registered-webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/webhooks/{webhook_id}\n  method: patch\n  operationId: update-webhook-endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/webhooks/{webhook_id}\n  method: delete\n  operationId: delete-webhook-endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/webhooks/{webhook_id}/test\n  method: post\n  operationId: test-webhook-endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/org/{org_id}/billing/invoices\n  method: get\n  operationId:\
  \ get-recent-invoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/billing/invoices/{invoice_id}/pdf\n  method: get\n  operationId: get-invoice-pdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/billing/usage\n  method: get\n  operationId: get-billing-usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/billing/active-devices\n  method: get\n  operationId: get-billing-active-devices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/billing/subscription\n  method: get\n  operationId: get-billing-subscription\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/org/{org_id}/billing/payment-method\n  method: get\n  operationId: get-billing-payment-method\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubble-network/refs/heads/main/agentic-access/hubble-network-agentic-access.yml
summary_line: 39 operations · 19 acting
tags:
- Company
- IoT
- Bluetooth
- Satellite
- Connectivity
- Asset Tracking
- Devices
- Networks
- Telemetry
- Logistics
---
