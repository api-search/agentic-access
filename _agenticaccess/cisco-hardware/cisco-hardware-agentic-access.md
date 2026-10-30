---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: cisco-hardware-devices-api-openapi.yml
  format: yaml
  label: Cisco Hardware Devices API
  slug: cisco-hardware-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-devices-api-openapi.yml
- filename: cisco-hardware-administered-api-openapi.yml
  format: yaml
  label: Cisco Hardware Administered API
  slug: cisco-hardware-administered-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-administered-api-openapi.yml
- filename: cisco-hardware-appliance-api-openapi.yml
  format: yaml
  label: Cisco Hardware Appliance API
  slug: cisco-hardware-appliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-appliance-api-openapi.yml
- filename: cisco-hardware-camera-api-openapi.yml
  format: yaml
  label: Cisco Hardware Camera API
  slug: cisco-hardware-camera-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-camera-api-openapi.yml
- filename: cisco-hardware-campusgateway-api-openapi.yml
  format: yaml
  label: Cisco Hardware Campus Gateway API
  slug: cisco-hardware-campusgateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-campusgateway-api-openapi.yml
- filename: cisco-hardware-cellulargateway-api-openapi.yml
  format: yaml
  label: Cisco Hardware Cellular Gateway API
  slug: cisco-hardware-cellulargateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-cellulargateway-api-openapi.yml
- filename: cisco-hardware-insight-api-openapi.yml
  format: yaml
  label: Cisco Hardware Insight API
  slug: cisco-hardware-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-insight-api-openapi.yml
- filename: cisco-hardware-licensing-api-openapi.yml
  format: yaml
  label: Cisco Hardware Licensing API
  slug: cisco-hardware-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-licensing-api-openapi.yml
- filename: cisco-hardware-networks-api-openapi.yml
  format: yaml
  label: Cisco Hardware Networks API
  slug: cisco-hardware-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-networks-api-openapi.yml
- filename: cisco-hardware-organizations-api-openapi.yml
  format: yaml
  label: Cisco Hardware Organizations API
  slug: cisco-hardware-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-organizations-api-openapi.yml
- filename: cisco-hardware-sensor-api-openapi.yml
  format: yaml
  label: Cisco Hardware Sensor API
  slug: cisco-hardware-sensor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-sensor-api-openapi.yml
- filename: cisco-hardware-sm-api-openapi.yml
  format: yaml
  label: Cisco Hardware Sm API
  slug: cisco-hardware-sm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-sm-api-openapi.yml
- filename: cisco-hardware-spaces-api-openapi.yml
  format: yaml
  label: Cisco Hardware Spaces API
  slug: cisco-hardware-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-spaces-api-openapi.yml
- filename: cisco-hardware-switch-api-openapi.yml
  format: yaml
  label: Cisco Hardware Switch API
  slug: cisco-hardware-switch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-switch-api-openapi.yml
- filename: cisco-hardware-wireless-api-openapi.yml
  format: yaml
  label: Cisco Hardware Wireless API
  slug: cisco-hardware-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-wireless-api-openapi.yml
- filename: cisco-hardware-wirelesscontroller-api-openapi.yml
  format: yaml
  label: Cisco Hardware Wireless Controller API
  slug: cisco-hardware-wirelesscontroller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/openapi/cisco-hardware-wirelesscontroller-api-openapi.yml
consequence_counts:
  read: 7
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cisco Hardware Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Cisco Hardware exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cisco Hardware
provider_slug: cisco-hardware
slug: cisco-hardware-agentic-access
source_filename: cisco-hardware-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cisco-hardware-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 6\n    connected: 7\n  by_consequence:\n    write: 6\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /dna/system/api/v1/auth/token\n  method: post\n  operationId: authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dna/intent/api/v1/network-device\n  method: get\n  operationId: getDeviceList\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dna/intent/api/v1/network-device\n  method: post\n  operationId: addDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dna/intent/api/v1/network-device/{id}\n  method: get\n  operationId: getDeviceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dna/intent/api/v1/network-device/{id}\n  method: delete\n  operationId: deleteDeviceById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dna/intent/api/v1/network-device/count\n  method: get\n  operationId: getDeviceCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dna/intent/api/v1/site\n  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dna/intent/api/v1/site\n  method: post\n  operationId: createSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dna/intent/api/v1/discovery\n  method: post\n  operationId: startDiscovery\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dna/intent/api/v1/discovery\n  method: get\n  operationId: getDiscoveriesByRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dna/intent/api/v1/network-device-poller/cli/read-request\n  method: post\n  operationId: runCliCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dna/intent/api/v1/topology/physical-topology\n  method: get\n  operationId: getPhysicalTopology\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dna/intent/api/v1/network\n  method: get\n  operationId: getNetwork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-hardware/refs/heads/main/agentic-access/cisco-hardware-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Hardware
- Infrastructure
- Networking
- Router
- Switches
---
