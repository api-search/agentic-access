---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: national-park-service-activities-api-openapi.yml
  format: yaml
  label: National Park Service Activities API
  slug: national-park-service-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-activities-api-openapi.yml
- filename: national-park-service-alerts-api-openapi.yml
  format: yaml
  label: National Park Service Alerts API
  slug: national-park-service-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-alerts-api-openapi.yml
- filename: national-park-service-articles-api-openapi.yml
  format: yaml
  label: National Park Service Articles API
  slug: national-park-service-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-articles-api-openapi.yml
- filename: national-park-service-campgrounds-api-openapi.yml
  format: yaml
  label: National Park Service Campgrounds API
  slug: national-park-service-campgrounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-campgrounds-api-openapi.yml
- filename: national-park-service-events-api-openapi.yml
  format: yaml
  label: National Park Service Events API
  slug: national-park-service-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-events-api-openapi.yml
- filename: national-park-service-newsreleases-api-openapi.yml
  format: yaml
  label: National Park Service Newsreleases API
  slug: national-park-service-newsreleases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-newsreleases-api-openapi.yml
- filename: national-park-service-parks-api-openapi.yml
  format: yaml
  label: National Park Service Parks API
  slug: national-park-service-parks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-parks-api-openapi.yml
- filename: national-park-service-people-api-openapi.yml
  format: yaml
  label: National Park Service People API
  slug: national-park-service-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-people-api-openapi.yml
- filename: national-park-service-places-api-openapi.yml
  format: yaml
  label: National Park Service Places API
  slug: national-park-service-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-places-api-openapi.yml
- filename: national-park-service-topics-api-openapi.yml
  format: yaml
  label: National Park Service Topics API
  slug: national-park-service-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-topics-api-openapi.yml
- filename: national-park-service-visitorcenters-api-openapi.yml
  format: yaml
  label: National Park Service Visitorcenters API
  slug: national-park-service-visitorcenters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-visitorcenters-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: National Park Service Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'National Park Service exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: National Park Service
provider_slug: national-park-service
slug: national-park-service-agentic-access
source_filename: national-park-service-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/national-park-service-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /parks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsreleases\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visitorcenters\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campgrounds\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activities\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/agentic-access/national-park-service-agentic-access.yml
summary_line: 11 operations
tags:
- Conservation
- Federal Government
- Parks
---
