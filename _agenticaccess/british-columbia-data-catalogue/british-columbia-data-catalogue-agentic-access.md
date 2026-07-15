---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: british-columbia-data-catalogue-openapi.yml
  format: yaml
  label: BC Data Catalogue CKAN API
  slug: ckan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/british-columbia-data-catalogue/refs/heads/main/openapi/british-columbia-data-catalogue-openapi.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: British Columbia Data Catalogue Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'British Columbia Data Catalogue exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: British Columbia Data Catalogue
provider_slug: british-columbia-data-catalogue
slug: british-columbia-data-catalogue-agentic-access
source_filename: british-columbia-data-catalogue-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/british-columbia-data-catalogue-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /action/status_show\n  method: get\n  operationId: statusShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/package_search\n  method: get\n  operationId: packageSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/package_list\n  method:\
  \ get\n  operationId: packageList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/package_show\n  method: get\n  operationId: packageShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/current_package_list_with_resources\n  method: get\n  operationId: currentPackageListWithResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/group_list\n  method: get\n  operationId: groupList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/group_show\n  method: get\n  operationId: groupShow\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/organization_list\n  method: get\n  operationId: organizationList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/organization_show\n  method: get\n  operationId: organizationShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/resource_show\n  method: get\n  operationId: resourceShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/resource_search\n  method: get\n  operationId: resourceSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /action/tag_list\n  method: get\n  operationId: tagList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/tag_show\n  method: get\n  operationId: tagShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/british-columbia-data-catalogue/refs/heads/main/agentic-access/british-columbia-data-catalogue-agentic-access.yml
summary_line: 13 operations
tags:
- Open Data
- Government
- Canadian Government
- British Columbia
- Provincial Data
- CKAN
- Geospatial
---
