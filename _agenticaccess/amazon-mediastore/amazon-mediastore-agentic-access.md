---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 6
api_specs:
- filename: amazon-mediastore-aws-elemental-mediastore-api-openapi.yml
  format: yaml
  label: Amazon MediaStore AWS Elemental MediaStore API
  slug: amazon-mediastore-aws-elemental-mediastore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/openapi/amazon-mediastore-aws-elemental-mediastore-api-openapi.yml
consequence_counts:
  read: 6
  safety-critical: 1
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Mediastore Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=MediaStore_20170901.StopAccessLogging
operation_count: 21
overview: 'Amazon MediaStore exposes 21 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 14 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
slug: amazon-mediastore-agentic-access
source_filename: amazon-mediastore-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/amazon-mediastore-x-amz-target-mediastore-20170901-createcontainer-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-deletecontainer-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-deletecontainerpolicy-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-deletecorspolicy-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-deletelifecyclepolicy-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-deletemetricpolicy-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-describecontainer-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-getcontainerpolicy-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-getcorspolicy-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-getlifecyclepolicy-api-openapi.yml,\n\
  \  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-getmetricpolicy-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-listcontainers-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-listtagsforresource-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-putcontainerpolicy-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-putcorspolicy-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-putlifecyclepolicy-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-putmetricpolicy-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-startaccesslogging-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-stopaccesslogging-api-openapi.yml,\n  openapi/amazon-mediastore-x-amz-target-mediastore-20170901-tagresource-api-openapi.yml, openapi/amazon-mediastore-x-amz-target-mediastore-20170901-untagresource-api-openapi.yml\n\
  description: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 15\n    connected: 6\n  by_consequence:\n    write: 14\n    read: 6\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /#X-Amz-Target=MediaStore_20170901.CreateContainer\n  method: post\n  operationId: CreateContainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=MediaStore_20170901.DeleteContainer\n  method: post\n  operationId: DeleteContainer\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=MediaStore_20170901.DeleteContainerPolicy\n  method: post\n  operationId: DeleteContainerPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=MediaStore_20170901.DeleteCorsPolicy\n  method: post\n  operationId: DeleteCorsPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /#X-Amz-Target=MediaStore_20170901.DeleteLifecyclePolicy\n  method: post\n  operationId: DeleteLifecyclePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=MediaStore_20170901.DeleteMetricPolicy\n  method: post\n  operationId: DeleteMetricPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=MediaStore_20170901.DescribeContainer\n  method: post\n  operationId: DescribeContainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=MediaStore_20170901.GetContainerPolicy\n  method: post\n  operationId: GetContainerPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=MediaStore_20170901.GetCorsPolicy\n  method: post\n  operationId: GetCorsPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=MediaStore_20170901.GetLifecyclePolicy\n  method: post\n  operationId: GetLifecyclePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=MediaStore_20170901.GetMetricPolicy\n\
  \  method: post\n  operationId: GetMetricPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=MediaStore_20170901.ListContainers\n  method: post\n  operationId: ListContainers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=MediaStore_20170901.ListTagsForResource\n  method: post\n  operationId: ListTagsForResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#X-Amz-Target=MediaStore_20170901.PutContainerPolicy\n  method: post\n  operationId: PutContainerPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=MediaStore_20170901.PutCorsPolicy\n  method: post\n  operationId: PutCorsPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=MediaStore_20170901.PutLifecyclePolicy\n  method: post\n  operationId: PutLifecyclePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=MediaStore_20170901.PutMetricPolicy\n  method: post\n  operationId: PutMetricPolicy\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=MediaStore_20170901.StartAccessLogging\n  method: post\n  operationId: StartAccessLogging\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=MediaStore_20170901.StopAccessLogging\n  method: post\n  operationId: StopAccessLogging\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=MediaStore_20170901.TagResource\n  method: post\n  operationId: TagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=MediaStore_20170901.UntagResource\n  method: post\n  operationId: UntagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/agentic-access/amazon-mediastore-agentic-access.yml
summary_line: 21 operations · 15 acting · 1 human-in-the-loop
tags:
- Broadcasting
- Media Processing
- Media
- Defunct
---
