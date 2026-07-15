---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: contentful-openapi.yml
  format: yaml
  label: Contentful Content Delivery API
  slug: contentful-content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentful/refs/heads/main/openapi/contentful-openapi.yml
- filename: contentful-webhooks-asyncapi.yml
  format: yaml
  label: Contentful Webhooks
  slug: contentful-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentful/refs/heads/main/openapi/contentful-webhooks-asyncapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Contentful Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Contentful exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Contentful
provider_slug: contentful
slug: contentful-agentic-access
source_filename: contentful-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/contentful-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /spaces/{space_id}\n  method: get\n  operationId: getSpace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/environments/{environment_id}/content_types\n  method: get\n  operationId: getContentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/environments/{environment_id}/content_types/{content_type_id}\n\
  \  method: get\n  operationId: getContentType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/environments/{environment_id}/entries\n  method: get\n  operationId: getEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/environments/{environment_id}/entries/{entry_id}\n  method: get\n  operationId: getEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/environments/{environment_id}/assets\n  method: get\n  operationId: getAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/environments/{environment_id}/assets/{asset_id}\n\
  \  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/environments/{environment_id}/locales\n  method: get\n  operationId: getLocales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/environments/{environment_id}/tags\n  method: get\n  operationId: getTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spaces/{space_id}/environments/{environment_id}/sync\n  method: get\n  operationId: sync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contentful/refs/heads/main/agentic-access/contentful-agentic-access.yml
summary_line: 10 operations
tags:
- CMS
- Content
---
