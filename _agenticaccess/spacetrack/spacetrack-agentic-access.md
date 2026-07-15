---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 21
api_specs:
- filename: openapi.json
  format: json
  label: Space-Track API
  slug: space-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacetrack/refs/heads/main/openapi/openapi.json
consequence_counts:
  read: 21
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Spacetrack Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Space-Track exposes 22 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Space-Track
provider_slug: spacetrack
slug: spacetrack-agentic-access
source_filename: spacetrack-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 1\n    connected: 21\n  by_consequence:\n    write: 1\n    read: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /ajaxauth/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /basicspacedata/query/class/gp/{queryParams}\n  method: get\n  operationId: queryGP\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/gp_history/{queryParams}\n  method: get\n  operationId: queryGPHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/satcat/{queryParams}\n  method: get\n  operationId: querySATCAT\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/satcat_change/{queryParams}\n  method: get\n  operationId: querySATCATChange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/satcat_debut/{queryParams}\n  method: get\n  operationId: querySATCATDebut\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/decay/{queryParams}\n  method: get\n  operationId: queryDecay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/cdm_public/{queryParams}\n  method: get\n  operationId: queryCDMPublic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/tip/{queryParams}\n  method: get\n  operationId: queryTIP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/boxscore/{queryParams}\n  method: get\n  operationId: queryBoxscore\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/launch_site/{queryParams}\n  method: get\n  operationId: queryLaunchSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/announcement/{queryParams}\n  method: get\n  operationId: queryAnnouncement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/omm/{queryParams}\n  method: get\n  operationId: queryOMM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/tle/{queryParams}\n  method: get\n  operationId: queryTLE\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/tle_latest/{queryParams}\n  method: get\n  operationId: queryTLELatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/tle_publish/{queryParams}\n  method: get\n  operationId: queryTLEPublish\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expandedspacedata/query/class/cdm/{queryParams}\n  method: get\n  operationId: queryCDM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expandedspacedata/query/class/maneuver/{queryParams}\n  method: get\n  operationId: queryManeuver\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expandedspacedata/query/class/maneuver_history/{queryParams}\n  method: get\n  operationId: queryManeuverHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expandedspacedata/query/class/organization/{queryParams}\n  method: get\n  operationId: queryOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expandedspacedata/query/class/satellite/{queryParams}\n  method: get\n  operationId: querySatellite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /expandedspacedata/query/class/car/{queryParams}\n  method: get\n  operationId: queryCAR\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacetrack/refs/heads/main/agentic-access/spacetrack-agentic-access.yml
summary_line: 22 operations · 1 acting
tags:
- Space
- Satellites
- TLE
- Orbital Data
- Space Surveillance
- Debris Tracking
- Conjunction Data
- US Military
---
