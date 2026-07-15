---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 4
api_specs:
- filename: amazon-privatelink-openapi.yaml
  format: yaml
  label: AWS PrivateLink API
  slug: aws-privatelink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/openapi/amazon-privatelink-openapi.yaml
consequence_counts:
  read: 4
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Privatelink Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Amazon PrivateLink exposes 13 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
slug: amazon-privatelink-agentic-access
source_filename: amazon-privatelink-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-privatelink-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 9\n    connected: 4\n  by_consequence:\n    write: 9\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /?Action=CreateVpcEndpointServiceConfiguration\n  method: post\n  operationId: CreateVpcEndpointServiceConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /?Action=DescribeVpcEndpointServices\n  method: get\n\
  \  operationId: DescribeVpcEndpointServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=ModifyVpcEndpointServiceConfiguration\n  method: post\n  operationId: ModifyVpcEndpointServiceConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /?Action=DeleteVpcEndpointServiceConfigurations\n  method: post\n  operationId: DeleteVpcEndpointServiceConfigurations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /?Action=CreateVpcEndpoint\n  method: post\n  operationId: CreateVpcEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /?Action=DescribeVpcEndpoints\n  method: get\n  operationId: DescribeVpcEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=ModifyVpcEndpoint\n  method: post\n  operationId: ModifyVpcEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /?Action=DeleteVpcEndpoints\n\
  \  method: post\n  operationId: DeleteVpcEndpoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /?Action=DescribeVpcEndpointConnections\n  method: get\n  operationId: DescribeVpcEndpointConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=AcceptVpcEndpointConnections\n  method: post\n  operationId: AcceptVpcEndpointConnections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /?Action=RejectVpcEndpointConnections\n\
  \  method: post\n  operationId: RejectVpcEndpointConnections\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /?Action=ModifyVpcEndpointServicePermissions\n  method: post\n  operationId: ModifyVpcEndpointServicePermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /?Action=DescribeVpcEndpointServicePermissions\n  method: get\n  operationId: DescribeVpcEndpointServicePermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/agentic-access/amazon-privatelink-agentic-access.yml
summary_line: 13 operations · 9 acting
tags:
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
---
