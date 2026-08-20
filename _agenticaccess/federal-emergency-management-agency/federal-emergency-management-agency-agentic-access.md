---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: federal-emergency-management-agency-assistance-api-openapi.yml
  format: yaml
  label: Federal Emergency Management Agency Assistance API
  slug: federal-emergency-management-agency-assistance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-emergency-management-agency/refs/heads/main/openapi/federal-emergency-management-agency-assistance-api-openapi.yml
- filename: federal-emergency-management-agency-disasters-api-openapi.yml
  format: yaml
  label: Federal Emergency Management Agency Disasters API
  slug: federal-emergency-management-agency-disasters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-emergency-management-agency/refs/heads/main/openapi/federal-emergency-management-agency-disasters-api-openapi.yml
- filename: federal-emergency-management-agency-metadata-api-openapi.yml
  format: yaml
  label: Federal Emergency Management Agency Metadata API
  slug: federal-emergency-management-agency-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-emergency-management-agency/refs/heads/main/openapi/federal-emergency-management-agency-metadata-api-openapi.yml
- filename: federal-emergency-management-agency-nfip-api-openapi.yml
  format: yaml
  label: Federal Emergency Management Agency NFIP API
  slug: federal-emergency-management-agency-nfip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-emergency-management-agency/refs/heads/main/openapi/federal-emergency-management-agency-nfip-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Federal Emergency Management Agency Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Federal Emergency Management Agency exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Federal Emergency Management Agency
provider_slug: federal-emergency-management-agency
slug: federal-emergency-management-agency-agentic-access
source_filename: federal-emergency-management-agency-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openfema.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/DisasterDeclarationsSummaries\n  method: get\n  operationId: listDisasterDeclarationsSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/FemaWebDisasterDeclarations\n  method: get\n  operationId: listFemaWebDisasterDeclarations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/DeclarationDenials\n  method: get\n  operationId: listDeclarationDenials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/PublicAssistanceFundedProjectsDetails\n  method: get\n  operationId: listPublicAssistanceFundedProjectsDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/IndividualAssistanceHousingRegistrantsLargeDisasters\n  method: get\n  operationId: listIndividualAssistanceHousingRegistrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/HazardMitigationGrantProgramDisasterSummaries\n  method: get\n  operationId: listHazardMitigationGrantProgramDisasterSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/FimaNfipPolicies\n  method: get\n  operationId: listFimaNfipPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/FimaNfipClaims\n  method: get\n  operationId: listFimaNfipClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/NfipCommunityStatusBook\n  method: get\n  operationId: listNfipCommunityStatusBook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/OpenFemaDataSets\n  method: get\n  operationId: listOpenFemaDataSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/FemaRegions\n\
  \  method: get\n  operationId: listFemaRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-emergency-management-agency/refs/heads/main/agentic-access/federal-emergency-management-agency-agentic-access.yml
summary_line: 11 operations
tags:
- Disasters
- Emergencies
- Federal-Government
- Flood Insurance
- Hazard Mitigation
---
