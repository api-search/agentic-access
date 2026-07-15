---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 11
api_specs:
- filename: datalastic-openapi.yml
  format: yaml
  label: Datalastic Live Vessel Tracking API
  slug: datalastic-live-vessel-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-openapi.yml
- filename: datalastic-openapi.yml
  format: yaml
  label: Datalastic Vessel Traffic in Radius API
  slug: datalastic-vessel-traffic-in-radius-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-openapi.yml
- filename: datalastic-openapi.yml
  format: yaml
  label: Datalastic Historical Vessel Track API
  slug: datalastic-historical-vessel-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-openapi.yml
- filename: datalastic-openapi.yml
  format: yaml
  label: Datalastic Vessel Info and Finder API
  slug: datalastic-vessel-info-and-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-openapi.yml
- filename: datalastic-openapi.yml
  format: yaml
  label: Datalastic Port Finder API
  slug: datalastic-port-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-openapi.yml
- filename: datalastic-openapi.yml
  format: yaml
  label: Datalastic Reports and Usage API
  slug: datalastic-reports-and-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-openapi.yml
consequence_counts:
  read: 11
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Datalastic Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Datalastic exposes 12 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Datalastic
provider_slug: datalastic
slug: datalastic-agentic-access
source_filename: datalastic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/datalastic-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 11\n    acting: 1\n  by_consequence:\n    read: 11\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /vessel\n  method: get\n  operationId: getVessel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel_pro\n  method: get\n  operationId: getVesselPro\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel_bulk\n  method: get\n  operationId: getVesselBulk\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel_inradius\n  method: get\n  operationId: getVesselsInRadius\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inradius_history\n  method: get\n  operationId: getInRadiusHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel_history\n  method: get\n  operationId: getVesselHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vessel_info\n  method: get\n  operationId: getVesselInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /vessel_find\n  method: get\n  operationId: findVessels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /port_find\n  method: get\n  operationId: findPorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report\n  method: post\n  operationId: submitReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stat\n\
  \  method: get\n  operationId: getUsageStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/agentic-access/datalastic-agentic-access.yml
summary_line: 12 operations · 1 acting
tags:
- Vessel Tracking
- Maritime
- AIS
- Ships
- Ports
- Shipping
---
