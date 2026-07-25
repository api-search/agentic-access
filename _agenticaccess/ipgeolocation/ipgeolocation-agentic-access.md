---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 9
api_specs:
- filename: ipgeolocation-asn-lookup-api-openapi.yml
  format: yaml
  label: IPGeolocation.io ASN Lookup API
  slug: ipgeolocation-asn-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-asn-lookup-api-openapi.yml
- filename: ipgeolocation-astronomy-api-openapi.yml
  format: yaml
  label: IPGeolocation.io Astronomy API
  slug: ipgeolocation-astronomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-astronomy-api-openapi.yml
- filename: ipgeolocation-ip-abuse-contact-api-openapi.yml
  format: yaml
  label: IPGeolocation.io IP Abuse Contact API
  slug: ipgeolocation-ip-abuse-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-ip-abuse-contact-api-openapi.yml
- filename: ipgeolocation-ip-geolocation-api-openapi.yml
  format: yaml
  label: IPGeolocation.io IP Geolocation API
  slug: ipgeolocation-ip-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-ip-geolocation-api-openapi.yml
- filename: ipgeolocation-ip-security-api-openapi.yml
  format: yaml
  label: IPGeolocation.io IP Security API
  slug: ipgeolocation-ip-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-ip-security-api-openapi.yml
- filename: ipgeolocation-timezone-api-openapi.yml
  format: yaml
  label: IPGeolocation.io Timezone API
  slug: ipgeolocation-timezone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-timezone-api-openapi.yml
- filename: ipgeolocation-user-agent-api-openapi.yml
  format: yaml
  label: IPGeolocation.io User Agent API
  slug: ipgeolocation-user-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-user-agent-api-openapi.yml
consequence_counts:
  read: 9
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ipgeolocation Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'IPGeolocation.io exposes 13 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IPGeolocation.io
provider_slug: ipgeolocation
slug: ipgeolocation-agentic-access
source_filename: ipgeolocation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ipgeolocation-abuse-openapi.yml, openapi/ipgeolocation-asn-openapi.yml, openapi/ipgeolocation-astronomy-openapi.yml,\n  openapi/ipgeolocation-ip-location-openapi.yml, openapi/ipgeolocation-security-openapi.yml,\n  openapi/ipgeolocation-timezone-openapi.yml, openapi/ipgeolocation-user-agent-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 9\n    acting: 4\n  by_consequence:\n    read: 9\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/abuse\n  method: get\n  operationId: lookupIpAbuseContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v3/asn\n  method: get\n  operationId: lookupASN\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/astronomy\n  method: get\n  operationId: lookupAstronomy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/astronomy/timeSeries\n  method: get\n  operationId: lookupAstronomyTimeSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/ipgeo\n  method: get\n  operationId: lookupIpGeolocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/ipgeo-bulk\n  method: post\n  operationId: bulkLookupIpGeolocation\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/security\n  method: get\n  operationId: lookupIpSecurity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/security-bulk\n  method: post\n  operationId: bulkLookupIpSecurity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/timezone\n  method: get\n  operationId: lookupTimezone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v3/timezone/convert\n  method: get\n  operationId: convertTimezone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/user-agent\n  method: get\n  operationId: parseUserAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/user-agent\n  method: post\n  operationId: parseCustomUserAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/user-agent-bulk\n  method: post\n  operationId: parseUserAgentBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/agentic-access/ipgeolocation-agentic-access.yml
summary_line: 13 operations · 4 acting
tags:
- Geocoding
- IP Geolocation
- IP Intelligence
- IP Security
- ASN Lookup
- Abuse Contact
- Timezone
- Astronomy
- User Agent
- Threat Intelligence
- Public APIs
---
