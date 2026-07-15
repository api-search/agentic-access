---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 10
api_specs:
- filename: hologram-openapi.yml
  format: yaml
  label: Hologram Devices & SIMs API
  slug: hologram-devices-sims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-openapi.yml
- filename: hologram-openapi.yml
  format: yaml
  label: Hologram Data Usage API
  slug: hologram-data-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-openapi.yml
- filename: hologram-openapi.yml
  format: yaml
  label: Hologram SMS & Messaging API
  slug: hologram-sms-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-openapi.yml
- filename: hologram-openapi.yml
  format: yaml
  label: Hologram Plans API
  slug: hologram-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-openapi.yml
- filename: hologram-openapi.yml
  format: yaml
  label: Hologram Tags API
  slug: hologram-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-openapi.yml
- filename: hologram-openapi.yml
  format: yaml
  label: Hologram Webhooks API
  slug: hologram-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/openapi/hologram-openapi.yml
consequence_counts:
  physical: 3
  read: 10
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hologram Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /devices/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /devices/messages/{deviceid}/{webhookguid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/incoming
operation_count: 23
overview: 'Hologram exposes 23 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 10 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hologram
provider_slug: hologram
slug: hologram-agentic-access
source_filename: hologram-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hologram-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 10\n    acting: 13\n  by_consequence:\n    read: 10\n    write: 10\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /devices\n  method: get\n  operationId: listDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{deviceid}\n  method: get\n  operationId: getDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{deviceid}\n\
  \  method: put\n  operationId: updateDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{deviceid}/state\n  method: post\n  operationId: setDeviceState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/tags\n  method: get\n  operationId: listDeviceTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/tags\n  method: post\n  operationId: createDeviceTag\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/tags/{tagid}\n  method: delete\n  operationId: deleteDeviceTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/tags/{tagid}/link\n  method: post\n  operationId: linkDeviceTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/tags/{tagid}/unlink\n  method:\
  \ post\n  operationId: unlinkDeviceTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /links/cellular\n  method: get\n  operationId: listCellularLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /links/cellular/{linkid}\n  method: get\n  operationId: getCellularLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /links/cellular/sim_{iccid}/claim\n  method: post\n  operationId: claimSim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /links/cellular/bulkclaim\n  method: post\n  operationId: bulkClaimSims\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /links/cellular/{linkid}/state\n  method: post\n  operationId: setCellularLinkState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /links/cellular/{linkid}/changeplan\n  method: post\n  operationId: changeCellularLinkPlan\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usage/data\n  method: get\n  operationId: listDataUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage/data/daily\n  method: get\n  operationId: listDailyDataUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage/sms\n  method: get\n  operationId: listSmsUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/incoming\n  method: post\n  operationId: sendSmsToDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/messages\n  method: post\n  operationId: sendCloudMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/messages/{deviceid}/{webhookguid}\n  method: post\n  operationId: sendWebhookMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans/{planid}\n  method: get\n  operationId: getPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hologram/refs/heads/main/agentic-access/hologram-agentic-access.yml
summary_line: 23 operations · 13 acting
tags:
- IoT
- Cellular
- Connectivity
- SIM
- M2M
---
