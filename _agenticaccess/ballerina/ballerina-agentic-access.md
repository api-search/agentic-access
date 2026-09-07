---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: ballerina-packages-api-openapi.yml
  format: yaml
  label: Ballerina Packages API
  slug: ballerina-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/openapi/ballerina-packages-api-openapi.yml
- filename: ballerina-connectors-api-openapi.yml
  format: yaml
  label: Ballerina Connectors API
  slug: ballerina-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/openapi/ballerina-connectors-api-openapi.yml
- filename: ballerina-triggers-api-openapi.yml
  format: yaml
  label: Ballerina Triggers API
  slug: ballerina-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/openapi/ballerina-triggers-api-openapi.yml
- filename: ballerina-docs-api-openapi.yml
  format: yaml
  label: Ballerina Docs API
  slug: ballerina-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/openapi/ballerina-docs-api-openapi.yml
consequence_counts:
  read: 6
description: 'Recommended x-agentic-access execution contracts for the Ballerina Central API, classified from the probed contract. Every published operation is an anonymous read of public registry data, so every classification below is connected/read with no human-in-the-loop and no audit requirement. The write path (bal push / bal deprecate) is NOT part of this surface and is deliberately not classified here — it is a credentialed CLI operation, not an HTTP endpoint an agent can be handed. Regenerated after the contract in this repo was replaced: the previous version classified nine operations, five of which do not exist on the live API.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ballerina Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Ballerina exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ballerina
provider_slug: ballerina
slug: ballerina-agentic-access
source_filename: ballerina-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: generated\nsource: openapi/_original/ballerina-central-api.yml (probed 2026-09-04)\ndescription: \"Recommended x-agentic-access execution contracts for the Ballerina Central API, classified\\\n  \\ from the probed contract. Every published operation is an anonymous read of public registry data,\\\n  \\ so every classification below is connected/read with no human-in-the-loop and no audit requirement.\\\n  \\ The write path (bal push / bal deprecate) is NOT part of this surface and is deliberately not classified\\\n  \\ here \\u2014 it is a credentialed CLI operation, not an HTTP endpoint an agent can be handed. Regenerated\\\n  \\ after the contract in this repo was replaced: the previous version classified nine operations, five\\\n  \\ of which do not exist on the live API.\"\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /2.0/registry/packages\n\
  \  method: get\n  operationId: searchPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2.0/registry/search-packages\n  method: get\n  operationId: fullTextSearchPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2.0/registry/packages/{orgName}/{packageName}\n  method: get\n  operationId: listPackageVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2.0/registry/connectors\n  method: get\n  operationId: searchConnectors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2.0/registry/triggers\n  method: get\n  operationId: searchTriggers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2.0/docs/{orgName}/{packageName}/{version}\n  method: get\n  operationId: getPackageApiDocs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ballerina/refs/heads/main/agentic-access/ballerina-agentic-access.yml
summary_line: 6 operations
tags:
- Integration
- Orchestrations
- Open-Source
- Programming Language
- Package Registry
- Developer Tools
- Code Generation
- Agent Skills
---
