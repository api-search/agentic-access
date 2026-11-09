---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: behindthewatt-com-announcements-json-api-openapi.yml
  format: yaml
  label: Behind the Watt Announcements.json API
  slug: behindthewatt-com-announcements-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/behindthewatt-com/openapi/behindthewatt-com-announcements-json-api-openapi.yml
- filename: behindthewatt-com-changes-json-api-openapi.yml
  format: yaml
  label: Behind the Watt Changes.json API
  slug: behindthewatt-com-changes-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/behindthewatt-com/openapi/behindthewatt-com-changes-json-api-openapi.yml
- filename: behindthewatt-com-coverage-json-api-openapi.yml
  format: yaml
  label: Behind the Watt Coverage.json API
  slug: behindthewatt-com-coverage-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/behindthewatt-com/openapi/behindthewatt-com-coverage-json-api-openapi.yml
- filename: behindthewatt-com-events-json-api-openapi.yml
  format: yaml
  label: Behind the Watt Events.json API
  slug: behindthewatt-com-events-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/behindthewatt-com/openapi/behindthewatt-com-events-json-api-openapi.yml
- filename: behindthewatt-com-facilities-json-api-openapi.yml
  format: yaml
  label: Behind the Watt Facilities.json API
  slug: behindthewatt-com-facilities-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/behindthewatt-com/openapi/behindthewatt-com-facilities-json-api-openapi.yml
- filename: behindthewatt-com-fleet-csv-api-openapi.yml
  format: yaml
  label: Behind the Watt Fleet.csv API
  slug: behindthewatt-com-fleet-csv-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/behindthewatt-com/openapi/behindthewatt-com-fleet-csv-api-openapi.yml
- filename: behindthewatt-com-index-json-api-openapi.yml
  format: yaml
  label: Behind the Watt Index.json API
  slug: behindthewatt-com-index-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/behindthewatt-com/openapi/behindthewatt-com-index-json-api-openapi.yml
- filename: behindthewatt-com-opsb-review-json-api-openapi.yml
  format: yaml
  label: Behind the Watt Opsb Review.json API
  slug: behindthewatt-com-opsb-review-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/behindthewatt-com/openapi/behindthewatt-com-opsb-review-json-api-openapi.yml
- filename: behindthewatt-com-research-projects-json-api-openapi.yml
  format: yaml
  label: Behind the Watt Research Projects.json API
  slug: behindthewatt-com-research-projects-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/behindthewatt-com/openapi/behindthewatt-com-research-projects-json-api-openapi.yml
- filename: behindthewatt-com-summary-json-api-openapi.yml
  format: yaml
  label: Behind the Watt Summary.json API
  slug: behindthewatt-com-summary-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/behindthewatt-com/openapi/behindthewatt-com-summary-json-api-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Behindthewatt Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Behind the Watt exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Behind the Watt
provider_slug: behindthewatt-com
slug: behindthewatt-com-agentic-access
source_filename: behindthewatt-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/behindthewatt-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/index.json\n  method: get\n  operationId: getAPImanifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/facilities.json\n  method: get\n  operationId: getVerifiedfacilitieswithunitspermitsandsourcereceipts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/announcements.json\n  method: get\n  operationId: getThirdpartyreportedprojectpipeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/events.json\n  method: get\n  operationId: getChronologicalpublicevents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/changes.json\n  method: get\n  operationId: getReviewedchangeinterpretationsandpublishedmirrorevents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/opsb-review.json\n  method: get\n  operationId: getExact44OPSBdocketrecordsandincompletecontentreviewstate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /api/v1/research-projects.json\n  method: get\n  operationId: getSelectedprimarysourceprojectresearchdistinctfromoperatingfleet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/summary.json\n  method: get\n  operationId: getVerifiedfleetsummaryanddatasetdate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/coverage.json\n  method: get\n  operationId: getSourcemonitoringcoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fleet.csv\n  method: get\n  operationId: getFlatverifiedfleetCSV\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://artifacts.apis.io/behindthewatt-com/agentic-access/behindthewatt-com-agentic-access.yml
summary_line: 10 operations
tags:
- Energy
- Data Center
- Open Data
- Power
- Economics
- Tracking
---
