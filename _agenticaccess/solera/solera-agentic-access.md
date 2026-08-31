---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 18
api_specs:
- filename: solera-assignment-api-openapi.yml
  format: yaml
  label: Solera Assignment API
  slug: solera-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-assignment-api-openapi.yml
- filename: solera-estimatereturn-api-openapi.yml
  format: yaml
  label: Solera Estimate Return API
  slug: solera-estimatereturn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-estimatereturn-api-openapi.yml
- filename: solera-getclaimimageresponse-api-openapi.yml
  format: yaml
  label: Solera Get Claim Image Response API
  slug: solera-getclaimimageresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getclaimimageresponse-api-openapi.yml
- filename: solera-getdocument-api-openapi.yml
  format: yaml
  label: Solera Get Document API
  slug: solera-getdocument-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getdocument-api-openapi.yml
- filename: solera-getdocuments-api-openapi.yml
  format: yaml
  label: Solera Get Documents API
  slug: solera-getdocuments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getdocuments-api-openapi.yml
- filename: solera-getimage-api-openapi.yml
  format: yaml
  label: Solera Get Image API
  slug: solera-getimage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getimage-api-openapi.yml
- filename: solera-getvaluation-api-openapi.yml
  format: yaml
  label: Solera Get Valuation API
  slug: solera-getvaluation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getvaluation-api-openapi.yml
- filename: solera-getvaluationresponse-api-openapi.yml
  format: yaml
  label: Solera Get Valuation Response API
  slug: solera-getvaluationresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getvaluationresponse-api-openapi.yml
- filename: solera-gicintegration-api-openapi.yml
  format: yaml
  label: Solera GIC Integration API
  slug: solera-gicintegration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-gicintegration-api-openapi.yml
- filename: solera-valuationreturn-api-openapi.yml
  format: yaml
  label: Solera Valuation Return API
  slug: solera-valuationreturn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-valuationreturn-api-openapi.yml
- filename: solera-version-api-openapi.yml
  format: yaml
  label: Solera Version API
  slug: solera-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-version-api-openapi.yml
consequence_counts:
  read: 18
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Solera Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Solera exposes 26 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Solera
provider_slug: solera
slug: solera-agentic-access
source_filename: solera-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/solera-claim-images-openapi.json, openapi/solera-claim-images-prod-swagger.json,\n  openapi/solera-dashboard-assignment-openapi.json, openapi/solera-eapi-getdocument-openapi.json,\n  openapi/solera-enterprise-assignment-prod-swagger.json, openapi/solera-getdocuments-v1-openapi.json,\n  openapi/solera-getdocuments-v2-openapi.json, openapi/solera-getimage-v1-openapi.json, openapi/solera-getimage-v2-openapi.json,\n  openapi/solera-gic-integration-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 18\n    acting: 8\n  by_consequence:\n    read: 18\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/image/{ClaimImage}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/decodedFile\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v{version}/image/{ClaimImage}\n  method: get\n  operationId: valuationReturn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v{version}/image/{type}\n  method: get\n  operationId: decodeImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/assignments\n  method: post\n  operationId: AddAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/v2/assignmentRequestMessage\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/v2/assignmentAcks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/v2/EstimateReturnResponse\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/v2/GetDocument/{assignmentId}/{locator}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/v2/{type}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/v2/valuation/{type}/{processId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/v2/valuation/{type}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/v2/assignments\n  method: post\n  operationId: AddAssignment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/assignmentRequestMessage\n  method: get\n  operationId: AssignmentRequestMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/assignmentAcks\n  method: post\n  operationId: AssignmentAcks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/EstimateReturnResponse\n  method: post\n  operationId: EstimateReturnResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v{version}/GetDocument\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/v{version}/claims/{assignmentId}/document/{locator}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/v{version}/GetValuation\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/Version\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/v{version}/valuation/{type}/{processId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/v{version}/claims/document/{locator}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /api/v{version}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/GICIntegration/{workAssignmentID}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/v1/getM31EventAcks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - readAccess\n    - writeAccess\n- path: /api/Version\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - readAccess\n    - writeAccess\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/agentic-access/solera-agentic-access.yml
summary_line: 26 operations · 8 acting
tags:
- Insurance
- United States
- Property and Casualty
- Claims
- Claims Technology
- Automotive Claims
- FNOL
- Vehicle Damage Assessment
- Risk Data
- CIECA
- Insurtech
---
