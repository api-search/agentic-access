---
acting_count: 0
action_class_counts:
  connected: 24
api_specs:
- filename: nasa-apod-openapi.yml
  format: yaml
  label: NASA Astronomy Picture of the Day (APOD) API
  slug: apod
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-apod-openapi.yml
- filename: nasa-mars-rover-photos-openapi.yml
  format: yaml
  label: NASA Mars Rover Photos API
  slug: mars-rover-photos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-mars-rover-photos-openapi.yml
- filename: nasa-neo-openapi.yml
  format: yaml
  label: NASA NeoWs (Near Earth Object Web Service) API
  slug: neo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-neo-openapi.yml
- filename: nasa-donki-openapi.yml
  format: yaml
  label: NASA DONKI (Space Weather) API
  slug: donki
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-donki-openapi.yml
- filename: nasa-epic-openapi.yml
  format: yaml
  label: NASA EPIC (Earth Polychromatic Imaging Camera) API
  slug: epic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-epic-openapi.yml
- filename: nasa-nasa-image-and-video-library-openapi.yml
  format: yaml
  label: NASA Image and Video Library API
  slug: image-and-video-library
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/openapi/nasa-nasa-image-and-video-library-openapi.yml
consequence_counts:
  read: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nasa Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'NASA exposes 24 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NASA
provider_slug: nasa
slug: nasa-agentic-access
source_filename: nasa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nasa-apod-openapi.yml, openapi/nasa-donki-openapi.yml, openapi/nasa-epic-openapi.yml,\n  openapi/nasa-mars-rover-photos-openapi.yml, openapi/nasa-nasa-image-and-video-library-openapi.yml,\n  openapi/nasa-neo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 24\n  by_consequence:\n    read: 24\n  human_in_the_loop_required: 0\noperations:\n- path: /planetary/apod\n  method: get\n  operationId: getApod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/CME\n  method: get\n  operationId: getCoronalMassEjections\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/CMEAnalysis\n  method: get\n  operationId: getCmeAnalysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/GST\n  method: get\n  operationId: getGeomagneticStorms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/FLR\n  method: get\n  operationId: getSolarFlares\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/SEP\n  method: get\n  operationId: getSolarEnergeticParticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /DONKI/MPC\n  method: get\n  operationId: getMagnetopauseCrossings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/IPS\n  method: get\n  operationId: getInterplanetaryShocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/notifications\n  method: get\n  operationId: getDonkiNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /EPIC/api/natural\n  method: get\n  operationId: getEpicNatural\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /EPIC/api/natural/date/{date}\n  method: get\n  operationId: getEpicNaturalByDate\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /EPIC/api/natural/all\n  method: get\n  operationId: getEpicNaturalDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /EPIC/api/enhanced\n  method: get\n  operationId: getEpicEnhanced\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /EPIC/api/enhanced/date/{date}\n  method: get\n  operationId: getEpicEnhancedByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mars-photos/api/v1/rovers/{rover}/photos\n  method: get\n  operationId: getRoverPhotos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /mars-photos/api/v1/rovers/{rover}/latest_photos\n  method: get\n  operationId: getLatestRoverPhotos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mars-photos/api/v1/manifests/{rover}\n  method: get\n  operationId: getRoverManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: searchMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset/{nasa_id}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata/{nasa_id}\n  method:\
  \ get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /captions/{nasa_id}\n  method: get\n  operationId: getCaptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /neo/rest/v1/feed\n  method: get\n  operationId: getNeoFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /neo/rest/v1/neo/{asteroid_id}\n  method: get\n  operationId: getNeoById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /neo/rest/v1/neo/browse\n  method: get\n  operationId: browseNeos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/agentic-access/nasa-agentic-access.yml
summary_line: 24 operations
tags:
- Government
- Science
- Space
---
