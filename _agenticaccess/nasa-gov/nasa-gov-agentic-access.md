---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 61
api_specs:
- filename: apod-openapi.yml
  format: yaml
  label: NASA Astronomy Picture of the Day (APOD)
  slug: apod
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/apod-openapi.yml
- filename: asteroids-neows-openapi.yml
  format: yaml
  label: NASA Asteroids NeoWs (Near Earth Object Web Service)
  slug: asteroids-neows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/asteroids-neows-openapi.yml
- filename: donki-openapi.yml
  format: yaml
  label: NASA DONKI Space Weather API
  slug: donki
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/donki-openapi.yml
- filename: earth-openapi.yml
  format: yaml
  label: NASA Earth Imagery API
  slug: earth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/earth-openapi.yml
- filename: eonet-openapi.yml
  format: yaml
  label: NASA EONET (Earth Observatory Natural Event Tracker)
  slug: eonet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/eonet-openapi.yml
- filename: epic-openapi.yml
  format: yaml
  label: NASA EPIC (Earth Polychromatic Imaging Camera)
  slug: epic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/epic-openapi.yml
- filename: exoplanet-openapi.yml
  format: yaml
  label: NASA Exoplanet Archive API
  slug: exoplanet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/exoplanet-openapi.yml
- filename: insight-openapi.yml
  format: yaml
  label: NASA InSight Mars Weather Service API
  slug: insight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/insight-openapi.yml
- filename: mars-rover-photos-openapi.yml
  format: yaml
  label: NASA Mars Rover Photos API
  slug: mars-rover-photos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/mars-rover-photos-openapi.yml
- filename: image-video-library-openapi.yml
  format: yaml
  label: NASA Image and Video Library API
  slug: image-video-library
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/image-video-library-openapi.yml
- filename: techtransfer-openapi.yml
  format: yaml
  label: NASA TechTransfer API
  slug: techtransfer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/techtransfer-openapi.yml
- filename: ssd-cneos-openapi.yml
  format: yaml
  label: NASA SSD/CNEOS API
  slug: ssd-cneos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/ssd-cneos-openapi.yml
- filename: techport-openapi.yml
  format: yaml
  label: NASA TechPort API
  slug: techport
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/techport-openapi.yml
- filename: tle-openapi.yml
  format: yaml
  label: NASA TLE API (Two-Line Element Set)
  slug: tle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/tle-openapi.yml
- filename: satellite-situation-center-openapi.yml
  format: yaml
  label: NASA Satellite Situation Center API
  slug: satellite-situation-center
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/satellite-situation-center-openapi.yml
- filename: genelab-openapi.yml
  format: yaml
  label: NASA GeneLab Search API
  slug: genelab
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/genelab-openapi.yml
- filename: trek-wmts-openapi.yml
  format: yaml
  label: NASA Vesta/Moon/Mars Trek WMTS
  slug: trek-wmts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/trek-wmts-openapi.yml
