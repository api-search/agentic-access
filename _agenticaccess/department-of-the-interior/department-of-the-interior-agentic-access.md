---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: department-of-the-interior-alerts-api-openapi.yml
  format: yaml
  label: Department of the Interior Alerts API
  slug: department-of-the-interior-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-alerts-api-openapi.yml
- filename: department-of-the-interior-articles-api-openapi.yml
  format: yaml
  label: Department of the Interior Articles API
  slug: department-of-the-interior-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-articles-api-openapi.yml
- filename: department-of-the-interior-campgrounds-api-openapi.yml
  format: yaml
  label: Department of the Interior Campgrounds API
  slug: department-of-the-interior-campgrounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-campgrounds-api-openapi.yml
- filename: department-of-the-interior-counts-api-openapi.yml
  format: yaml
  label: Department of the Interior Counts API
  slug: department-of-the-interior-counts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-counts-api-openapi.yml
- filename: department-of-the-interior-dailyvalues-api-openapi.yml
  format: yaml
  label: Department of the Interior DailyValues API
  slug: department-of-the-interior-dailyvalues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-dailyvalues-api-openapi.yml
- filename: department-of-the-interior-events-api-openapi.yml
  format: yaml
  label: Department of the Interior Events API
  slug: department-of-the-interior-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-events-api-openapi.yml
- filename: department-of-the-interior-instantaneousvalues-api-openapi.yml
  format: yaml
  label: Department of the Interior InstantaneousValues API
  slug: department-of-the-interior-instantaneousvalues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-instantaneousvalues-api-openapi.yml
- filename: department-of-the-interior-parks-api-openapi.yml
  format: yaml
  label: Department of the Interior Parks API
  slug: department-of-the-interior-parks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-parks-api-openapi.yml
- filename: department-of-the-interior-sites-api-openapi.yml
  format: yaml
  label: Department of the Interior Sites API
  slug: department-of-the-interior-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-sites-api-openapi.yml
- filename: department-of-the-interior-visitorcenters-api-openapi.yml
  format: yaml
  label: Department of the Interior VisitorCenters API
  slug: department-of-the-interior-visitorcenters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-visitorcenters-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Department Of The Interior Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Department of the Interior exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Department of the Interior
provider_slug: department-of-the-interior
slug: department-of-the-interior-agentic-access
source_filename: department-of-the-interior-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nps-data-api-openapi.yml, openapi/usgs-earthquake-api-openapi.yml, openapi/usgs-water-services-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /parks\n  method: get\n  operationId: listParks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts\n  method: get\n  operationId: listAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /campgrounds\n  method: get\n  operationId: listCampgrounds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visitorcenters\n  method: get\n  operationId: listVisitorCenters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles\n  method: get\n  operationId: listArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query\n  method: get\n  operationId: queryEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /count\n  method: get\n  operationId: countEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/\n  method: get\n  operationId: getSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iv/\n  method: get\n  operationId: getInstantaneousValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dv/\n  method: get\n  operationId: getDailyValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/agentic-access/department-of-the-interior-agentic-access.yml
summary_line: 11 operations
tags:
- Federal-Government
- Public Lands
- Natural Resources
- Geospatial
---
