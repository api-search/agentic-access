---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 10
api_specs:
- filename: pypi-json-api-openapi.yml
  format: yaml
  label: PyPI JSON API
  slug: json
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-json-api-openapi.yml
- filename: pypi-index-api-openapi.yml
  format: yaml
  label: PyPI Index API
  slug: index
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-index-api-openapi.yml
- filename: pypi-integrity-api-openapi.yml
  format: yaml
  label: PyPI Integrity API
  slug: integrity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-integrity-api-openapi.yml
- filename: pypi-upload-api-openapi.yml
  format: yaml
  label: PyPI Upload API
  slug: upload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-upload-api-openapi.yml
- filename: pypi-stats-api-openapi.yml
  format: yaml
  label: PyPI Stats API
  slug: stats
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/openapi/pypi-stats-api-openapi.yml
consequence_counts:
  read: 10
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pypi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'PyPI exposes 11 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PyPI
provider_slug: pypi
slug: pypi-agentic-access
source_filename: pypi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pypi-index-api-openapi.yml, openapi/pypi-integrity-api-openapi.yml, openapi/pypi-json-api-openapi.yml,\n  openapi/pypi-stats-api-openapi.yml, openapi/pypi-upload-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 10\n    acting: 1\n  by_consequence:\n    read: 10\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /simple/\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /simple/{project}/\n  method: get\n  operationId: getProjectFiles\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrity/{project}/{version}/{filename}/provenance\n  method: get\n  operationId: getFileProvenance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pypi/{project}/json\n  method: get\n  operationId: getProjectMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pypi/{project}/{version}/json\n  method: get\n  operationId: getProjectVersionMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages/{package}/recent\n  method: get\n  operationId: getRecentDownloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages/{package}/overall\n  method: get\n  operationId: getOverallDownloads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages/{package}/python_major\n  method: get\n  operationId: getDownloadsByPythonMajor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages/{package}/python_minor\n  method: get\n  operationId: getDownloadsByPythonMinor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages/{package}/system\n  method: get\n  operationId: getDownloadsBySystem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /legacy/\n  method: post\n  operationId: uploadDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/agentic-access/pypi-agentic-access.yml
summary_line: 11 operations · 1 acting
tags:
- Developer Tools
- Open Source
- Package Management
- Packages
- Python
---
