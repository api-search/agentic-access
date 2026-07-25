---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: biorxiv-details-api-openapi.yml
  format: yaml
  label: bioRxiv Details API
  slug: biorxiv-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biorxiv/refs/heads/main/openapi/biorxiv-details-api-openapi.yml
- filename: biorxiv-funder-api-openapi.yml
  format: yaml
  label: bioRxiv Funder API
  slug: biorxiv-funder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biorxiv/refs/heads/main/openapi/biorxiv-funder-api-openapi.yml
- filename: biorxiv-pub-api-openapi.yml
  format: yaml
  label: bioRxiv Pub API
  slug: biorxiv-pub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biorxiv/refs/heads/main/openapi/biorxiv-pub-api-openapi.yml
- filename: biorxiv-publisher-api-openapi.yml
  format: yaml
  label: bioRxiv Publisher API
  slug: biorxiv-publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biorxiv/refs/heads/main/openapi/biorxiv-publisher-api-openapi.yml
- filename: biorxiv-pubs-api-openapi.yml
  format: yaml
  label: bioRxiv Pubs API
  slug: biorxiv-pubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biorxiv/refs/heads/main/openapi/biorxiv-pubs-api-openapi.yml
- filename: biorxiv-sum-api-openapi.yml
  format: yaml
  label: bioRxiv Sum API
  slug: biorxiv-sum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biorxiv/refs/heads/main/openapi/biorxiv-sum-api-openapi.yml
- filename: biorxiv-usage-api-openapi.yml
  format: yaml
  label: bioRxiv Usage API
  slug: biorxiv-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biorxiv/refs/heads/main/openapi/biorxiv-usage-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Biorxiv Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'bioRxiv exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: bioRxiv
provider_slug: biorxiv
slug: biorxiv-agentic-access
source_filename: biorxiv-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /details/{server}/{interval}/{cursor}/{format}\n  method: get\n  operationId: getContentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /details/{server}/{doi}/na/{format}\n  method: get\n  operationId: getContentDetailsByDOI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pubs/{server}/{interval}/{cursor}\n\
  \  method: get\n  operationId: getPublishedPreprintDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pubs/{server}/{doi}/na/{format}\n  method: get\n  operationId: getPublishedPreprintByDOI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pub/{interval}/{cursor}/{format}\n  method: get\n  operationId: getPublishedArticleDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{publisherPrefix}/{interval}/{cursor}\n  method: get\n  operationId: getPublisherArticleDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funder/{server}/{interval}/{funderRorId}/{cursor}/{format}\n\
  \  method: get\n  operationId: getFunderFilteredContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sum/{interval}/{format}\n  method: get\n  operationId: getContentSummaryStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage/{interval}/{server}/{format}\n  method: get\n  operationId: getUsageSummaryStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biorxiv/refs/heads/main/agentic-access/biorxiv-agentic-access.yml
summary_line: 9 operations
tags:
- Biology
- Preprints
- Research
- Open Access
- Life Sciences
- Scientific Publications
---
