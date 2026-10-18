---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 38
api_specs:
- filename: yatmo-bikepaths-api-openapi.yml
  format: yaml
  label: Yatmo Bike Paths API
  slug: yatmo-bikepaths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-bikepaths-api-openapi.yml
- filename: yatmo-categories-api-openapi.yml
  format: yaml
  label: Yatmo Categories API
  slug: yatmo-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-categories-api-openapi.yml
- filename: yatmo-enrichment-api-openapi.yml
  format: yaml
  label: Yatmo Enrichment API
  slug: yatmo-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-enrichment-api-openapi.yml
- filename: yatmo-frenchneighbourhoods-api-openapi.yml
  format: yaml
  label: Yatmo French Neighbourhoods API
  slug: yatmo-frenchneighbourhoods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-frenchneighbourhoods-api-openapi.yml
- filename: yatmo-geolocation-api-openapi.yml
  format: yaml
  label: Yatmo Geolocation API
  slug: yatmo-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-geolocation-api-openapi.yml
- filename: yatmo-geopositionencoder-api-openapi.yml
  format: yaml
  label: Yatmo Geo Position Encoder API
  slug: yatmo-geopositionencoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-geopositionencoder-api-openapi.yml
- filename: yatmo-image-api-openapi.yml
  format: yaml
  label: Yatmo Image API
  slug: yatmo-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-image-api-openapi.yml
- filename: yatmo-immotopcategories-api-openapi.yml
  format: yaml
  label: Yatmo Immotop Categories API
  slug: yatmo-immotopcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-immotopcategories-api-openapi.yml
- filename: yatmo-isochrone-api-openapi.yml
  format: yaml
  label: Yatmo Isochrone API
  slug: yatmo-isochrone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-isochrone-api-openapi.yml
- filename: yatmo-nearcheck-api-openapi.yml
  format: yaml
  label: Yatmo Near Check API
  slug: yatmo-nearcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-nearcheck-api-openapi.yml
- filename: yatmo-neighbourhood-api-openapi.yml
  format: yaml
  label: Yatmo Neighbourhood API
  slug: yatmo-neighbourhood-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-neighbourhood-api-openapi.yml
- filename: yatmo-points-api-openapi.yml
  format: yaml
  label: Yatmo Points API
  slug: yatmo-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-points-api-openapi.yml
- filename: yatmo-route-api-openapi.yml
  format: yaml
  label: Yatmo Route API
  slug: yatmo-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-route-api-openapi.yml
- filename: yatmo-scores-api-openapi.yml
  format: yaml
  label: Yatmo Scores API
  slug: yatmo-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-scores-api-openapi.yml
- filename: yatmo-shape-api-openapi.yml
  format: yaml
  label: Yatmo Shape API
  slug: yatmo-shape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-shape-api-openapi.yml
- filename: yatmo-simplifiedcategories-api-openapi.yml
  format: yaml
  label: Yatmo Simplified Categories API
  slug: yatmo-simplifiedcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-simplifiedcategories-api-openapi.yml
- filename: yatmo-summary-api-openapi.yml
  format: yaml
  label: Yatmo Summary API
  slug: yatmo-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-summary-api-openapi.yml
consequence_counts:
  read: 38
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Yatmo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 40
overview: 'Yatmo exposes 40 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Yatmo
provider_slug: yatmo
slug: yatmo-agentic-access
source_filename: yatmo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: generated\nsource: openapi/yatmo-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 38\n    acting: 2\n  by_consequence:\n    read: 38\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /BikePaths\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /BikePaths\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Categories\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Categories\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Categories/Lifestyle\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Categories/Lifestyle/Lines\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Enrichment\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Enrichment\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /FrenchNeighbourhoods\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /FrenchNeighbourhoods\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Geolocation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Geolocation/GetClose\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /GeoPositionEncoder\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /GeoPositionEncoder/random-circle-center\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Image\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ImmotopCategories\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ImmotopCategories\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Isochrone\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Isochrone/TravelTime\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Isochrone/GetMultipleTimes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /NearCheck\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /NearCheck\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Neighbourhood\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Neighbourhood\n  method: head\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Points\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Points\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Route\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Route/AllTravelModes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Scores\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /Scores\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Shape/{shapeId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SimplifiedCategories\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SimplifiedCategories\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Summary\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Summary\n\
  \  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Summary/encoded/{encodedGeoPosition}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Summary/text\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Summary/text-and-data\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Summary/clear\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /Summary/text-encoded/{encodedGeoPosition}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/agentic-access/yatmo-agentic-access.yml
summary_line: 40 operations · 2 acting
tags:
- Company
- Real Estate
- LocationIntelligence
- MappingAPI
- POIData
---
