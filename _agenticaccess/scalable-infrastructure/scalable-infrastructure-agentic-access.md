---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 1
api_specs:
- filename: openapi.yaml
  format: yaml
  label: AWS EC2 API
  slug: aws-ec2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/APIs-guru/openapi-directory/main/APIs/amazonaws.com/ec2/2016-11-15/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: AWS VPC API
  slug: aws-vpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/APIs-guru/openapi-directory/main/APIs/amazonaws.com/ec2/2016-11-15/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: AWS EKS API
  slug: aws-eks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/APIs-guru/openapi-directory/main/APIs/amazonaws.com/eks/2018-08-23/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Google Compute Engine API
  slug: google-compute-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/APIs-guru/openapi-directory/main/APIs/googleapis.com/compute/v1/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Google Kubernetes Engine API
  slug: google-kubernetes-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/APIs-guru/openapi-directory/main/APIs/googleapis.com/container/v1/openapi.yaml
- filename: resources.json
  format: json
  label: Azure Resource Manager API
  slug: azure-resource-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/resources/resource-manager/Microsoft.Resources/stable/2023-07-01/resources.json
- filename: managedClusters.json
  format: json
  label: Azure AKS API
  slug: azure-aks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/containerservice/resource-manager/Microsoft.ContainerService/aks/stable/2024-01-01/managedClusters.json
- filename: DigitalOcean-public.v2.yaml
  format: yaml
  label: DigitalOcean API
  slug: digitalocean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/digitalocean/openapi/main/specification/DigitalOcean-public.v2.yaml
consequence_counts:
  read: 1
  safety-critical: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Scalable Infrastructure Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /
operation_count: 2
overview: 'Scalable Infrastructure exposes 2 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Scalable Infrastructure
provider_slug: scalable-infrastructure
slug: scalable-infrastructure-agentic-access
source_filename: scalable-infrastructure-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/scalable-infrastructure-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 1\n    connected: 1\n  by_consequence:\n    safety-critical: 1\n    read: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /\n  method: post\n  operationId: invokeAction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /\n  method: get\n  operationId: invokeActionGet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-infrastructure/refs/heads/main/agentic-access/scalable-infrastructure-agentic-access.yml
summary_line: 2 operations · 1 acting · 1 human-in-the-loop
tags:
- Cloud Infrastructure
- Compute
- DevOps
- Infrastructure as Code
- Kubernetes
- Networking
- Scalability
- Storage
---
