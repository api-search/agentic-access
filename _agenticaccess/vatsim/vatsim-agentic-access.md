---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 32
api_specs:
- filename: openapi.json
  format: json
  label: VATSIM Core API
  slug: vatsim-core-api
  spec_type: OpenAPI
  url: https://api.vatsim.net/v2/openapi.json
- filename: openapi.json
  format: json
  label: VATSIM Data API
  slug: vatsim-data-api
  spec_type: OpenAPI
  url: https://data.vatsim.net/openapi.json
- filename: metar.yaml
  format: yaml
  label: VATSIM METAR API
  slug: vatsim-metar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/metar.yaml
- filename: connect.yaml
  format: yaml
  label: VATSIM Connect API
  slug: vatsim-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/connect.yaml
- filename: slurper.yaml
  format: yaml
  label: VATSIM Slurper API
  slug: vatsim-slurper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/slurper.yaml
consequence_counts:
  read: 32
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vatsim Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 34
overview: 'VATSIM exposes 34 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: VATSIM
provider_slug: vatsim
slug: vatsim-agentic-access
source_filename: vatsim-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/aip.yaml, openapi/connect.yaml, openapi/core-api.json, openapi/data.yaml, openapi/events-v1.yaml,\n  openapi/events-v2.yaml, openapi/metar.yaml, openapi/slurper.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 32\n    acting: 2\n  by_consequence:\n    read: 32\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /airports/{icao}\n  method: get\n  operationId: getAirport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /airports/{icao}/stations\n  method: get\n  operationId: listAirportStations\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/authorize\n  method: get\n  operationId: redirect\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/token\n  method: post\n  operationId: getToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/user\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - country\n    - email\n    - full_name\n    - vatsim_details\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/members/{member_id}/flightplans\n  method: get\n\
  \  operationId: members_api_retrieve_member_flightplans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/members/{member_id}/stats\n  method: get\n  operationId: members_api_retrieve_member_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/members/{member_id}/status\n  method: get\n  operationId: members_api_retrieve_member_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/members/{member_id}\n  method: get\n  operationId: members_api_retrieve_member_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/members/{member_id}\n  method: patch\n\
  \  operationId: members_api_update_member_details\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/members/{member_id}/atc\n  method: get\n  operationId: members_api_history_atc_cid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/members/online\n  method: get\n  operationId: members_api_online\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/members/{member_id}/history\n  method: get\n  operationId: members_api_history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /v2/members/discord/{discord_user_id}\n  method: get\n  operationId: members_api_get_vatsim_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orgs/subdivision/{subdivision_id}\n  method: get\n  operationId: orgs_api_subdivision_roster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orgs/division/{division_id}\n  method: get\n  operationId: orgs_api_division_roster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/atc/online\n  method: get\n  operationId: atc_api_online_atc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v2/atc/history\n  method: get\n  operationId: atc_api_history_atc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vatsim-servers.json\n  method: get\n  operationId: listLiveFSDServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sweatbox-servers.json\n  method: get\n  operationId: listSweatboxFSDServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /all-servers.json\n  method: get\n  operationId: listAllFSDServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vatsim-data.json\n  method: get\n  operationId: getNetworkData\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transceivers-data.json\n  method: get\n  operationId: listAudioClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /afv-atis-data.json\n  method: get\n  operationId: listATISStations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{num}\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{num}/{regionId}\n  method: get\n  operationId: listEventsByRegion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /latest\n  method: get\n  operationId: listAllEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /latest/{num}\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /view/{eventId}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /view/region/{regionId}\n  method: get\n  operationId: listEventsByRegion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /view/division/{divisionId}\n  method: get\n  operationId: listEventsByDivision\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export\n  method: get\n  operationId: exportEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{icao}\n  method: get\n  operationId: getMetar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/info\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/agentic-access/vatsim-agentic-access.yml
summary_line: 34 operations · 2 acting
tags:
- Aviation
- Flight Simulation
- Air Traffic Control
- Real-Time Data
- Community
---
