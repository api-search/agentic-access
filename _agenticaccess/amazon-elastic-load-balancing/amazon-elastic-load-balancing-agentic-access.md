---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: amazon-elastic-load-balancing-openapi.yml
  format: yaml
  label: Elastic Load Balancing v2 API
  slug: elastic-load-balancing-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/openapi/amazon-elastic-load-balancing-openapi.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Elastic Load Balancing Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Amazon Elastic Load Balancing exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
slug: amazon-elastic-load-balancing-agentic-access
source_filename: amazon-elastic-load-balancing-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-elastic-load-balancing-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /?Action=CreateLoadBalancer\n  method: get\n  operationId: createLoadBalancer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeLoadBalancers\n  method: get\n  operationId: describeLoadBalancers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /?Action=DeleteLoadBalancer\n  method: get\n  operationId: deleteLoadBalancer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=ModifyLoadBalancerAttributes\n  method: get\n  operationId: modifyLoadBalancerAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=CreateTargetGroup\n  method: get\n  operationId: createTargetGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeTargetGroups\n  method: get\n  operationId: describeTargetGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=RegisterTargets\n  method: get\n  operationId:\
  \ registerTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DeregisterTargets\n  method: get\n  operationId: deregisterTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeTargetHealth\n  method: get\n  operationId: describeTargetHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=CreateListener\n  method: get\n  operationId: createListener\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeListeners\n  method: get\n  operationId: describeListeners\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=CreateRule\n  method: get\n  operationId: createRule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeRules\n  method: get\n  operationId: describeRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/agentic-access/amazon-elastic-load-balancing-agentic-access.yml
summary_line: 13 operations
tags:
- Amazon Web Services
- High Availability
- Load Balancing
- Networking
- Scalability
---
