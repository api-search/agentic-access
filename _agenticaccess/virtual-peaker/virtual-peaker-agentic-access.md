---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 8
api_specs:
- filename: virtual-peaker-commands-api-openapi.yml
  format: yaml
  label: Virtual Peaker Commands API
  slug: virtual-peaker-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-commands-api-openapi.yml
- filename: virtual-peaker-devices-api-openapi.yml
  format: yaml
  label: Virtual Peaker Devices API
  slug: virtual-peaker-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-devices-api-openapi.yml
- filename: virtual-peaker-energy-interval-endpoint-api-openapi.yml
  format: yaml
  label: Virtual Peaker Energy Interval Endpoint API
  slug: virtual-peaker-energy-interval-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-energy-interval-endpoint-api-openapi.yml
- filename: virtual-peaker-group-management-api-openapi.yml
  format: yaml
  label: Virtual Peaker Group Management API
  slug: virtual-peaker-group-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-group-management-api-openapi.yml
- filename: virtual-peaker-oauth-device-discovery-preferred-api-openapi.yml
  format: yaml
  label: Virtual Peaker OAuth Device Discovery (Preferred) API
  slug: virtual-peaker-oauth-device-discovery-preferred-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-oauth-device-discovery-preferred-api-openapi.yml
- filename: virtual-peaker-pairing-code-device-discovery-end-user-app-api-openapi.yml
  format: yaml
  label: Virtual Peaker Pairing Code Device Discovery - End User App API
  slug: virtual-peaker-pairing-code-device-discovery-end-user-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-pairing-code-device-discovery-end-user-app-api-openapi.yml
- filename: virtual-peaker-pairing-code-device-discovery-utility-commissioned-installation-api-openapi.yml
  format: yaml
  label: Virtual Peaker Pairing Code Device Discovery - Utility Commissioned Installation API
  slug: virtual-peaker-pairing-code-device-discovery-utility-commissioned-installation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-pairing-code-device-discovery-utility-commissioned-installation-api-openapi.yml
- filename: virtual-peaker-publishing-api-openapi.yml
  format: yaml
  label: Virtual Peaker Publishing API
  slug: virtual-peaker-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/openapi/virtual-peaker-publishing-api-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Virtual Peaker Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /command
operation_count: 23
overview: 'Virtual Peaker exposes 23 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 14 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Virtual Peaker
provider_slug: virtual-peaker
slug: virtual-peaker-agentic-access
source_filename: virtual-peaker-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/virtual-peaker-gravity-connect-device-partner-api-openapi.yml, openapi/virtual-peaker-gravity-connect-vpp-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 8\n    acting: 15\n  by_consequence:\n    read: 8\n    write: 14\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /device/{DEVICE_UID}\n  method: get\n  operationId: readDeviceDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - basic_partner_read_write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/{DEVICE_UID}/{SIGNAL_OR_SETTING}/{DATA_KEY}\n  method: put\n  operationId:\
  \ updateSignalSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - basic_partner_read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /device/{DEVICE_UID}/{SIGNAL_OR_SETTING}/{DATA_KEY}\n  method: get\n  operationId: readSignalSetting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - basic_partner_read_write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/{DEVICE_UID}/user\n  method: get\n  operationId: readDeviceUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - basic_partner_read_write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /houses\n  method: post\n  operationId: publishHouseList\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - basic_partner_read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /command\n  method: post\n  operationId: sendCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - basic_partner_read_write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /command/{COMMAND_REFERENCE_ID}\n  method: get\n  operationId: readCommandState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - basic_partner_read_write\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /command/{COMMAND_REFERENCE_ID}\n  method: delete\n  operationId: cancelCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - basic_partner_read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscription\n  method: post\n  operationId: modifySubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - basic_partner_read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - basic_partner_read_write\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group/{GROUP_ID}\n  method: get\n  operationId: readGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - basic_partner_read_write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group/{GROUP_ID}\n  method: put\n  operationId: updateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - basic_partner_read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group/{GROUP_ID}\n  method: delete\n  operationId: deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - basic_partner_read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group/{GROUP_ID}/devices\n  method: post\n  operationId: manageGroupDevices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - basic_partner_read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /command/{COMMAND_REFERENCE_ID}/opt-out\n  method: post\n  operationId: commandOptOut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - basic_partner_read_write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /devices\n  method: get\n  operationId: readCurrentUserDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user\n  method: get\n  operationId: readCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - user_read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/{DEVICE_UID}/energy\n  method: get\n  operationId: readDeviceEnergyInterval\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - basic_partner_read_write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publish/{PROGRAM_PUBLISH_KEY}/update\n  method: post\n  operationId: publishSignalSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /publish/{PROGRAM_PUBLISH_KEY}/command\n  method: post\n  operationId: publishCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /publish/{PROGRAM_PUBLISH_KEY}/command/device\n  method: post\n  operationId: publishDeviceCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /publish/{PROGRAM_PUBLISH_KEY}/device\n\
  \  method: post\n  operationId: publishDeviceEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /publish/{PROGRAM_PUBLISH_KEY}/enrollment\n  method: post\n  operationId: publishDevicePartnerDrivenEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtual-peaker/refs/heads/main/agentic-access/virtual-peaker-agentic-access.yml
summary_line: 23 operations · 15 acting
tags:
- Energy
- United States
- Utilities
- Electricity
- Grid
- Demand Response
- DER
- DERMS
- Virtual Power Plant
- EV Charging
- Smart Thermostats
- Energy Storage
---
