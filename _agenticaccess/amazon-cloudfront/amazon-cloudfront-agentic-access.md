---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 4
api_specs:
- filename: amazon-cloudfront-openapi.yml
  format: yaml
  label: Amazon CloudFront API
  slug: amazon-cloudfront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/openapi/amazon-cloudfront-openapi.yml
consequence_counts:
  read: 4
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Cloudfront Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Amazon CloudFront exposes 9 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon CloudFront
provider_slug: amazon-cloudfront
slug: amazon-cloudfront-agentic-access
source_filename: amazon-cloudfront-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-cloudfront-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 5\n    connected: 4\n  by_consequence:\n    write: 5\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /2020-05-31/distribution\n  method: post\n  operationId: CreateDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-05-31/distribution\n  method: get\n  operationId: ListDistributions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-05-31/distribution/{Id}\n  method: get\n  operationId: GetDistribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-05-31/distribution/{Id}\n  method: delete\n  operationId: DeleteDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-05-31/distribution/{Id}/config\n  method: put\n  operationId: UpdateDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-05-31/distribution/{DistributionId}/invalidation\n  method: post\n  operationId: CreateInvalidation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-05-31/distribution/{DistributionId}/invalidation\n  method: get\n  operationId: ListInvalidations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-05-31/function\n  method: post\n  operationId: CreateFunction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-05-31/function\n  method: get\n  operationId: ListFunctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/agentic-access/amazon-cloudfront-agentic-access.yml
summary_line: 9 operations · 5 acting
tags:
- CloudFront
- CDN
- Content Delivery
- Edge
---
