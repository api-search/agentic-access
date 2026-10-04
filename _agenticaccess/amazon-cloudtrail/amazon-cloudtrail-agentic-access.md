---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: amazon-cloudtrail-event-data-stores-api-openapi.yml
  format: yaml
  label: Amazon CloudTrail Event Data Stores API
  slug: amazon-cloudtrail-event-data-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/openapi/amazon-cloudtrail-event-data-stores-api-openapi.yml
- filename: amazon-cloudtrail-events-api-openapi.yml
  format: yaml
  label: Amazon CloudTrail Events API
  slug: amazon-cloudtrail-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/openapi/amazon-cloudtrail-events-api-openapi.yml
- filename: amazon-cloudtrail-trails-api-openapi.yml
  format: yaml
  label: Amazon CloudTrail Trails API
  slug: amazon-cloudtrail-trails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/openapi/amazon-cloudtrail-trails-api-openapi.yml
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Cloudtrail Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Amazon CloudTrail exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon CloudTrail
provider_slug: amazon-cloudtrail
slug: amazon-cloudtrail-agentic-access
source_filename: amazon-cloudtrail-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/amazon-cloudtrail-event-data-stores-api-openapi.yml, openapi/amazon-cloudtrail-events-api-openapi.yml,\n  openapi/amazon-cloudtrail-trails-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 3\n    connected: 3\n  by_consequence:\n    write: 3\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /event-data-stores\n  method: post\n  operationId: CreateEventDataStore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /event-data-stores\n  method: get\n  operationId: ListEventDataStores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/lookup\n  method: post\n  operationId: LookupEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trails\n  method: post\n  operationId: CreateTrail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trails\n  method: get\n  operationId: DescribeTrails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /trails/{trailName}\n  method: delete\n  operationId: DeleteTrail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/agentic-access/amazon-cloudtrail-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- CloudTrail
- Audit
- Compliance
- Governance
- Security
---
