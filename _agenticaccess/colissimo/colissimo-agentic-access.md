---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 4
api_specs:
- filename: colissimo-description-et-exemples-des-m-thodes-du-ws-sls-api-openapi.yml
  format: yaml
  label: Colissimo Description et exemples des méthodes du WS SLS API
  slug: colissimo-description-et-exemples-des-m-thodes-du-ws-sls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colissimo/refs/heads/main/openapi/colissimo-description-et-exemples-des-m-thodes-du-ws-sls-api-openapi.yml
- filename: colissimo-g-n-ration-de-bordereau-de-d-pot-api-openapi.yml
  format: yaml
  label: Colissimo Génération de bordereau de dépot API
  slug: colissimo-g-n-ration-de-bordereau-de-d-pot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colissimo/refs/heads/main/openapi/colissimo-g-n-ration-de-bordereau-de-d-pot-api-openapi.yml
- filename: colissimo-slsinternalservice-services-destin-s-aux-applications-internes-api-openapi.yml
  format: yaml
  label: 'Colissimo SlsInternalService : Services destinés aux applications internes API'
  slug: colissimo-slsinternalservice-services-destin-s-aux-applications-internes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colissimo/refs/heads/main/openapi/colissimo-slsinternalservice-services-destin-s-aux-applications-internes-api-openapi.yml
- filename: colissimo-slsservicews-documentation-api-openapi.yml
  format: yaml
  label: 'Colissimo SlsServiceWS : documentation API'
  slug: colissimo-slsservicews-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/colissimo/refs/heads/main/openapi/colissimo-slsservicews-documentation-api-openapi.yml
consequence_counts:
  physical: 1
  read: 4
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Colissimo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /generateBordereauByParcelsNumbers
operation_count: 12
overview: 'Colissimo exposes 12 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 7 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Colissimo
provider_slug: colissimo
slug: colissimo-agentic-access
source_filename: colissimo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/colissimo-sls-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 8\n    connected: 4\n  by_consequence:\n    write: 7\n    read: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /checkGenerateLabel\n  method: post\n  operationId: checkGenerateLabel_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generateLabel\n  method: post\n  operationId: generateLabel_1\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getLabel\n  method: post\n  operationId: getLabel_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generateCN23\n  method: post\n  operationId: generateCN23_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getListMailBoxPickingDates\n  method: post\n  operationId: getListMailBoxPickingDates_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /SlsInternalService/checkInfoPlanPickup\n  method: post\n  operationId: checkInfoPlanPickup_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /SlsInternalService/getListMailBoxPickingDates\n  method: post\n  operationId: getListMailBoxPickingDates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SlsInternalService/planPickup\n  method: post\n  operationId: planPickup_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /generateBordereauByParcelsNumbers\n  method: post\n  operationId: generateBordereauByParcelsNumbers_1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generateToken\n  method: post\n  operationId: generateToken_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getProductInter\n  method: post\n  operationId: getProductInter_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /planPickup\n  method: post\n  operationId: planPickup_2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colissimo/refs/heads/main/agentic-access/colissimo-agentic-access.yml
summary_line: 12 operations · 8 acting
tags:
- Company
- Shipping
- Logistics
- Parcel
- Labels
- Pickup Points
- France
---
