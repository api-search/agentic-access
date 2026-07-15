---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 9
api_specs:
- filename: ptc-thingworx-rest-openapi.yml
  format: yaml
  label: PTC ThingWorx REST API
  slug: thingworx-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/openapi/ptc-thingworx-rest-openapi.yml
- filename: ptc-thingworx-websocket-asyncapi.yml
  format: yaml
  label: PTC ThingWorx WebSocket/AlwaysOn API
  slug: thingworx-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/asyncapi/ptc-thingworx-websocket-asyncapi.yml
consequence_counts:
  read: 9
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ptc Thingworx Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'ptc-thingworx exposes 11 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ptc-thingworx
provider_slug: ptc-thingworx
slug: ptc-thingworx-agentic-access
source_filename: ptc-thingworx-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ptc-thingworx-rest-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 9\n    acting: 2\n  by_consequence:\n    read: 9\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /Things\n  method: get\n  operationId: listThings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Things/{thingName}\n  method: get\n  operationId: getThing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Things/{thingName}/Properties\n  method:\
  \ get\n  operationId: getThingProperties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Things/{thingName}/Properties/{propertyName}\n  method: get\n  operationId: getThingProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Things/{thingName}/Properties/{propertyName}\n  method: put\n  operationId: setThingProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Things/{thingName}/Properties/{propertyName}/QueryPropertyHistory\n  method: get\n  operationId: queryPropertyHistory\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Things/{thingName}/Services/{serviceName}\n  method: post\n  operationId: executeService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Things/{thingName}/Events\n  method: get\n  operationId: getThingEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Things/{thingName}/EventHistory\n  method: get\n  operationId: getEventHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ThingTemplates\n  method: get\n  operationId: listThingTemplates\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DataShapes/{dataShapeName}\n  method: get\n  operationId: getDataShape\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/agentic-access/ptc-thingworx-agentic-access.yml
summary_line: 11 operations · 2 acting
tags: []
---
