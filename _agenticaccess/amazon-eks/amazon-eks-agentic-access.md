---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: amazon-eks-clusters-api-openapi.yml
  format: yaml
  label: Amazon EKS Clusters API
  slug: amazon-eks-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-clusters-api-openapi.yml
- filename: amazon-eks-fargate-profiles-api-openapi.yml
  format: yaml
  label: Amazon EKS Fargate Profiles API
  slug: amazon-eks-fargate-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-fargate-profiles-api-openapi.yml
- filename: amazon-eks-node-groups-api-openapi.yml
  format: yaml
  label: Amazon EKS Node Groups API
  slug: amazon-eks-node-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-node-groups-api-openapi.yml
- filename: amazon-eks-add-ons-api-openapi.yml
  format: yaml
  label: Amazon EKS Add Ons API
  slug: amazon-eks-add-ons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-add-ons-api-openapi.yml
- filename: amazon-eks-access-entries-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Access Entries API
  slug: amazon-eks-access-entries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-access-entries-api-openapi.yml
- filename: amazon-eks-access-policies-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Access Policies API
  slug: amazon-eks-access-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-access-policies-api-openapi.yml
- filename: amazon-eks-capabilities-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Capabilities API
  slug: amazon-eks-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-capabilities-api-openapi.yml
- filename: amazon-eks-certificate-authorities-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Certificate Authorities API
  slug: amazon-eks-certificate-authorities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-certificate-authorities-api-openapi.yml
- filename: amazon-eks-eks-anywhere-subscriptions-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Eks Anywhere Subscriptions API
  slug: amazon-eks-eks-anywhere-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-eks-anywhere-subscriptions-api-openapi.yml
- filename: amazon-eks-identity-provider-configs-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Identity Provider Configs API
  slug: amazon-eks-identity-provider-configs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-identity-provider-configs-api-openapi.yml
- filename: amazon-eks-operations-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Operations API
  slug: amazon-eks-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-operations-api-openapi.yml
- filename: amazon-eks-pod-identity-associations-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Pod Identity Associations API
  slug: amazon-eks-pod-identity-associations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-pod-identity-associations-api-openapi.yml
- filename: amazon-eks-tags-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Tags API
  slug: amazon-eks-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-tags-api-openapi.yml
- filename: amazon-eks-updates-api-openapi.yml
  format: yaml
  label: Amazon EKS Eks Updates API
  slug: amazon-eks-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-eks/openapi/amazon-eks-updates-api-openapi.yml
consequence_counts:
  read: 8
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Eks Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Amazon EKS exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon EKS
provider_slug: amazon-eks
slug: amazon-eks-agentic-access
source_filename: amazon-eks-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-eks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 8\n    connected: 8\n  by_consequence:\n    write: 8\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /clusters\n  method: post\n  operationId: CreateCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters\n  method: get\n  operationId: ListClusters\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{name}\n  method: get\n  operationId: DescribeCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{name}\n  method: delete\n  operationId: DeleteCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters/{name}/node-groups\n  method: post\n  operationId: CreateNodegroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /clusters/{name}/node-groups\n  method: get\n  operationId: ListNodegroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{name}/node-groups/{nodegroupName}\n  method: get\n  operationId: DescribeNodegroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{name}/node-groups/{nodegroupName}\n  method: delete\n  operationId: DeleteNodegroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters/{name}/fargate-profiles\n  method: post\n  operationId: CreateFargateProfile\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters/{name}/fargate-profiles\n  method: get\n  operationId: ListFargateProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{name}/fargate-profiles/{fargateProfileName}\n  method: get\n  operationId: DescribeFargateProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{name}/fargate-profiles/{fargateProfileName}\n  method: delete\n  operationId: DeleteFargateProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters/{name}/addons\n  method: post\n  operationId: CreateAddon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters/{name}/addons\n  method: get\n  operationId: ListAddons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{name}/addons/{addonName}\n  method: get\n  operationId: DescribeAddon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{name}/addons/{addonName}\n  method:\
  \ delete\n  operationId: DeleteAddon\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/amazon-eks/agentic-access/amazon-eks-agentic-access.yml
summary_line: 16 operations · 8 acting
tags:
- Amazon Web Services
- Container Orchestration
- Containers
- EKS
- Kubernetes
---
