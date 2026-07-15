---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: service-fabric-cluster-openapi.yml
  format: yaml
  label: Service Fabric Cluster Management API
  slug: service-fabric-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-fabric/refs/heads/main/openapi/service-fabric-cluster-openapi.yml
consequence_counts:
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Service Fabric Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Service Fabric exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Service Fabric
provider_slug: service-fabric
slug: service-fabric-agentic-access
source_filename: service-fabric-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/service-fabric-cluster-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 7\n    acting: 2\n  by_consequence:\n    read: 7\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /$/GetClusterHealth\n  method: get\n  operationId: getClusterHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Nodes\n  method: get\n  operationId: getNodeInfoList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Nodes/{nodeName}\n\
  \  method: get\n  operationId: getNodeInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Applications\n  method: get\n  operationId: getApplicationInfoList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Applications/{applicationId}\n  method: get\n  operationId: getApplicationInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Applications/$/Create\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /Applications/{applicationId}/$/Delete\n  method: post\n  operationId: deleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Applications/{applicationId}/$/GetHealth\n  method: get\n  operationId: getApplicationHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Applications/{applicationId}/$/GetServices\n  method: get\n  operationId: getServiceInfoList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/service-fabric/refs/heads/main/agentic-access/service-fabric-agentic-access.yml
summary_line: 9 operations · 2 acting
tags:
- Distributed Systems
- Microservices
- Containers
- Cloud Native
- Kubernetes
- Azure
- Open Source
---
