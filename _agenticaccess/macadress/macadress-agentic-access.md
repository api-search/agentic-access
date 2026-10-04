---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: macadress-healthz-api-openapi.yml
  format: yaml
  label: 'MAC Address Lookup: Find Vendor, OUI & Device Type Healthz API'
  slug: macadress-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macadress/refs/heads/main/openapi/macadress-healthz-api-openapi.yml
- filename: macadress-mac-api-openapi.yml
  format: yaml
  label: 'MAC Address Lookup: Find Vendor, OUI & Device Type Mac API'
  slug: macadress-mac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macadress/refs/heads/main/openapi/macadress-mac-api-openapi.yml
- filename: macadress-vendors-api-openapi.yml
  format: yaml
  label: 'MAC Address Lookup: Find Vendor, OUI & Device Type Vendors API'
  slug: macadress-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macadress/refs/heads/main/openapi/macadress-vendors-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Macadress Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'MAC Address Lookup: Find Vendor, OUI & Device Type exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 'MAC Address Lookup: Find Vendor, OUI & Device Type'
provider_slug: macadress
slug: macadress-agentic-access
source_filename: macadress-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/macadress-healthz-api-openapi.yml, openapi/macadress-mac-api-openapi.yml, openapi/macadress-vendors-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/healthz\n  method: get\n  operationId: healthz\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mac/{mac}\n  method: get\n  operationId: lookupMAC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/mac/batch\n  method: post\n  operationId: lookupMACBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vendors\n  method: get\n  operationId: searchVendors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macadress/refs/heads/main/agentic-access/macadress-agentic-access.yml
summary_line: 4 operations
tags:
- Networking
- Network Access Control
- Security
- SecOps
- IoT
- Device Fleet Management
- MDM
- Reference Data
- IEEE OUI Lookup
- Developer Tools
- MCP
- Agent-Native
---
