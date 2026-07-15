---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: cgmix-maritime-information-exchange-openapi.yml
  format: yaml
  label: CGMIX Maritime Information Exchange API
  slug: cgmix-maritime-information-exchange
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-coast-guard/refs/heads/main/openapi/cgmix-maritime-information-exchange-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: United States Coast Guard Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'United States Coast Guard exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: United States Coast Guard
provider_slug: united-states-coast-guard
slug: united-states-coast-guard-agentic-access
source_filename: united-states-coast-guard-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cgmix-maritime-information-exchange-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /VDS/SearchAndReturn/Search.aspx\n  method: get\n  operationId: searchVesselDocumentation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /xml/PSIXData.asmx/getVesselSummaryXMLString\n  method: get\n  operationId: getVesselSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /xml/PSIXData.asmx/getVesselParticularsXMLString\n  method: get\n  operationId: getVesselParticulars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /xml/PSIXData.asmx/getVesselCasesXMLString\n  method: get\n  operationId: getVesselCases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /xml/PSIXData.asmx/getVesselDeficienciesXMLString\n  method: get\n  operationId: getVesselDeficiencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /xml/PSIXData.asmx/getVesselDocumentsXMLString\n  method: get\n  operationId: getVesselDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /xml/EquipmentData.asmx/getEquipmentDetails\n  method: get\n  operationId: getEquipmentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /xml/IIRData.asmx/getIIRReferralForEnforcementActionXMLString\n  method: get\n  operationId: getIncidentInvestigationReferral\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-coast-guard/refs/heads/main/agentic-access/united-states-coast-guard-agentic-access.yml
summary_line: 8 operations
tags:
- Federal Government
- Maritime Safety
- Vessel Documentation
- Emergency Response
- Law Enforcement
---
