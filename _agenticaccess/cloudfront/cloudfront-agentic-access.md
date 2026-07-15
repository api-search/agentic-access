---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 12
api_specs:
- filename: cloudfront-openapi.yml
  format: yaml
  label: AWS CloudFront API (canonical)
  slug: canonical
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudfront/refs/heads/main/openapi/cloudfront-openapi.yml
consequence_counts:
  read: 12
  safety-critical: 2
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudfront Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /2020-05-31/origin-access-control
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /2020-05-31/origin-access-control/{Id}
operation_count: 23
overview: 'CloudFront exposes 23 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 9 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CloudFront
provider_slug: cloudfront
slug: cloudfront-agentic-access
source_filename: cloudfront-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloudfront-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 12\n    acting: 11\n  by_consequence:\n    read: 12\n    write: 9\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /2020-05-31/distribution\n  method: get\n  operationId: listDistributions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-05-31/distribution\n  method: post\n  operationId: createDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-05-31/distribution/{Id}\n  method: get\n  operationId: getDistribution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-05-31/distribution/{Id}\n  method: delete\n  operationId: deleteDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-05-31/distribution/{Id}/config\n  method: get\n  operationId: getDistributionConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /2020-05-31/distribution/{Id}/config\n  method: put\n  operationId: updateDistribution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-05-31/distribution/{DistributionId}/invalidation\n  method: get\n  operationId: listInvalidations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-05-31/distribution/{DistributionId}/invalidation\n  method: post\n  operationId: createInvalidation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /2020-05-31/distribution/{DistributionId}/invalidation/{Id}\n  method: get\n  operationId: getInvalidation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-05-31/origin-access-control\n  method: get\n  operationId: listOriginAccessControls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-05-31/origin-access-control\n  method: post\n  operationId: createOriginAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /2020-05-31/origin-access-control/{Id}\n  method:\
  \ get\n  operationId: getOriginAccessControl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-05-31/origin-access-control/{Id}\n  method: delete\n  operationId: deleteOriginAccessControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /2020-05-31/cache-policy\n  method: get\n  operationId: listCachePolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-05-31/cache-policy\n  method: post\n  operationId: createCachePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-05-31/cache-policy/{Id}\n  method: get\n  operationId: getCachePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-05-31/cache-policy/{Id}\n  method: delete\n  operationId: deleteCachePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-05-31/function\n  method: get\n  operationId: listFunctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /2020-05-31/function\n  method: post\n  operationId: createFunction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-05-31/function/{Name}\n  method: get\n  operationId: describeFunction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-05-31/function/{Name}\n  method: delete\n  operationId: deleteFunction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /2020-05-31/public-key\n\
  \  method: get\n  operationId: listPublicKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /2020-05-31/public-key\n  method: post\n  operationId: createPublicKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudfront/refs/heads/main/agentic-access/cloudfront-agentic-access.yml
summary_line: 23 operations · 11 acting · 2 human-in-the-loop
tags:
- Alias
- CDN
- Caching
- Content Delivery
- Edge Computing
- Lambda@Edge
- Network
---
