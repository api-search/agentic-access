---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 10
api_specs:
- filename: spacemesh-v2beta1-openapi-original.json
  format: json
  label: Spacemesh API (v2beta1)
  slug: spacemesh-api-v2beta1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/openapi/spacemesh-v2beta1-openapi-original.json
- filename: spacemesh-v1-openapi-original.json
  format: json
  label: Spacemesh API (v1)
  slug: spacemesh-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/openapi/spacemesh-v1-openapi-original.json
consequence_counts:
  read: 10
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Spacemesh Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'Spacemesh exposes 26 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Spacemesh
provider_slug: spacemesh
slug: spacemesh-agentic-access
source_filename: spacemesh-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/spacemesh-v1-openapi-original.json, openapi/spacemesh-v2beta1-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 16\n    connected: 10\n  by_consequence:\n    write: 16\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /spacemesh.v2alpha1.AccountService/List\n  method: post\n  operationId: AccountService_List\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2alpha1.ActivationService/ActivationsCount\n\
  \  method: post\n  operationId: ActivationService_ActivationsCount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2alpha1.ActivationService/Highest\n  method: post\n  operationId: ActivationService_Highest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2alpha1.ActivationService/List\n  method: post\n  operationId: ActivationService_List\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2alpha1.LayerService/List\n  method: post\n  operationId: LayerService_List\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2alpha1.MalfeasanceService/List\n  method: post\n  operationId: MalfeasanceService_List\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2alpha1.NetworkService/Info\n  method: post\n  operationId: NetworkService_Info\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2alpha1.NodeService/Status\n  method: post\n  operationId: NodeService_Status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2alpha1.RewardService/List\n  method: post\n  operationId: RewardService_List\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /spacemesh.v2alpha1.TransactionService/EstimateGas\n  method: post\n  operationId: TransactionService_EstimateGas\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2alpha1.TransactionService/List\n  method: post\n  operationId: TransactionService_List\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2alpha1.TransactionService/ParseTransaction\n  method: post\n  operationId: TransactionService_ParseTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2alpha1.TransactionService/SubmitTransaction\n  method: post\n  operationId: TransactionService_SubmitTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2beta1.AccountService/List\n  method: get\n  operationId: AccountService_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spacemesh.v2beta1.ActivationService/ActivationsCount\n  method: get\n  operationId: ActivationService_ActivationsCount\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spacemesh.v2beta1.ActivationService/Highest\n  method: get\n  operationId: ActivationService_Highest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spacemesh.v2beta1.ActivationService/List\n  method: get\n  operationId: ActivationService_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spacemesh.v2beta1.LayerService/List\n  method: get\n  operationId: LayerService_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spacemesh.v2beta1.MalfeasanceService/List\n  method: get\n  operationId: MalfeasanceService_List\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spacemesh.v2beta1.NetworkService/Info\n  method: get\n  operationId: NetworkService_Info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spacemesh.v2beta1.NodeService/Status\n  method: get\n  operationId: NodeService_Status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spacemesh.v2beta1.RewardService/List\n  method: get\n  operationId: RewardService_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spacemesh.v2beta1.TransactionService/EstimateGas\n  method: post\n  operationId: TransactionService_EstimateGas\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2beta1.TransactionService/List\n  method: get\n  operationId: TransactionService_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spacemesh.v2beta1.TransactionService/ParseTransaction\n  method: post\n  operationId: TransactionService_ParseTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spacemesh.v2beta1.TransactionService/SubmitTransaction\n  method: post\n\
  \  operationId: TransactionService_SubmitTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/agentic-access/spacemesh-agentic-access.yml
summary_line: 26 operations · 16 acting
tags:
- Company
- Crypto Infrastructure
- Blockchain
- Cryptocurrency
- Proof of Space-Time
- Layer 1
- gRPC
- Node API
- Open Source
---
