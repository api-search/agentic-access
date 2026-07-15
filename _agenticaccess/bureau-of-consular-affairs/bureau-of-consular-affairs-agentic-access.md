---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 15
api_specs:
- filename: bureau-of-consular-affairs-openapi.yml
  format: yaml
  label: Bureau of Consular Affairs Data Catalog (CKAN API)
  slug: ca-data-catalog-ckan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-consular-affairs/refs/heads/main/openapi/bureau-of-consular-affairs-openapi.yml
consequence_counts:
  read: 15
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bureau Of Consular Affairs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Bureau of Consular Affairs exposes 18 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bureau of Consular Affairs
provider_slug: bureau-of-consular-affairs
slug: bureau-of-consular-affairs-agentic-access
source_filename: bureau-of-consular-affairs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bureau-of-consular-affairs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 15\n    acting: 3\n  by_consequence:\n    read: 15\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /action/site_read\n  method: get\n  operationId: siteRead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/package_list\n  method: get\n  operationId: packageList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/current_package_list_with_resources\n\
  \  method: get\n  operationId: currentPackageListWithResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/package_show\n  method: get\n  operationId: packageShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/package_search\n  method: get\n  operationId: packageSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/resource_show\n  method: get\n  operationId: resourceShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/resource_search\n  method: get\n  operationId: resourceSearch\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/group_list\n  method: get\n  operationId: groupList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/group_show\n  method: get\n  operationId: groupShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/organization_list\n  method: get\n  operationId: organizationList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/organization_show\n  method: get\n  operationId: organizationShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/tag_list\n\
  \  method: get\n  operationId: tagList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/tag_show\n  method: get\n  operationId: tagShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/datastore_search\n  method: get\n  operationId: datastoreSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/datastore_search_sql\n  method: get\n  operationId: datastoreSearchSql\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /action/package_create\n  method: post\n  operationId: packageCreate\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /action/package_update\n  method: post\n  operationId: packageUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /action/package_delete\n  method: post\n  operationId: packageDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-consular-affairs/refs/heads/main/agentic-access/bureau-of-consular-affairs-agentic-access.yml
summary_line: 18 operations · 3 acting
tags:
- Federal Government
- Passports
- Travel
- Travel Advisories
- Visas
---
