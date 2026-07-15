---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 9
api_specs:
- filename: ipgeolocation-ip-location-openapi.yml
  format: yaml
  label: IP Geolocation
  slug: ip-geolocation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-ip-location-openapi.yml
- filename: ipgeolocation-security-openapi.yml
  format: yaml
  label: IP Security
  slug: ip-security
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-security-openapi.yml
- filename: ipgeolocation-asn-openapi.yml
  format: yaml
  label: ASN Lookup
  slug: asn-lookup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-asn-openapi.yml
- filename: ipgeolocation-abuse-openapi.yml
  format: yaml
  label: IP Abuse Contact
  slug: ip-abuse-contact
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-abuse-openapi.yml
- filename: ipgeolocation-timezone-openapi.yml
  format: yaml
  label: Timezone
  slug: timezone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-timezone-openapi.yml
- filename: ipgeolocation-astronomy-openapi.yml
  format: yaml
  label: Astronomy
  slug: astronomy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-astronomy-openapi.yml
- filename: ipgeolocation-user-agent-openapi.yml
  format: yaml
  label: User Agent
  slug: user-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-user-agent-openapi.yml
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
