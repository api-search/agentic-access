---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: department-of-homeland-security-openapi.yml
  format: yaml
  label: OpenFEMA API
  slug: openfema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-homeland-security/refs/heads/main/openapi/department-of-homeland-security-openapi.yml
consequence_counts:
  read: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Department Of Homeland Security Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Department of Homeland Security exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Department of Homeland Security
provider_slug: department-of-homeland-security
slug: department-of-homeland-security-agentic-access
source_filename: department-of-homeland-security-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/department-of-homeland-security-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/DisasterDeclarationsSummaries\n  method: get\n  operationId: listDisasterDeclarationsSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/FemaWebDisasterSummaries\n  method: get\n  operationId: listFemaWebDisasterSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v2/HazardMitigationGrants\n  method: get\n  operationId: listHazardMitigationGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/HousingAssistanceOwners\n  method: get\n  operationId: listHousingAssistanceOwners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/HousingAssistanceRenters\n  method: get\n  operationId: listHousingAssistanceRenters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/IndividualsAndHouseholdsProgramValidRegistrations\n  method: get\n  operationId: listIHPValidRegistrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/PublicAssistanceFundedProjectsDetails\n  method: get\n  operationId: listPublicAssistanceFundedProjectsDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/PublicAssistanceApplicants\n  method: get\n  operationId: listPublicAssistanceApplicants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/MissionAssignments\n  method: get\n  operationId: listMissionAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/EmergencyManagementPerformanceGrants\n  method: get\n  operationId: listEmergencyManagementPerformanceGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/FemaRegions\n  method: get\n  operationId: listFemaRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/FimaNfipClaims\n  method: get\n  operationId: listFimaNfipClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/FimaNfipPolicies\n  method: get\n  operationId: listFimaNfipPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/HazardMitigationAssistanceProjects\n  method: get\n  operationId: listHazardMitigationAssistanceProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-homeland-security/refs/heads/main/agentic-access/department-of-homeland-security-agentic-access.yml
summary_line: 14 operations
tags:
- CISA
- Cybersecurity
- Disaster
- Federal Government
- FEMA
- Homeland Security
- Immigration
- NTAS
- Open Data
- USCIS
---
