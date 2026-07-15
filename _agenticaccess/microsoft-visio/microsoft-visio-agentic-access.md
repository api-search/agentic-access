---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: microsoft-visio-graph-api.yaml
  format: yaml
  label: Microsoft Graph Visio API
  slug: microsoft-graph-visio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/openapi/microsoft-visio-graph-api.yaml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Visio Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Microsoft Visio exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Visio
provider_slug: microsoft-visio
slug: microsoft-visio-agentic-access
source_filename: microsoft-visio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-visio-graph-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /me/drive/items/{item-id}/workbook\n  method: get\n  operationId: getVisioDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.Read\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/pages\n  method: get\n  operationId: listPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n    scope:\n    - Files.Read\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/pages/{page-id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.Read\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/pages/{page-id}/shapes\n  method: get\n  operationId: listShapes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.Read\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/pages/{page-id}/shapes/{shape-id}\n  method: get\n  operationId: getShape\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.Read\n    - Files.ReadWrite\n\
  - path: /me/drive/items/{item-id}/workbook/pages/{page-id}/shapes/{shape-id}/shapeDataItems\n  method: get\n  operationId: listShapeDataItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.Read\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/pages/{page-id}/shapes/{shape-id}/comments\n  method: get\n  operationId: listShapeComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.Read\n    - Files.ReadWrite\n- path: /me/drive/items/{item-id}/workbook/pages/{page-id}/shapes/{shape-id}/hyperlinks\n  method: get\n  operationId: listShapeHyperlinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - Files.Read\n    - Files.ReadWrite\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-visio/refs/heads/main/agentic-access/microsoft-visio-agentic-access.yml
summary_line: 8 operations
tags:
- Business Process
- Diagramming
- Flowcharts
- Microsoft 365
- Visualization
---
