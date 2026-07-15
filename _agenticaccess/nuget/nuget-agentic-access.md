---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 13
api_specs:
- filename: nuget-server-api-openapi.yml
  format: yaml
  label: NuGet Server API
  slug: nuget-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-server-api-openapi.yml
- filename: nuget-catalog-api-openapi.yml
  format: yaml
  label: NuGet Catalog API
  slug: nuget-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-catalog-api-openapi.yml
- filename: nuget-search-api-openapi.yml
  format: yaml
  label: NuGet Search API
  slug: nuget-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-search-api-openapi.yml
- filename: nuget-package-metadata-api-openapi.yml
  format: yaml
  label: NuGet Package Metadata API
  slug: nuget-package-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-package-metadata-api-openapi.yml
- filename: nuget-package-content-api-openapi.yml
  format: yaml
  label: NuGet Package Content API
  slug: nuget-package-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-package-content-api-openapi.yml
consequence_counts:
  read: 13
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nuget Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'NuGet exposes 16 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NuGet
provider_slug: nuget
slug: nuget-agentic-access
source_filename: nuget-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nuget-catalog-api-openapi.yml, openapi/nuget-package-content-api-openapi.yml,\n  openapi/nuget-package-metadata-api-openapi.yml, openapi/nuget-search-api-openapi.yml, openapi/nuget-server-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 13\n    acting: 3\n  by_consequence:\n    read: 13\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /index.json\n  method: get\n  operationId: getCatalogIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{pageName}.json\n  method: get\n  operationId: getCatalogPage\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/{timestamp}/{packageId}.{version}.json\n  method: get\n  operationId: getCatalogLeaf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lowerId}/index.json\n  method: get\n  operationId: listPackageVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lowerId}/{lowerVersion}/{lowerId}.{lowerVersion}.nupkg\n  method: get\n  operationId: downloadPackage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lowerId}/{lowerVersion}/{lowerId}.nuspec\n  method: get\n  operationId: downloadPackageManifest\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lowerId}/index.json\n  method: get\n  operationId: getRegistrationIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lowerId}/page/{lower}/{upper}.json\n  method: get\n  operationId: getRegistrationPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lowerId}/{version}.json\n  method: get\n  operationId: getRegistrationLeaf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /query\n  method: get\n  operationId: searchPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /autocomplete\n  method: get\n  operationId: autocompletePackageIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autocomplete-versions\n  method: get\n  operationId: enumeratePackageVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /index.json\n  method: get\n  operationId: getServiceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /package\n  method: put\n  operationId: pushPackage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /package/{id}/{version}\n  method: delete\n  operationId: deletePackage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /package/{id}/{version}\n  method: post\n  operationId: relistPackage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/agentic-access/nuget-agentic-access.yml
summary_line: 16 operations · 3 acting
tags:
- Package Management
- .NET
- Packages
- Dependencies
- Software Distribution
- Registry
---
