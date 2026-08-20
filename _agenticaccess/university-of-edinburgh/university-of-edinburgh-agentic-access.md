---
acting_count: 0
action_class_counts:
  connected: 14
api_specs:
- filename: university-of-edinburgh-datashare-repository-api-openapi.yml
  format: yaml
  label: Edinburgh DataShare REST API
  slug: datashare-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-datashare-repository-api-openapi.yml
- filename: university-of-edinburgh-datashare-oai-pmh-openapi.yml
  format: yaml
  label: Edinburgh DataShare OAI-PMH
  slug: datashare-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-datashare-oai-pmh-openapi.yml
- filename: university-of-edinburgh-era-repository-api-openapi.yml
  format: yaml
  label: Edinburgh Research Archive (ERA) REST API
  slug: era-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-era-repository-api-openapi.yml
- filename: university-of-edinburgh-era-oai-pmh-openapi.yml
  format: yaml
  label: Edinburgh Research Archive (ERA) OAI-PMH
  slug: era-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-era-oai-pmh-openapi.yml
- filename: university-of-edinburgh-eidf-data-catalogue-api-openapi.yml
  format: yaml
  label: EIDF Data Catalogue API
  slug: eidf-data-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-eidf-data-catalogue-api-openapi.yml
- filename: university-of-edinburgh-elm-api-openapi.yml
  format: yaml
  label: ELM — Edinburgh Language Models API
  slug: elm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-elm-api-openapi.yml
consequence_counts:
  generate: 1
  read: 13
description: 'Recommended x-agentic-access execution contracts for the institution-operated University of Edinburgh surfaces, derived from the probed OpenAPI documents in this repository. A governance starting point for exposing these APIs to AI agents — review and bind audience per deployment. Regenerated on 2026-08-19: the previous version was derived from the retired DSpace 6 legacy /rest API and classified twenty operations that no longer exist.'
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: derived
name: University Of Edinburgh Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'University of Edinburgh exposes 14 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: University of Edinburgh
provider_slug: university-of-edinburgh
slug: university-of-edinburgh-agentic-access
source_filename: university-of-edinburgh-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: derived\nsource: openapi/university-of-edinburgh-datashare-repository-api-openapi.yml\noperator: institution\ndescription: >-\n  Recommended x-agentic-access execution contracts for the institution-operated\n  University of Edinburgh surfaces, derived from the probed OpenAPI documents in this\n  repository. A governance starting point for exposing these APIs to AI agents — review\n  and bind audience per deployment. Regenerated on 2026-08-19: the previous version was\n  derived from the retired DSpace 6 legacy /rest API and classified twenty operations\n  that no longer exist.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 14\n  by_consequence:\n    read: 13\n    generate: 1\n  human_in_the_loop_required: 1\noperations:\n\n- api: Edinburgh DataShare REST API\n  path: /\n  method: get\n  operationId: getRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n    note: Anonymous. Safe\
  \ for unattended agent use.\n- api: Edinburgh DataShare REST API\n  path: /core/communities\n  method: get\n  operationId: listCommunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n- api: Edinburgh DataShare REST API\n  path: /core/collections\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n- api: Edinburgh DataShare REST API\n  path: /discover/search/objects\n  method: get\n  operationId: searchObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n    note: Preferred anonymous route to item metadata, since /core/items requires auth.\n- api: Edinburgh DataShare REST API\n  path: /discover/browses\n  method: get\n  operationId: listBrowses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n- api: Edinburgh DataShare REST API\n  path: /core/items\n\
  \  method: get\n  operationId: listItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: authenticated\n    note: Returns 401 anonymously on this deployment. Agents must hold a University credential.\n- api: Edinburgh DataShare REST API\n  path: /core/bitstreams\n  method: get\n  operationId: listBitstreams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: authenticated\n    note: Returns 401 anonymously. Bitstreams are the binary research data — treat egress as sensitive.\n\n- api: Edinburgh Research Archive (ERA) REST API\n  path: /core/communities\n  method: get\n  operationId: listCommunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n- api: Edinburgh Research Archive (ERA) REST API\n  path: /discover/search/objects\n  method: get\n  operationId: searchObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n\
  \n- api: Edinburgh DataShare OAI-PMH\n  path: /request\n  method: get\n  operationId: oaiRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n    note: >-\n      Fully anonymous bulk metadata harvesting. Agents must respect resumptionToken flow\n      control and must not treat HTTP 200 as success — OAI returns protocol errors with 200.\n- api: Edinburgh Research Archive (ERA) OAI-PMH\n  path: /request\n  method: get\n  operationId: oaiRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n\n- api: EIDF Data Catalogue API\n  path: /package_search\n  method: get\n  operationId: packageSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n- api: EIDF Data Catalogue API\n  path: /package_show\n  method: get\n  operationId: packageShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n\n- api: ELM\
  \ — Edinburgh Language Models API\n  path: /chat/completions\n  method: post\n  operationId: createChatCompletion\n  x-agentic-access:\n    action-class: connected\n    consequence: generate\n    audience: authenticated\n    human-in-the-loop: required\n    note: >-\n      Generative inference against a University-operated LLM gateway, billed and governed\n      under Edinburgh's own generative-AI guidance. Requires a bearer token, has no public\n      self-service registration, and should not be driven unattended by an agent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/agentic-access/university-of-edinburgh-agentic-access.yml
summary_line: 14 operations · 1 human-in-the-loop
tags:
- University
- Higher Education
- Education
- United Kingdom
- Scotland
- Russell Group
- Research Repository
- Open Data
- Identity Federation
- Research Computing
- OAI-PMH
- Artificial Intelligence
---
