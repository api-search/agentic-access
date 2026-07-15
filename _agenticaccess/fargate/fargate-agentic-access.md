---
acting_count: 16
action_class_counts:
  acting: 16
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon ECS API (Fargate)
  slug: amazon-ecs-api-fargate
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/ecs/2014-11-13/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Amazon EKS API (Fargate)
  slug: amazon-eks-api-fargate
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/eks/2017-11-01/openapi.yaml
consequence_counts:
  safety-critical: 1
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Fargate Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.StopTask
operation_count: 16
overview: 'AWS Fargate exposes 16 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 write and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AWS Fargate
provider_slug: fargate
slug: fargate-agentic-access
source_filename: fargate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fargate-ecs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 16\n  by_consequence:\n    write: 15\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.RegisterTaskDefinition\n  method: post\n  operationId: registerTaskDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.DescribeTaskDefinition\n\
  \  method: post\n  operationId: describeTaskDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.ListTaskDefinitions\n  method: post\n  operationId: listTaskDefinitions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.DeregisterTaskDefinition\n  method: post\n  operationId: deregisterTaskDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.RunTask\n  method: post\n  operationId: runTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.StopTask\n  method: post\n  operationId: stopTask\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.DescribeTasks\n\
  \  method: post\n  operationId: describeTasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.ListTasks\n  method: post\n  operationId: listTasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.CreateService\n  method: post\n  operationId: createService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.UpdateService\n  method: post\n  operationId: updateService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.DeleteService\n  method: post\n  operationId: deleteService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.DescribeServices\n  method: post\n  operationId:\
  \ describeServices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.ListServices\n  method: post\n  operationId: listServices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.CreateCluster\n  method: post\n  operationId: createCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.DescribeClusters\n  method: post\n  operationId: describeClusters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AmazonEC2ContainerServiceV20141113.ExecuteCommand\n  method: post\n  operationId: executeCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fargate/refs/heads/main/agentic-access/fargate-agentic-access.yml
summary_line: 16 operations · 16 acting · 1 human-in-the-loop
tags:
- Compute
- Containers
- Docker
- Kubernetes
- Serverless
---
