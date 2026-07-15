---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: plantuml-server-openapi.yml
  format: yaml
  label: PlantUML Server API
  slug: plantuml-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uml/refs/heads/main/openapi/plantuml-server-openapi.yml
- filename: kroki-openapi.yml
  format: yaml
  label: Kroki Diagram API
  slug: kroki
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uml/refs/heads/main/openapi/kroki-openapi.yml
consequence_counts:
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Uml Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'UML exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: UML
provider_slug: uml
slug: uml-agentic-access
source_filename: uml-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kroki-openapi.yml, openapi/plantuml-server-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 8\n    acting: 1\n  by_consequence:\n    read: 8\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{diagram_type}/{output_format}/{encoded_diagram}\n  method: get\n  operationId: getDiagramGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /{diagram_type}/{output_format}\n  method: post\n  operationId: postDiagram\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /png/{encoded}\n  method: get\n  operationId: getDiagramPng\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /svg/{encoded}\n  method: get\n  operationId: getDiagramSvg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /txt/{encoded}\n  method: get\n  operationId: getDiagramAscii\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /pdf/{encoded}\n  method: get\n  operationId: getDiagramPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /map/{encoded}\n  method: get\n  operationId: getDiagramImageMap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check/{encoded}\n  method: get\n  operationId: validateDiagramSyntax\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uml/refs/heads/main/agentic-access/uml-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- UML
- Modeling
- Diagrams
- Software Architecture
- Design
- Standards
---
