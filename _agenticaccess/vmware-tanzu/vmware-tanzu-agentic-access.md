---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: vmware-tanzu-service-mesh-openapi.yml
  format: yaml
  label: VMware Tanzu Service Mesh API
  slug: tanzu-service-mesh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware-tanzu/refs/heads/main/openapi/vmware-tanzu-service-mesh-openapi.yml
- filename: vmware-tanzu-kubernetes-grid-openapi.yml
  format: yaml
  label: VMware Tanzu Kubernetes Grid API
  slug: tanzu-kubernetes-grid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware-tanzu/refs/heads/main/openapi/vmware-tanzu-kubernetes-grid-openapi.yml
consequence_counts:
  read: 5
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vmware Tanzu Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'VMware Tanzu exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: VMware Tanzu
provider_slug: vmware-tanzu
slug: vmware-tanzu-agentic-access
source_filename: vmware-tanzu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vmware-tanzu-service-mesh-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 7\n    connected: 5\n  by_consequence:\n    write: 7\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /csp/gateway/am/api/auth/api-tokens/authorize\n  method: post\n  operationId: exchangeApiToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha1/clusters\n  method: get\n  operationId: listClusters\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha1/clusters/{cluster_name}\n  method: get\n  operationId: getCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha1/clusters/{cluster_name}\n  method: put\n  operationId: onboardCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha1/clusters/{cluster_name}\n  method: delete\n  operationId: removeCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha1/global-namespaces\n  method: get\n  operationId: listGlobalNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha1/global-namespaces\n  method: post\n  operationId: createGlobalNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha1/global-namespaces/{namespace_id}\n  method: get\n  operationId: getGlobalNamespace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha1/global-namespaces/{namespace_id}\n  method:\
  \ put\n  operationId: updateGlobalNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha1/global-namespaces/{namespace_id}\n  method: delete\n  operationId: deleteGlobalNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1alpha1/resource-groups\n  method: get\n  operationId: listResourceGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1alpha1/resource-groups\n  method: post\n  operationId:\
  \ createResourceGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vmware-tanzu/refs/heads/main/agentic-access/vmware-tanzu-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- Cloud Native
- Containers
- Enterprise
- Kubernetes
- Multi-Cloud
- Service Mesh
- VMware
---
