---
acting_count: 0
action_class_counts:
  connected: 30
api_specs:
- filename: cisco-psirt-current-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Current Endpoints API
  slug: cisco-psirt-current-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-current-endpoints-api-openapi.yml
- filename: cisco-psirt-obsolete-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Obsolete Endpoints API
  slug: cisco-psirt-obsolete-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-obsolete-endpoints-api-openapi.yml
- filename: cisco-psirt-sunset-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Sunset Endpoints API
  slug: cisco-psirt-sunset-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-sunset-endpoints-api-openapi.yml
consequence_counts:
  read: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cisco Psirt Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'Cisco PSIRT openVuln API exposes 30 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cisco PSIRT openVuln API
provider_slug: cisco-psirt
slug: cisco-psirt-agentic-access
source_filename: cisco-psirt-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: generated\nsource: openapi/cisco-psirt-current-endpoints-api-openapi.yml, openapi/cisco-psirt-obsolete-endpoints-api-openapi.yml,\n  openapi/cisco-psirt-sunset-endpoints-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 30\n  by_consequence:\n    read: 30\n  human_in_the_loop_required: 0\noperations:\n- path: /all\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /all/firstpublished\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /all/lastpublished\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /advisory/{advisoryId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cve/{cve_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bugid/{bug_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /latest/{number}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /severity/{severity}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /severity/{severity}/firstpublished\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /severity/{severity}/lastpublished\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /year/{year}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OSType/{OSType}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /OS_version/OS_data\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cvrf/advisory/{advisoryId}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cvrf/all\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cvrf/all/firstpublished\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cvrf/all/lastpublished\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cvrf/cve/{cve_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /cvrf/product\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cvrf/severity/{severity}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cvrf/severity/{severity}/lastpublished\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cvrf/severity/{severity}/firstpublished\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cvrf/year/{year}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ios\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iosxe\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aci\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nxos\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /nos_version/nos_data\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:advisories\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/agentic-access/cisco-psirt-agentic-access.yml
summary_line: 30 operations
tags:
- Security
- Vulnerability Management
- Threat Intelligence
- Disclosure
- Compliance
- Networking
---
