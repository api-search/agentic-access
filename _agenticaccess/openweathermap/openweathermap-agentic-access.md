---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 33
api_specs:
- filename: openweathermap-accumulated-parameters-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Accumulated Parameters API
  slug: openweathermap-accumulated-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-accumulated-parameters-api-openapi.yml
- filename: openweathermap-air-pollution-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Air Pollution API
  slug: openweathermap-air-pollution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-air-pollution-api-openapi.yml
- filename: openweathermap-current-weather-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Current Weather API
  slug: openweathermap-current-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-current-weather-api-openapi.yml
- filename: openweathermap-forecast-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Forecast API
  slug: openweathermap-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-forecast-api-openapi.yml
- filename: openweathermap-geocoding-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Geocoding API
  slug: openweathermap-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-geocoding-api-openapi.yml
- filename: openweathermap-history-api-openapi.yml
  format: yaml
  label: OpenWeatherMap History API
  slug: openweathermap-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-history-api-openapi.yml
- filename: openweathermap-measurements-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Measurements API
  slug: openweathermap-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-measurements-api-openapi.yml
- filename: openweathermap-one-call-api-openapi.yml
  format: yaml
  label: OpenWeatherMap One Call API
  slug: openweathermap-one-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-one-call-api-openapi.yml
- filename: openweathermap-road-risk-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Road Risk API
  slug: openweathermap-road-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-road-risk-api-openapi.yml
- filename: openweathermap-solar-irradiance-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Solar Irradiance API
  slug: openweathermap-solar-irradiance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-solar-irradiance-api-openapi.yml
- filename: openweathermap-solar-panels-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Solar Panels API
  slug: openweathermap-solar-panels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-solar-panels-api-openapi.yml
- filename: openweathermap-stations-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Stations API
  slug: openweathermap-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-stations-api-openapi.yml
- filename: openweathermap-statistical-weather-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Statistical Weather API
  slug: openweathermap-statistical-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-statistical-weather-api-openapi.yml
- filename: openweathermap-weather-maps-api-openapi.yml
  format: yaml
  label: OpenWeatherMap Weather Maps API
  slug: openweathermap-weather-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/openapi/openweathermap-weather-maps-api-openapi.yml
consequence_counts:
  read: 33
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openweathermap Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 42
overview: 'OpenWeatherMap exposes 42 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 33 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenWeatherMap
provider_slug: openweathermap
slug: openweathermap-agentic-access
source_filename: openweathermap-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openweathermap-accumulated-parameters-openapi.yml, openapi/openweathermap-air-pollution-openapi.yml,\n  openapi/openweathermap-current-weather-openapi.yml, openapi/openweathermap-forecast-openapi.yml,\n  openapi/openweathermap-geocoding-openapi.yml, openapi/openweathermap-history-openapi.yml,\n  openapi/openweathermap-one-call-openapi.yml, openapi/openweathermap-road-risk-openapi.yml,\n  openapi/openweathermap-solar-openapi.yml, openapi/openweathermap-statistical-weather-openapi.yml,\n  openapi/openweathermap-weather-maps-openapi.yml, openapi/openweathermap-weather-stations-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 33\n    acting:\
  \ 9\n  by_consequence:\n    read: 33\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /accumulated_temperature\n  method: get\n  operationId: getAccumulatedTemperature\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accumulated_precipitation\n  method: get\n  operationId: getAccumulatedPrecipitation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air_pollution\n  method: get\n  operationId: getCurrentAirPollution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /air_pollution/forecast\n  method: get\n  operationId: getAirPollutionForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /air_pollution/history\n  method: get\n  operationId: getAirPollutionHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /weather\n  method: get\n  operationId: getCurrentWeather\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecast\n  method: get\n  operationId: getForecastFiveDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecast/hourly\n  method: get\n  operationId: getForecastHourly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecast/daily\n  method: get\n  operationId: getForecastDaily\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forecast/climate\n  method: get\n  operationId: getForecastClimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /direct\n  method: get\n  operationId: getDirectGeocoding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zip\n  method: get\n  operationId: getZipGeocoding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse\n  method: get\n  operationId: getReverseGeocoding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/city\n\
  \  method: get\n  operationId: getHistoricalWeatherCity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /current\n  method: get\n  operationId: getOneCallCurrent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeline/1min\n  method: get\n  operationId: getOneCallTimelineOneMinute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeline/15min\n  method: get\n  operationId: getOneCallTimelineFifteenMinute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeline/1h\n  method: get\n  operationId: getOneCallTimelineHour\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeline/1day\n  method: get\n  operationId: getOneCallTimelineDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alert/{alert_id}\n  method: get\n  operationId: getOneCallAlert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/2.5/roadrisk\n  method: post\n  operationId: postRoadRisk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /solar/interval_data\n  method: get\n  operationId: getSolarIrradianceIntervalData\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: listSolarLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: post\n  operationId: createSolarLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /location/{location_id}\n  method: get\n  operationId: getSolarLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /location/{location_id}\n  method: delete\n  operationId: deleteSolarLocation\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /location/{location_id}/panels\n  method: get\n  operationId: listSolarPanels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /location/{location_id}/panels\n  method: post\n  operationId: createSolarPanel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /panel/{panel_id}\n  method: get\n  operationId: getSolarPanel\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /panel/{panel_id}\n  method: delete\n  operationId: deleteSolarPanel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /location/{location_id}/interval_data\n  method: get\n  operationId: getSolarPanelIntervalData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aggregated/year\n  method: get\n  operationId: getStatisticalAggregatedYear\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aggregated/month\n  method: get\n  operationId: getStatisticalAggregatedMonth\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aggregated/day\n  method: get\n  operationId: getStatisticalAggregatedDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /map/{layer}/{z}/{x}/{y}.png\n  method: get\n  operationId: getWeatherMapTile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations\n  method: get\n  operationId: listStations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations\n  method: post\n  operationId: createStation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stations/{station_id}\n  method: get\n  operationId: getStation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stations/{station_id}\n  method: put\n  operationId: updateStation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stations/{station_id}\n  method: delete\n  operationId: deleteStation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /measurements\n  method: get\n  operationId: getMeasurements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /measurements\n  method: post\n  operationId: postMeasurements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openweathermap/refs/heads/main/agentic-access/openweathermap-agentic-access.yml
summary_line: 42 operations · 9 acting
tags:
- Weather
- Forecast
- Climate
- Air Pollution
- Air Quality
- Solar
- Geocoding
- History
- Maps
- Road Risk
- Public APIs
---
