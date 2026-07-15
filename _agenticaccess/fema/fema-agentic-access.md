---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: fema-openapi.yml
  format: yaml
  label: FEMA Disaster Declarations Summaries API
  slug: fema-disaster-declarations-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA Public Assistance Funded Projects Details API
  slug: fema-public-assistance-funded-projects-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA Hazard Mitigation Assistance Projects API
  slug: fema-hazard-mitigation-assistance-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA NFIP Redacted Policies API
  slug: fema-nfip-redacted-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA NFIP Redacted Claims API
  slug: fema-nfip-redacted-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA IPAWS Archived Alerts API
  slug: fema-ipaws-archived-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA Web Disaster Summaries API
  slug: fema-web-disaster-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
- filename: fema-openapi.yml
  format: yaml
  label: FEMA OpenFEMA Dataset Catalog API
  slug: fema-openfema-dataset-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/openapi/fema-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fema Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'OpenFEMA exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenFEMA
provider_slug: fema
slug: fema-agentic-access
source_filename: fema-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fema-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/DisasterDeclarationsSummaries\n  method: get\n  operationId: listDisasterDeclarationsSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/PublicAssistanceFundedProjectsDetails\n  method: get\n  operationId: listPublicAssistanceFundedProjectsDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v3/HazardMitigationAssistanceProjects\n  method: get\n  operationId: listHazardMitigationAssistanceProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/FimaNfipPolicies\n  method: get\n  operationId: listFimaNfipPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/FimaNfipClaims\n  method: get\n  operationId: listFimaNfipClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/IpawsArchivedAlerts\n  method: get\n  operationId: listIpawsArchivedAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/FemaWebDisasterSummaries\n\
  \  method: get\n  operationId: listFemaWebDisasterSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/OpenFemaDataSets\n  method: get\n  operationId: listOpenFemaDataSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/OpenFemaDataSetFields\n  method: get\n  operationId: listOpenFemaDataSetFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fema/refs/heads/main/agentic-access/fema-agentic-access.yml
summary_line: 9 operations
tags:
- Government
- Open Data
- Emergency Management
- Disaster
- FEMA
- Public Safety
---
