---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 25
api_specs:
- filename: spacex-api-capsules-api-openapi.yml
  format: yaml
  label: SpaceX API Capsules API
  slug: spacex-api-capsules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/openapi/spacex-api-capsules-api-openapi.yml
- filename: spacex-api-cores-api-openapi.yml
  format: yaml
  label: SpaceX API Cores API
  slug: spacex-api-cores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/openapi/spacex-api-cores-api-openapi.yml
- filename: spacex-api-crew-api-openapi.yml
  format: yaml
  label: SpaceX API Crew API
  slug: spacex-api-crew-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/openapi/spacex-api-crew-api-openapi.yml
- filename: spacex-api-landing-pads-api-openapi.yml
  format: yaml
  label: SpaceX API Landing Pads API
  slug: spacex-api-landing-pads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/openapi/spacex-api-landing-pads-api-openapi.yml
- filename: spacex-api-launches-api-openapi.yml
  format: yaml
  label: SpaceX API Launches API
  slug: spacex-api-launches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/openapi/spacex-api-launches-api-openapi.yml
- filename: spacex-api-launchpads-api-openapi.yml
  format: yaml
  label: SpaceX API Launchpads API
  slug: spacex-api-launchpads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/openapi/spacex-api-launchpads-api-openapi.yml
- filename: spacex-api-payloads-api-openapi.yml
  format: yaml
  label: SpaceX API Payloads API
  slug: spacex-api-payloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/openapi/spacex-api-payloads-api-openapi.yml
- filename: spacex-api-roadster-api-openapi.yml
  format: yaml
  label: SpaceX API Roadster API
  slug: spacex-api-roadster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/openapi/spacex-api-roadster-api-openapi.yml
- filename: spacex-api-rockets-api-openapi.yml
  format: yaml
  label: SpaceX API Rockets API
  slug: spacex-api-rockets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/openapi/spacex-api-rockets-api-openapi.yml
- filename: spacex-api-ships-api-openapi.yml
  format: yaml
  label: SpaceX API Ships API
  slug: spacex-api-ships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/openapi/spacex-api-ships-api-openapi.yml
- filename: spacex-api-starlink-api-openapi.yml
  format: yaml
  label: SpaceX API Starlink API
  slug: spacex-api-starlink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/openapi/spacex-api-starlink-api-openapi.yml
consequence_counts:
  read: 25
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Spacex Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'SpaceX API exposes 26 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SpaceX API
provider_slug: spacex-api
slug: spacex-api-agentic-access
source_filename: spacex-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/spacex-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 25\n    acting: 1\n  by_consequence:\n    read: 25\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /launches\n  method: get\n  operationId: listLaunches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /launches/latest\n  method: get\n  operationId: getLatestLaunch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /launches/next\n  method: get\n \
  \ operationId: getNextLaunch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /launches/upcoming\n  method: get\n  operationId: listUpcomingLaunches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /launches/past\n  method: get\n  operationId: listPastLaunches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /launches/{id}\n  method: get\n  operationId: getLaunch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /launches/query\n  method: post\n  operationId: queryLaunches\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rockets\n  method: get\n  operationId: listRockets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rockets/{id}\n  method: get\n  operationId: getRocket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capsules\n  method: get\n  operationId: listCapsules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capsules/{id}\n  method: get\n  operationId: getCapsule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /cores\n  method: get\n  operationId: listCores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cores/{id}\n  method: get\n  operationId: getCore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crew\n  method: get\n  operationId: listCrew\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crew/{id}\n  method: get\n  operationId: getCrewMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /launchpads\n  method: get\n  operationId: listLaunchpads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /launchpads/{id}\n  method: get\n  operationId: getLaunchpad\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /landpads\n  method: get\n  operationId: listLandpads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /landpads/{id}\n  method: get\n  operationId: getLandpad\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payloads\n  method: get\n  operationId: listPayloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payloads/{id}\n  method: get\n  operationId: getPayload\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ships\n  method: get\n  operationId: listShips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ships/{id}\n  method: get\n  operationId: getShip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /starlink\n  method: get\n  operationId: listStarlink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /starlink/{id}\n  method: get\n  operationId: getStarlinkSatellite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roadster\n  method: get\n  operationId: getRoadster\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/agentic-access/spacex-api-agentic-access.yml
summary_line: 26 operations · 1 acting
tags:
- Space
- Aerospace
- Launches
- SpaceX
---
