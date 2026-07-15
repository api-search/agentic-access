---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 9
api_specs:
- filename: conduktor-openapi.yml
  format: yaml
  label: Conduktor Console - Clusters, Topics & Consumer Groups API
  slug: console-clusters-topics-consumer-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/openapi/conduktor-openapi.yml
- filename: conduktor-openapi.yml
  format: yaml
  label: Conduktor Console - RBAC & Users API
  slug: console-rbac-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/openapi/conduktor-openapi.yml
- filename: conduktor-openapi.yml
  format: yaml
  label: Conduktor Console - Self-Service API
  slug: console-self-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/openapi/conduktor-openapi.yml
- filename: conduktor-openapi.yml
  format: yaml
  label: Conduktor Gateway - Interceptors API
  slug: gateway-interceptors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/openapi/conduktor-openapi.yml
- filename: conduktor-openapi.yml
  format: yaml
  label: Conduktor Gateway - Virtual Clusters API
  slug: gateway-virtual-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/openapi/conduktor-openapi.yml
consequence_counts:
  physical: 1
  read: 9
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Conduktor Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /public/iam/v2/user/{userEmail}
operation_count: 22
overview: 'Conduktor exposes 22 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Conduktor
provider_slug: conduktor
slug: conduktor-agentic-access
source_filename: conduktor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/conduktor-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 9\n    acting: 13\n  by_consequence:\n    read: 9\n    write: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /public/v1/configs/{cluster}/clusters\n  method: get\n  operationId: listClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/clusters\n  method: get\n  operationId: getClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /public/v1/clusters\n  method: post\n  operationId: upsertCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/clusters/{cluster}\n  method: delete\n  operationId: deleteCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v1/certificates\n  method: get\n  operationId: listCertificates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/certificates\n  method: post\n  operationId:\
  \ upsertCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/iam/v2/user\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/iam/v2/user/{userEmail}\n  method: put\n  operationId: upsertUser\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/iam/v2/user/{userEmail}\n  method: delete\n  operationId:\
  \ deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/iam/v2/group\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/iam/v2/group/{groupName}\n  method: get\n  operationId: getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/iam/v2/group/{groupName}\n  method: put\n  operationId: upsertGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/iam/v2/group/{groupName}\n  method: delete\n  operationId: deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/self-serve/v1/application\n  method: get\n  operationId: listApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/self-serve/v1/application\n  method: put\n  operationId: upsertApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /public/self-serve/v1/topic-policy\n  method: put\n  operationId: upsertTopicPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/v2/interceptor\n  method: get\n  operationId: listInterceptors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/v2/interceptor\n  method: put\n  operationId: upsertInterceptor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /gateway/v2/virtual-cluster\n  method: put\n  operationId: upsertVirtualCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/v2/virtual-cluster/{name}\n  method: get\n  operationId: getVirtualCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/v2/service-account\n  method: put\n  operationId: upsertServiceAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/v2/token\n\
  \  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conduktor/refs/heads/main/agentic-access/conduktor-agentic-access.yml
summary_line: 22 operations · 13 acting
tags:
- Apache Kafka
- Streaming
- Data Governance
- Kafka Management
- Gateway
---
