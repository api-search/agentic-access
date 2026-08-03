---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 38
api_specs:
- filename: us-dot-faa-aeronautic-product-release-api-openapi.yml
  format: yaml
  label: FAA Aeronautic Product Release API (APRA)
  slug: faa-aeronautic-product-release-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-faa-aeronautic-product-release-api-openapi.yml
- filename: us-dot-faa-air-carrier-prd-api-openapi.yml
  format: yaml
  label: FAA Air Carrier Pilot Records Database (PRD) API
  slug: faa-air-carrier-prd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-faa-air-carrier-prd-api-openapi.yml
- filename: us-dot-faa-safety-assurance-system-api-openapi.yml
  format: yaml
  label: FAA Safety Assurance System (SAS) API
  slug: faa-safety-assurance-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-faa-safety-assurance-system-api-openapi.yml
- filename: us-dot-its-jpo-ode-rest-api-openapi.yml
  format: yaml
  label: USDOT ITS JPO Operational Data Environment (ODE) REST API
  slug: its-jpo-ode-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-its-jpo-ode-rest-api-openapi.yml
- filename: us-dot-faa-airport-status-web-service-openapi.yml
  format: yaml
  label: U.S. Department of Transportation Airport Status Web Service
  slug: us-dot-faa-airport-status-web-service-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-faa-airport-status-web-service-openapi.yml
consequence_counts:
  read: 38
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Us Dot Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 53
overview: 'U.S. Department of Transportation exposes 53 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: U.S. Department of Transportation
provider_slug: us-dot
slug: us-dot-agentic-access
source_filename: us-dot-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: generated\nsource: openapi/us-dot-faa-aeronautic-product-release-api-openapi.yml, openapi/us-dot-faa-air-carrier-prd-api-openapi.yml,\n  openapi/us-dot-faa-airport-status-web-service-openapi.yml, openapi/us-dot-faa-safety-assurance-system-api-openapi.yml,\n  openapi/us-dot-its-jpo-ode-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    connected: 38\n    acting: 15\n  by_consequence:\n    read: 38\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /cifp/chart\n  method: get\n  operationId: getCIFPRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /cifp/info\n  method: get\n  operationId: getCIFPEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ddof/chart\n  method: get\n  operationId: getDDOFRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ddof/info\n  method: get\n  operationId: getDDOFEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dec/chart\n  method: get\n  operationId: getDECRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dec/info\n  method: get\n  operationId: getDECEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /ders/chart\n  method: get\n  operationId: getDERSRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ders/info\n  method: get\n  operationId: getDERSEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dtpp/chart\n  method: get\n  operationId: getTPPRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dtpp/info\n  method: get\n  operationId: getTPPEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enroute/chart\n  method: get\n  operationId: getIFREnrouteRelease\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enroute/gom/chart\n  method: get\n  operationId: getGOMRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enroute/gom/info\n  method: get\n  operationId: getGOMEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enroute/info\n  method: get\n  operationId: getIFREnrouteEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ifr/oceanic/chart\n  method: get\n  operationId: getOceanicRouteChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /ifr/oceanic/info\n  method: get\n  operationId: getOceanicRouteEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ifr/planning/chart\n  method: get\n  operationId: getIfrPlanningChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ifr/planning/info\n  method: get\n  operationId: getIfrPlanningInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nfdc/nasr/chart\n  method: get\n  operationId: getNASRSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nfdc/nasr/info\n  method: get\n  operationId: getNASREdition\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supplement/chart\n  method: get\n  operationId: getSupplementRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supplement/info\n  method: get\n  operationId: getSupplementEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vfr/grandcanyon/chart\n  method: get\n  operationId: getGrandCanyonRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vfr/grandcanyon/info\n  method: get\n  operationId: getGrandCanyonEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /vfr/helicopter/chart\n  method: get\n  operationId: getHelicopterRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vfr/helicopter/gulf/chart\n  method: get\n  operationId: getGulfCoastRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vfr/helicopter/gulf/info\n  method: get\n  operationId: getGulfCoastEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vfr/helicopter/info\n  method: get\n  operationId: getHelicopterEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vfr/sectional/chart\n  method:\
  \ get\n  operationId: getSectionalChart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vfr/sectional/info\n  method: get\n  operationId: getSectionalInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vfr/tac/chart\n  method: get\n  operationId: getTACRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vfr/tac/info\n  method: get\n  operationId: getTACEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vfr/wallplanning/chart\n  method: get\n  operationId: getProductRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vfr/wallplanning/info\n  method: get\n  operationId: getProductEdition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AirCarrierApi/Pilot\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AirCarrierApi/Pilot\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AirCarrierApi/Pilot\n  method: delete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AirCarrierApi/PilotDataTracking\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AirCarrierApi/PilotDataTracking\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AirCarrierApi/PilotDataTracking\n  method: delete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AirCarrierApi/AcPilotDataSearchRequest\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AirCarrierApi/AcPilotDataSearchResponse\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/airport/delays\n  method: get\n  operationId:\
  \ getDelays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/airport/status/{airportCode}\n  method: get\n  operationId: getAirportStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /axhsubmitdiscrepancies\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tim/query\n  method: post\n  operationId: tim_query\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tim\n  method: put\n  operationId: tim_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tim\n  method: post\n  operationId: tim_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tim\n  method: delete\n  operationId: tim_delete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rsuHeartbeat\n  method: get\n  operationId: snmp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pdm\n  method: post\n  operationId: pdm_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /upload/obulog\n  method: post\n  operationId: upload-obulog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/agentic-access/us-dot-agentic-access.yml
summary_line: 53 operations · 15 acting
tags:
- Travel
- United States
- Aviation
- Airlines
- Airports
- Government
- Regulator
- Distribution
- Aviation Consumer Protection
- Open Data
- Transportation
- Safety
- Statistics
- Automotive
- Rail
---
