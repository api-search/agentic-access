---
acting_count: 0
action_class_counts:
  connected: 22
api_specs:
- filename: acma-spectrum-licensing-openapi.yml
  format: yaml
  label: ACMA Spectrum Licensing API
  slug: spectrum-licensing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acma/refs/heads/main/openapi/acma-spectrum-licensing-openapi.yml
consequence_counts:
  read: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Acma Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'ACMA exposes 22 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ACMA
provider_slug: acma
slug: acma-agentic-access
source_filename: acma-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/acma-spectrum-licensing-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 22\n  by_consequence:\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /LicenceSearchXML\n  method: get\n  operationId: licenceSearchXML\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /LicenceSearchJSON\n  method: get\n  operationId: licenceSearchJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ClientSearchXML/{searchText}\n \
  \ method: get\n  operationId: clientSearchXML\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ClientSearchJSON/{searchText}\n  method: get\n  operationId: clientSearchJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SiteSearchXML/{searchText}\n  method: get\n  operationId: siteSearchXML\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SiteSearchJSON/{searchText}\n  method: get\n  operationId: siteSearchJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /RegistrationSearchXML\n  method: get\n  operationId: registrationSearchXML\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /RegistrationSearchJSON\n  method: get\n  operationId: registrationSearchJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccessAreaXML/{areaCode}\n  method: get\n  operationId: showAccessAreaSearchXML\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccessAreaJSON/{areaCode}\n  method: get\n  operationId: showAccessAreaSearchJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AntennaSearchXML/{searchText}\n  method: get\n  operationId: antennaSearchXML\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /AntennaSearchJSON/{searchText}\n  method: get\n  operationId: antennaSearchJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CategoryListXML\n  method: get\n  operationId: spectrumLicencesCategoryListXML\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CategoryListJSON\n  method: get\n  operationId: spectrumLicencesCategoryListJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /LicenceListXML/{licenceCategory}\n  method: get\n  operationId: spectrumLicenceListXML\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /LicenceListJSON/{licenceCategory}\n  method: get\n  operationId: spectrumLicenceListJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SiteByLocationXML/{strLatitude}/{strLongitude}\n  method: get\n  operationId: spectrumLicenceSiteSearchByLocationXML\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SiteByLocationJSON/{strLatitude}/{strLongitude}\n  method: get\n  operationId: spectrumLicenceSiteSearchByLocationJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AssignmentRangeXML\n  method: get\n  operationId: assignmentRangeXML\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /AssignmentRangeJSON\n  method: get\n  operationId: assignmentRangeJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /400MHZSearchXML/{searchText}/{searchTarget}\n  method: get\n  operationId: spectrumLicence400MHzRegisterSearchXML\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /400MHZSearchJSON/{searchText}/{searchTarget}\n  method: get\n  operationId: spectrumLicence400MHzRegisterSearchJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acma/refs/heads/main/agentic-access/acma-agentic-access.yml
summary_line: 22 operations
tags:
- Telecommunications
- Australia
- Regulator
- Spectrum
- Broadcasting
- Numbering
- Do Not Call Register
- Radio Communications
- Licensing
- Open Data
- Government
- SOAP
---
