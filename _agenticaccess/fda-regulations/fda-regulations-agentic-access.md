---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: fda-regulations-fda-data-dashboard-api-api-openapi.yml
  format: yaml
  label: FDA Regulations FDA Data Dashboard API
  slug: fda-regulations-fda-data-dashboard-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fda-regulations/refs/heads/main/openapi/fda-regulations-fda-data-dashboard-api-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts for the FDA Data Dashboard API. The mechanical classifier treated all four operations as writes because the API uses HTTP POST; corrected here against the provider's own documentation, which describes every endpoint as "Search and retrieve ... data" over a read-only public dataset. POST is used only to carry the JSON filter/column/sort body, not to mutate state. A governance starting point — review and bind audience per deployment.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fda Regulations Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'FDA Regulations exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FDA Regulations
provider_slug: fda-regulations
slug: fda-regulations-agentic-access
source_filename: fda-regulations-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: generated\nsource: openapi/fda-regulations-data-dashboard-openapi.yml\ndescription: Recommended x-agentic-access execution contracts for the FDA Data Dashboard API. The mechanical\n  classifier treated all four operations as writes because the API uses HTTP POST; corrected here against\n  the provider's own documentation, which describes every endpoint as \"Search and retrieve ... data\" over\n  a read-only public dataset. POST is used only to carry the JSON filter/column/sort body, not to mutate\n  state. A governance starting point — review and bind audience per deployment.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n  - path: /import_refusals\n    method: post\n    operationId: importRefusals\n    x-agentic-access:\n      action-class: connected\n      consequence: read\n      subject: required\n      audience: null\n      token:\n        max-ttl:\
  \ 3600\n      escalation:\n        human-in-the-loop: not-required\n      audit: recommended\n  - path: /inspections_citations\n    method: post\n    operationId: inspectionsCitations\n    x-agentic-access:\n      action-class: connected\n      consequence: read\n      subject: required\n      audience: null\n      token:\n        max-ttl: 3600\n      escalation:\n        human-in-the-loop: not-required\n      audit: recommended\n  - path: /inspections_classifications\n    method: post\n    operationId: inspectionsClassifications\n    x-agentic-access:\n      action-class: connected\n      consequence: read\n      subject: required\n      audience: null\n      token:\n        max-ttl: 3600\n      escalation:\n        human-in-the-loop: not-required\n      audit: recommended\n  - path: /compliance_actions\n    method: post\n    operationId: complianceActions\n    x-agentic-access:\n      action-class: connected\n      consequence: read\n      subject: required\n      audience: null\n  \
  \    token:\n        max-ttl: 3600\n      escalation:\n        human-in-the-loop: not-required\n      audit: recommended\ncuration_note: 'Action class downgraded acting/write -> connected/read on all 4 operations: https://datadashboard.fda.gov/oii/api/index.htm\n  documents them as dataset searches; the API exposes no create/update/delete surface.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fda-regulations/refs/heads/main/agentic-access/fda-regulations-agentic-access.yml
summary_line: 4 operations
tags:
- Regulatory Compliance
- Healthcare
- Medical Devices
- Pharmaceuticals
- Food Safety
- Inspection
- Enforcement
- Federal-Government
- Public Data
- Import
---