consequence_counts:
  read: 61
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nasa Gov Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 62
overview: 'NASA Open APIs exposes 62 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 61 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NASA Open APIs
provider_slug: nasa-gov
slug: nasa-gov-agentic-access
source_filename: nasa-gov-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/apod-openapi.yml, openapi/asteroids-neows-openapi.yml, openapi/donki-openapi.yml,\n  openapi/earth-openapi.yml, openapi/eonet-openapi.yml, openapi/epic-openapi.yml, openapi/exoplanet-openapi.yml,\n  openapi/genelab-openapi.yml, openapi/image-video-library-openapi.yml, openapi/insight-openapi.yml,\n  openapi/mars-rover-photos-openapi.yml, openapi/satellite-situation-center-openapi.yml, openapi/ssd-cneos-openapi.yml,\n  openapi/techport-openapi.yml, openapi/techtransfer-openapi.yml, openapi/tle-openapi.yml, openapi/trek-wmts-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 62\n  by_action_class:\n    connected: 61\n    acting: 1\n  by_consequence:\n    read: 61\n    write:\
  \ 1\n  human_in_the_loop_required: 0\noperations:\n- path: /planetary/apod\n  method: get\n  operationId: getApod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /neo/rest/v1/feed\n  method: get\n  operationId: getNeoFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /neo/rest/v1/neo/{asteroid_id}\n  method: get\n  operationId: getNeoLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /neo/rest/v1/neo/browse\n  method: get\n  operationId: browseNeo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/CME\n  method: get\n  operationId: getCME\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/CMEAnalysis\n  method: get\n  operationId: getCMEAnalysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/GST\n  method: get\n  operationId: getGST\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/IPS\n  method: get\n  operationId: getIPS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/FLR\n  method: get\n  operationId: getFLR\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/SEP\n  method: get\n  operationId:\
  \ getSEP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/MPC\n  method: get\n  operationId: getMPC\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/RBE\n  method: get\n  operationId: getRBE\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/HSS\n  method: get\n  operationId: getHSS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DONKI/WSAEnlilSimulations\n  method: get\n  operationId: getWSAEnlilSimulations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /DONKI/notifications\n  method: get\n  operationId: getNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /planetary/earth/imagery\n  method: get\n  operationId: getEarthImagery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /planetary/earth/assets\n  method: get\n  operationId: getEarthAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: getEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: get\n  operationId: getCategories\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{category}\n  method: get\n  operationId: getEventsByCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources\n  method: get\n  operationId: getSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /layers\n  method: get\n  operationId: getLayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /magnitudes\n  method: get\n  operationId: getMagnitudes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/natural\n  method: get\n  operationId: getNaturalRecent\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/natural/date/{date}\n  method: get\n  operationId: getNaturalByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/natural/available\n  method: get\n  operationId: getNaturalAvailable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/natural/all\n  method: get\n  operationId: getNaturalAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/enhanced\n  method: get\n  operationId: getEnhancedRecent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/enhanced/date/{date}\n  method: get\n  operationId: getEnhancedByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/enhanced/available\n  method: get\n  operationId: getEnhancedAvailable\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sync\n  method: get\n  operationId: tapSync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /async\n  method: post\n  operationId: tapAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /search\n  method: get\n  operationId: searchGeneLab\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: searchLibrary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset/{nasa_id}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata/{nasa_id}\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /captions/{nasa_id}\n  method: get\n  operationId: getCaptions\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /album/{album_name}\n  method: get\n  operationId: getAlbum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getInsightWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rovers\n  method: get\n  operationId: listRovers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rovers/{rover}/photos\n  method: get\n  operationId: getRoverPhotos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rovers/{rover}/latest_photos\n  method: get\n\
  \  operationId: getRoverLatestPhotos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manifests/{rover}\n  method: get\n  operationId: getRoverManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /observatories\n  method: get\n  operationId: listObservatories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groundStations\n  method: get\n  operationId: listGroundStations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: getLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /cad.api\n  method: get\n  operationId: getCAD\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sbdb.api\n  method: get\n  operationId: sbdbLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sbdb_query.api\n  method: get\n  operationId: sbdbQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sentry.api\n  method: get\n  operationId: sentry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fireball.api\n  method: get\n  operationId: fireball\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nhats.api\n  method: get\n  operationId: nhats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scout.api\n  method: get\n  operationId: scout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/projects/{id}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patent\n  method: get\n  operationId: searchPatents\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patent/issued\n  method: get\n  operationId: searchIssuedPatents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /software\n  method: get\n  operationId: searchSoftware\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spinoff\n  method: get\n  operationId: searchSpinoff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tle\n  method: get\n  operationId: listTle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tle/{satelliteId}\n  method:\
  \ get\n  operationId: getTle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiles/{body}/EQ/{layer}/1.0.0/default/default028mm/{z}/{y}/{x}.{ext}\n  method: get\n  operationId: getTrekTile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/agentic-access/nasa-gov-agentic-access.yml
summary_line: 62 operations · 1 acting
tags:
- Government
- Federal
- Space
- Earth Science
- Open Data
- Astronomy
- Planetary Science
- Heliophysics
- Bioscience
- NASA
---
