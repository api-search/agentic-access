---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 8
api_specs:
- filename: volcano-job-openapi.yml
  format: yaml
  label: Volcano Batch Scheduling API
  slug: volcano-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volcano/refs/heads/main/openapi/volcano-job-openapi.yml
- filename: volcano-queue-openapi.yml
  format: yaml
  label: Volcano Queue API
  slug: volcano-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volcano/refs/heads/main/openapi/volcano-queue-openapi.yml
- filename: volcano-podgroup-openapi.yml
  format: yaml
  label: Volcano PodGroup API
  slug: volcano-podgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volcano/refs/heads/main/openapi/volcano-podgroup-openapi.yml
consequence_counts:
  read: 8
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Volcano Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Volcano exposes 20 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Volcano
provider_slug: volcano
slug: volcano-agentic-access
source_filename: volcano-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/volcano-job-openapi.yml, openapi/volcano-podgroup-openapi.yml, openapi/volcano-queue-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 8\n    acting: 12\n  by_consequence:\n    read: 8\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /apis/batch.volcano.sh/v1alpha1/namespaces/{namespace}/jobs\n  method: get\n  operationId: listNamespacedJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/batch.volcano.sh/v1alpha1/namespaces/{namespace}/jobs\n  method: post\n  operationId: createNamespacedJob\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/batch.volcano.sh/v1alpha1/namespaces/{namespace}/jobs/{name}\n  method: get\n  operationId: readNamespacedJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/batch.volcano.sh/v1alpha1/namespaces/{namespace}/jobs/{name}\n  method: put\n  operationId: replaceNamespacedJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/batch.volcano.sh/v1alpha1/namespaces/{namespace}/jobs/{name}\n\
  \  method: patch\n  operationId: patchNamespacedJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/batch.volcano.sh/v1alpha1/namespaces/{namespace}/jobs/{name}\n  method: delete\n  operationId: deleteNamespacedJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/batch.volcano.sh/v1alpha1/jobs\n  method: get\n  operationId: listJobAllNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/scheduling.volcano.sh/v1beta1/namespaces/{namespace}/podgroups\n\
  \  method: get\n  operationId: listNamespacedPodGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/scheduling.volcano.sh/v1beta1/namespaces/{namespace}/podgroups\n  method: post\n  operationId: createNamespacedPodGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/scheduling.volcano.sh/v1beta1/namespaces/{namespace}/podgroups/{name}\n  method: get\n  operationId: readNamespacedPodGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/scheduling.volcano.sh/v1beta1/namespaces/{namespace}/podgroups/{name}\n  method: put\n \
  \ operationId: replaceNamespacedPodGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/scheduling.volcano.sh/v1beta1/namespaces/{namespace}/podgroups/{name}\n  method: patch\n  operationId: patchNamespacedPodGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/scheduling.volcano.sh/v1beta1/namespaces/{namespace}/podgroups/{name}\n  method: delete\n  operationId: deleteNamespacedPodGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/scheduling.volcano.sh/v1beta1/podgroups\n  method: get\n  operationId: listPodGroupAllNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/scheduling.volcano.sh/v1beta1/queues\n  method: get\n  operationId: listQueues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/scheduling.volcano.sh/v1beta1/queues\n  method: post\n  operationId: createQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /apis/scheduling.volcano.sh/v1beta1/queues/{name}\n  method: get\n  operationId: readQueue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/scheduling.volcano.sh/v1beta1/queues/{name}\n  method: put\n  operationId: replaceQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/scheduling.volcano.sh/v1beta1/queues/{name}\n  method: patch\n  operationId: patchQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /apis/scheduling.volcano.sh/v1beta1/queues/{name}\n  method: delete\n  operationId: deleteQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volcano/refs/heads/main/agentic-access/volcano-agentic-access.yml
summary_line: 20 operations · 12 acting
tags:
- Batch Processing
- Cloud Native
- HPC
- Incubating
- Kubernetes
- Scheduling
- Machine Learning
---
