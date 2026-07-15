---
acting_count: 0
action_class_counts:
  connected: 26
api_specs:
- filename: amazon-ec2-openapi.yml
  format: yaml
  label: Amazon EC2 API
  slug: amazon-ec2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/openapi/amazon-ec2-openapi.yml
consequence_counts:
  read: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Ec2 Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Amazon EC2 exposes 26 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon EC2
provider_slug: amazon-ec2
slug: amazon-ec2-agentic-access
source_filename: amazon-ec2-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-ec2-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 26\n  by_consequence:\n    read: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /?Action=RunInstances\n  method: get\n  operationId: runInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeInstances\n  method: get\n  operationId: describeInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=StartInstances\n  method: get\n\
  \  operationId: startInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=StopInstances\n  method: get\n  operationId: stopInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=TerminateInstances\n  method: get\n  operationId: terminateInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=RebootInstances\n  method: get\n  operationId: rebootInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeInstanceStatus\n  method: get\n  operationId: describeInstanceStatus\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=CreateImage\n  method: get\n  operationId: createImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeImages\n  method: get\n  operationId: describeImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DeregisterImage\n  method: get\n  operationId: deregisterImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=CreateSecurityGroup\n  method: get\n  operationId: createSecurityGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /?Action=DescribeSecurityGroups\n  method: get\n  operationId: describeSecurityGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=AuthorizeSecurityGroupIngress\n  method: get\n  operationId: authorizeSecurityGroupIngress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DeleteSecurityGroup\n  method: get\n  operationId: deleteSecurityGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=CreateKeyPair\n  method: get\n  operationId: createKeyPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeKeyPairs\n  method: get\n\
  \  operationId: describeKeyPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DeleteKeyPair\n  method: get\n  operationId: deleteKeyPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=AllocateAddress\n  method: get\n  operationId: allocateAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=AssociateAddress\n  method: get\n  operationId: associateAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=ReleaseAddress\n  method: get\n  operationId: releaseAddress\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=CreateLaunchTemplate\n  method: get\n  operationId: createLaunchTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeLaunchTemplates\n  method: get\n  operationId: describeLaunchTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=RequestSpotInstances\n  method: get\n  operationId: requestSpotInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeSpotInstanceRequests\n  method: get\n  operationId: describeSpotInstanceRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeRegions\n  method: get\n  operationId: describeRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeAvailabilityZones\n  method: get\n  operationId: describeAvailabilityZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/agentic-access/amazon-ec2-agentic-access.yml
summary_line: 26 operations
tags:
- Cloud Computing
- Compute
- IaaS
- Infrastructure
- Virtual Machines
---
