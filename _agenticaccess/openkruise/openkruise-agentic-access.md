---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: openkruise-openapi.yml
  format: yaml
  label: OpenKruise Workload API
  slug: openkruise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openkruise/refs/heads/main/openapi/openkruise-openapi.yml
consequence_counts:
  read: 9
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openkruise Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'OpenKruise exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenKruise
provider_slug: openkruise
slug: openkruise-agentic-access
source_filename: openkruise-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openkruise-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 9\n    acting: 8\n  by_consequence:\n    read: 9\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /apis/apps.kruise.io/v1alpha1/clonesets\n  method: get\n  operationId: listClonesetsAllNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apps.kruise.io/v1alpha1/namespaces/{namespace}/clonesets\n  method: get\n  operationId: listClonesets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /apis/apps.kruise.io/v1alpha1/namespaces/{namespace}/clonesets\n  method: post\n  operationId: createCloneset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.kruise.io/v1alpha1/namespaces/{namespace}/clonesets/{name}\n  method: get\n  operationId: getCloneset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apps.kruise.io/v1alpha1/namespaces/{namespace}/clonesets/{name}\n  method: delete\n  operationId: deleteCloneset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.kruise.io/v1beta1/namespaces/{namespace}/statefulsets\n  method: get\n  operationId: listAdvancedStatefulSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apps.kruise.io/v1beta1/namespaces/{namespace}/statefulsets\n  method: post\n  operationId: createAdvancedStatefulSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.kruise.io/v1beta1/namespaces/{namespace}/statefulsets/{name}\n  method: get\n  operationId: getAdvancedStatefulSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apps.kruise.io/v1beta1/namespaces/{namespace}/statefulsets/{name}\n  method: delete\n  operationId: deleteAdvancedStatefulSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.kruise.io/v1alpha1/namespaces/{namespace}/daemonsets\n  method: get\n  operationId: listAdvancedDaemonSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apps.kruise.io/v1alpha1/namespaces/{namespace}/daemonsets\n  method: post\n  operationId: createAdvancedDaemonSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.kruise.io/v1alpha1/sidecarsets\n  method: get\n  operationId: listSidecarSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apps.kruise.io/v1alpha1/sidecarsets\n  method: post\n  operationId: createSidecarSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.kruise.io/v1alpha1/namespaces/{namespace}/broadcastjobs\n  method: get\n  operationId: listBroadcastJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apps.kruise.io/v1alpha1/namespaces/{namespace}/broadcastjobs\n  method: post\n  operationId: createBroadcastJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/apps.kruise.io/v1alpha1/imagepulljobs\n  method: get\n  operationId: listImagePullJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/apps.kruise.io/v1alpha1/imagepulljobs\n  method: post\n  operationId: createImagePullJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openkruise/refs/heads/main/agentic-access/openkruise-agentic-access.yml
summary_line: 17 operations · 8 acting
tags:
- Cloud Native
- Controllers
- Deployment
- Incubating
- Kubernetes
- Workload Management
- CRDs
---
