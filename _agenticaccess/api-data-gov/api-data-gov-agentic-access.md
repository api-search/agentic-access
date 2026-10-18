---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 24
api_specs:
- filename: api-data-gov-dataset-api-openapi.yml
  format: yaml
  label: api.data.gov Dataset API
  slug: api-data-gov-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-dataset-api-openapi.yml
- filename: api-data-gov-harvest-jobs-api-openapi.yml
  format: yaml
  label: api.data.gov Harvest Jobs API
  slug: api-data-gov-harvest-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-harvest-jobs-api-openapi.yml
- filename: api-data-gov-harvest-records-api-openapi.yml
  format: yaml
  label: api.data.gov Harvest Records API
  slug: api-data-gov-harvest-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-harvest-records-api-openapi.yml
- filename: api-data-gov-harvest-sources-api-openapi.yml
  format: yaml
  label: api.data.gov Harvest Sources API
  slug: api-data-gov-harvest-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-harvest-sources-api-openapi.yml
- filename: api-data-gov-keywords-api-openapi.yml
  format: yaml
  label: api.data.gov Keywords API
  slug: api-data-gov-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-keywords-api-openapi.yml
- filename: api-data-gov-location-api-openapi.yml
  format: yaml
  label: api.data.gov Location API
  slug: api-data-gov-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-location-api-openapi.yml
- filename: api-data-gov-locations-api-openapi.yml
  format: yaml
  label: api.data.gov Locations API
  slug: api-data-gov-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-locations-api-openapi.yml
- filename: api-data-gov-organizations-api-openapi.yml
  format: yaml
  label: api.data.gov Organizations API
  slug: api-data-gov-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-organizations-api-openapi.yml
- filename: api-data-gov-publishers-api-openapi.yml
  format: yaml
  label: api.data.gov Publishers API
  slug: api-data-gov-publishers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-publishers-api-openapi.yml
- filename: api-data-gov-search-api-openapi.yml
  format: yaml
  label: api.data.gov Search API
  slug: api-data-gov-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-search-api-openapi.yml
- filename: api-data-gov-stats-api-openapi.yml
  format: yaml
  label: api.data.gov Stats API
  slug: api-data-gov-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-stats-api-openapi.yml
- filename: api-data-gov-validate-api-openapi.yml
  format: yaml
  label: api.data.gov Validate API
  slug: api-data-gov-validate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-validate-api-openapi.yml
- filename: api-data-gov-open-search-api-openapi.yml
  format: yaml
  label: api.data.gov Open Search API
  slug: api-data-gov-open-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/openapi/api-data-gov-open-search-api-openapi.yml
consequence_counts:
  read: 24
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Api Data Gov Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'api.data.gov exposes 25 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: api.data.gov
provider_slug: api-data-gov
slug: api-data-gov-agentic-access
source_filename: api-data-gov-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/catalog.data.gov-openapi.json, openapi/harvest.data.gov-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 24\n    acting: 1\n  by_consequence:\n    read: 24\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/dataset/{slug_or_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/keywords\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/location/{location_id}\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/locations/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/opensearch/health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/publishers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/stats\n  method: get\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/harvest_error/{error_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/harvest_job/{job_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/harvest_job/{job_id}/errors/{error_type}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/harvest_job_errors/\n  method: get\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/harvest_jobs/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/harvest_record/{record_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/harvest_record/{record_id}/errors\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/harvest_record/{record_id}/raw\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/harvest_record/{record_id}/transformed\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/harvest_record_errors/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/harvest_records/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/harvest_sources/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organization/{org_identifier}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organization_list/\n  method: get\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/organizations/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/validate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-data-gov/refs/heads/main/agentic-access/api-data-gov-agentic-access.yml
summary_line: 25 operations · 1 acting
tags:
- Company
- Government
- Data
- Open Data
---
