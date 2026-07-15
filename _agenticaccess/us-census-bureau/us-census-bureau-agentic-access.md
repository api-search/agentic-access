---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 45
api_specs:
- filename: census-data-api-openapi.yml
  format: yaml
  label: Census Data API
  slug: census-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-data-api-openapi.yml
- filename: census-microdata-api-openapi.yml
  format: yaml
  label: Census Microdata API
  slug: census-microdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-microdata-api-openapi.yml
- filename: census-tigerweb-rest-openapi.yml
  format: yaml
  label: TIGERweb REST Services
  slug: census-tigerweb-rest-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-tigerweb-rest-openapi.yml
- filename: census-geocoder-api-openapi.yml
  format: yaml
  label: Census Geocoding Services API
  slug: census-geocoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-geocoder-api-openapi.yml
- filename: census-bds-api-openapi.yml
  format: yaml
  label: Business Dynamics Statistics API
  slug: census-bds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-bds-api-openapi.yml
- filename: census-international-trade-api-openapi.yml
  format: yaml
  label: International Trade API
  slug: census-international-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-international-trade-api-openapi.yml
- filename: census-population-clock-api-openapi.yml
  format: yaml
  label: Population Clock API
  slug: census-population-clock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/openapi/census-population-clock-api-openapi.yml
consequence_counts:
  read: 45
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Us Census Bureau Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 47
overview: 'US Census Bureau exposes 47 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 45 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: US Census Bureau
provider_slug: us-census-bureau
slug: us-census-bureau-agentic-access
source_filename: us-census-bureau-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/census-bds-api-openapi.yml, openapi/census-data-api-openapi.yml, openapi/census-geocoder-api-openapi.yml,\n  openapi/census-international-trade-api-openapi.yml, openapi/census-microdata-api-openapi.yml,\n  openapi/census-population-clock-api-openapi.yml, openapi/census-tigerweb-rest-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 45\n    acting: 2\n  by_consequence:\n    read: 45\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /timeseries/bds\n  method: get\n  operationId: queryBdsTimeseries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /timeseries/bds/variables.json\n  method: get\n  operationId: getBdsVariables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.json\n  method: get\n  operationId: getDiscoveryCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/acs/acs5\n  method: get\n  operationId: getAcs5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/acs/acs5/subject\n  method: get\n  operationId: getAcs5Subject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/acs/acs5/profile\n  method: get\n  operationId: getAcs5Profile\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/acs/acs1\n  method: get\n  operationId: getAcs1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/acs/acs1/supplemental\n  method: get\n  operationId: getAcs1Supplemental\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/dec/pl\n  method: get\n  operationId: getDecennialPl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/dec/dhc\n  method: get\n  operationId: getDecennialDhc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /{vintage}/cbp\n  method: get\n  operationId: getCbp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/zbp\n  method: get\n  operationId: getZbp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/abscs\n  method: get\n  operationId: getAbsCompanySummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/nonemp\n  method: get\n  operationId: getNonemployer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/pep/population\n  method: get\n  operationId: getPepPopulation\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/pep/charagegroups\n  method: get\n  operationId: getPepCharacteristics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/pulse\n  method: get\n  operationId: getHouseholdPulse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/acs/acs5/variables.json\n  method: get\n  operationId: getAcs5Variables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/acs/acs5/groups.json\n  method: get\n  operationId: getAcs5Groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /{vintage}/acs/acs5/geography.json\n  method: get\n  operationId: getAcs5Geography\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/onelineaddress\n  method: get\n  operationId: locationsOnelineAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/address\n  method: get\n  operationId: locationsAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/coordinates\n  method: get\n  operationId: locationsCoordinates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geographies/onelineaddress\n  method: get\n\
  \  operationId: geographiesOnelineAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geographies/address\n  method: get\n  operationId: geographiesAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geographies/coordinates\n  method: get\n  operationId: geographiesCoordinates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/addressbatch\n  method: post\n  operationId: batchLocations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /geographies/addressbatch\n  method: post\n  operationId: batchGeographies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timeseries/intltrade/exports/hs\n  method: get\n  operationId: queryExportsHs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeseries/intltrade/imports/hs\n  method: get\n  operationId: queryImportsHs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeseries/intltrade/exports/porths\n  method: get\n  operationId: queryExportsPortHs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeseries/intltrade/imports/porths\n  method: get\n  operationId: queryImportsPortHs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeseries/intltrade/exports/statehs\n  method: get\n  operationId: queryExportsStateHs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/acs/acs1/pums\n  method: get\n  operationId: tabulateAcs1PumsPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/acs/acs1/pums/hus\n  method: get\n  operationId: tabulateAcs1PumsHousehold\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /{vintage}/acs/acs5/pums\n  method: get\n  operationId: tabulateAcs5PumsPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/cps/basic/{month}\n  method: get\n  operationId: getCpsBasic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{vintage}/sipp/{panel}/wave{wave}\n  method: get\n  operationId: getSippWave\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /popclock/data/population/uspop.json\n  method: get\n  operationId: getUsPopClock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /popclock/data/population/world.json\n\
  \  method: get\n  operationId: getWorldPopClock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getServiceCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /TIGERweb/State_County/MapServer\n  method: get\n  operationId: getStateCountyService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /TIGERweb/State_County/MapServer/{layerId}/query\n  method: get\n  operationId: queryStateCountyLayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /TIGERweb/Tracts_Blocks/MapServer/{layerId}/query\n  method: get\n  operationId: queryTractsBlocksLayer\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /TIGERweb/PUMA_TAD_TAZ_UGA_ZCTA/MapServer/{layerId}/query\n  method: get\n  operationId: queryPumaZctaLayer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Census2020/State_County/MapServer/{layerId}/query\n  method: get\n  operationId: query2020StateCounty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Census2010/State_County/MapServer/{layerId}/query\n  method: get\n  operationId: query2010StateCounty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-census-bureau/refs/heads/main/agentic-access/us-census-bureau-agentic-access.yml
summary_line: 47 operations · 2 acting
tags:
- Government
- Federal
- Demographics
- Statistics
- Economics
- Geospatial
- Open Data
- Public Sector
---
