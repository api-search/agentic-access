---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 72
api_specs:
- filename: smarterweather-com-agriculture-api-openapi.yml
  format: yaml
  label: smarterweather-com Agriculture API
  slug: smarterweather-com-agriculture-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smarterweather-com/openapi/smarterweather-com-agriculture-api-openapi.yml
- filename: smarterweather-com-alerts-api-openapi.yml
  format: yaml
  label: smarterweather-com Alerts API
  slug: smarterweather-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smarterweather-com/openapi/smarterweather-com-alerts-api-openapi.yml
- filename: smarterweather-com-climate-api-openapi.yml
  format: yaml
  label: smarterweather-com Climate API
  slug: smarterweather-com-climate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smarterweather-com/openapi/smarterweather-com-climate-api-openapi.yml
- filename: smarterweather-com-geocode-api-openapi.yml
  format: yaml
  label: smarterweather-com Geocode API
  slug: smarterweather-com-geocode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smarterweather-com/openapi/smarterweather-com-geocode-api-openapi.yml
- filename: smarterweather-com-guidance-api-openapi.yml
  format: yaml
  label: smarterweather-com Guidance API
  slug: smarterweather-com-guidance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smarterweather-com/openapi/smarterweather-com-guidance-api-openapi.yml
- filename: smarterweather-com-health-api-openapi.yml
  format: yaml
  label: smarterweather-com Health API
  slug: smarterweather-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smarterweather-com/openapi/smarterweather-com-health-api-openapi.yml
- filename: smarterweather-com-meta-api-openapi.yml
  format: yaml
  label: smarterweather-com Meta API
  slug: smarterweather-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smarterweather-com/openapi/smarterweather-com-meta-api-openapi.yml
- filename: smarterweather-com-observations-api-openapi.yml
  format: yaml
  label: smarterweather-com Observations API
  slug: smarterweather-com-observations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smarterweather-com/openapi/smarterweather-com-observations-api-openapi.yml
- filename: smarterweather-com-products-api-openapi.yml
  format: yaml
  label: smarterweather-com Products API
  slug: smarterweather-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smarterweather-com/openapi/smarterweather-com-products-api-openapi.yml
- filename: smarterweather-com-storms-api-openapi.yml
  format: yaml
  label: smarterweather-com Storms API
  slug: smarterweather-com-storms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smarterweather-com/openapi/smarterweather-com-storms-api-openapi.yml
- filename: smarterweather-com-weather-api-openapi.yml
  format: yaml
  label: smarterweather-com Weather API
  slug: smarterweather-com-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/smarterweather-com/openapi/smarterweather-com-weather-api-openapi.yml
consequence_counts:
  read: 72
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Smarterweather Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 78
overview: 'smarterweather-com exposes 78 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 72 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: smarterweather-com
provider_slug: smarterweather-com
slug: smarterweather-com-agentic-access
source_filename: smarterweather-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/developers-smarterweather-com-openapi.yaml, openapi/smarterweather-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 78\n  by_action_class:\n    connected: 72\n    acting: 6\n  by_consequence:\n    read: 72\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/catalog\n  method: get\n  operationId: listCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/{product_id}\n  method: get\n  operationId: getCatalogProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/weather\n  method: get\n  operationId: getWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/weather/batch\n  method: post\n  operationId: postWeatherBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/weather/route\n  method: post\n  operationId: postWeatherRoute\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alerts\n  method: get\n  operationId: searchAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alerts/{id}\n  method: get\n  operationId: getAlertById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{product_id}/exposure-summary\n  method: get\n  operationId: getProductExposureSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pois/exposure\n  method: post\n  operationId: postPoisExposure\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storm-tracks\n  method: get\n  operationId: getStormTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/observations\n  method: get\n  operationId: getObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/observations/nearest\n  method: get\n  operationId: getObservationsNearest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lightning\n  method: get\n  operationId: getLightning\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/soundings\n  method: get\n  operationId: getSoundings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/soundings/nearest\n  method: get\n  operationId: getSoundingsNearest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storm-reports\n  method: get\n  operationId: getStormReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/nexrad/features\n  method: get\n  operationId: getNexradFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/guidance/mesoscale\n  method: get\n  operationId: getGuidanceMesoscale\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/guidance/precipitation\n  method: get\n  operationId: getGuidancePrecipitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/text-products\n  method: get\n  operationId: listTextProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/discussions/mesoscale\n  method: get\n  operationId: getDiscussionsMesoscale\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tropical\n  method: get\n  operationId: getTropical\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tropical/observations\n  method: get\n  operationId: getTropicalObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/record-events\n  method: get\n  operationId: getRecordEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/climate-reports\n  method: get\n  operationId: getClimateReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geocode/reverse\n  method: get\n  operationId: getGeocodeReverse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geocode/autosuggest\n  method: get\n  operationId: getGeocodeAutosuggest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geocode/search\n  method: get\n  operationId: getGeocodeSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/deprecations\n  method: get\n  operationId: getDeprecations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agriculture/growing-degree-days\n  method: get\n  operationId: getGrowingDegreeDays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/climate/normals\n\
  \  method: get\n  operationId: getClimateNormals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/windows\n  method: get\n  operationId: getWindows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/point\n  method: get\n  operationId: getPointValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/series\n  method: get\n  operationId: getSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/series/batch\n  method: post\n  operationId: postSeriesBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/outlooks\n  method: get\n  operationId: getOutlookDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/outlooks/climate\n  method: get\n  operationId: getClimateOutlooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/catalog\n  method: get\n  operationId: listCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalog/{product_id}\n  method: get\n  operationId: getCatalogProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/weather\n  method: get\n  operationId: getWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/weather/batch\n  method: post\n  operationId: postWeatherBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/weather/route\n  method: post\n  operationId: postWeatherRoute\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alerts\n  method: get\n  operationId: searchAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alerts/{id}\n  method: get\n  operationId: getAlertById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/products/{product_id}/exposure-summary\n  method: get\n  operationId: getProductExposureSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pois/exposure\n  method: post\n  operationId: postPoisExposure\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/storm-tracks\n  method: get\n  operationId: getStormTracks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/observations\n  method: get\n  operationId: getObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/observations/nearest\n  method: get\n  operationId: getObservationsNearest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lightning\n  method: get\n  operationId: getLightning\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/soundings\n  method: get\n  operationId: getSoundings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/soundings/nearest\n  method: get\n  operationId: getSoundingsNearest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/storm-reports\n  method: get\n  operationId: getStormReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/nexrad/features\n  method: get\n  operationId: getNexradFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/guidance/mesoscale\n  method: get\n  operationId: getGuidanceMesoscale\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/guidance/precipitation\n  method: get\n  operationId: getGuidancePrecipitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/text-products\n  method: get\n  operationId: listTextProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/discussions/mesoscale\n  method: get\n  operationId: getDiscussionsMesoscale\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tropical\n  method: get\n  operationId: getTropical\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tropical/observations\n  method: get\n  operationId: getTropicalObservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/record-events\n  method: get\n  operationId: getRecordEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/climate-reports\n  method: get\n  operationId: getClimateReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geocode/reverse\n  method: get\n  operationId: getGeocodeReverse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geocode/autosuggest\n  method: get\n  operationId: getGeocodeAutosuggest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geocode/search\n  method: get\n  operationId: getGeocodeSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/deprecations\n  method: get\n  operationId: getDeprecations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agriculture/growing-degree-days\n  method: get\n  operationId: getGrowingDegreeDays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/climate/normals\n\
  \  method: get\n  operationId: getClimateNormals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/windows\n  method: get\n  operationId: getWindows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/point\n  method: get\n  operationId: getPointValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/series\n  method: get\n  operationId: getSeries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/series/batch\n  method: post\n  operationId: postSeriesBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/outlooks\n  method: get\n  operationId: getOutlookDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/outlooks/climate\n  method: get\n  operationId: getClimateOutlooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/smarterweather-com/agentic-access/smarterweather-com-agentic-access.yml
summary_line: 78 operations · 6 acting
tags:
- Company
- Weather
- Data
- Forecasting
- Climate
---
