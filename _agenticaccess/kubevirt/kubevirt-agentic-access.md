---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 14
api_specs:
- filename: kubevirt-vm-openapi.yml
  format: yaml
  label: KubeVirt VM Management API
  slug: kubevirt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubevirt/refs/heads/main/openapi/kubevirt-vm-openapi.yml
- filename: kubevirt-cdi-openapi.yml
  format: yaml
  label: KubeVirt Containerized Data Importer API
  slug: kubevirt-cdi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubevirt/refs/heads/main/openapi/kubevirt-cdi-openapi.yml
consequence_counts:
  read: 14
  safety-critical: 1
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Kubevirt Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachines/{name}/stop
operation_count: 32
overview: 'KubeVirt exposes 32 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 17 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: KubeVirt
provider_slug: kubevirt
slug: kubevirt-agentic-access
source_filename: kubevirt-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kubevirt-cdi-openapi.yml, openapi/kubevirt-vm-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 14\n    acting: 18\n  by_consequence:\n    read: 14\n    write: 17\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /apis/cdi.kubevirt.io/v1beta1/namespaces/{namespace}/datavolumes\n  method: get\n  operationId: listNamespacedDataVolume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/cdi.kubevirt.io/v1beta1/namespaces/{namespace}/datavolumes\n  method: post\n  operationId: createNamespacedDataVolume\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/cdi.kubevirt.io/v1beta1/namespaces/{namespace}/datavolumes/{name}\n  method: get\n  operationId: readNamespacedDataVolume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/cdi.kubevirt.io/v1beta1/namespaces/{namespace}/datavolumes/{name}\n  method: put\n  operationId: replaceNamespacedDataVolume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/cdi.kubevirt.io/v1beta1/namespaces/{namespace}/datavolumes/{name}\n\
  \  method: delete\n  operationId: deleteNamespacedDataVolume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/cdi.kubevirt.io/v1beta1/namespaces/{namespace}/datasources\n  method: get\n  operationId: listNamespacedDataSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/cdi.kubevirt.io/v1beta1/namespaces/{namespace}/datasources\n  method: post\n  operationId: createNamespacedDataSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /apis/cdi.kubevirt.io/v1beta1/namespaces/{namespace}/datasources/{name}\n  method: get\n  operationId: readNamespacedDataSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/cdi.kubevirt.io/v1beta1/namespaces/{namespace}/datasources/{name}\n  method: delete\n  operationId: deleteNamespacedDataSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/cdi.kubevirt.io/v1beta1/storageprofiles\n  method: get\n  operationId: listStorageProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/cdi.kubevirt.io/v1beta1/storageprofiles/{name}\n\
  \  method: get\n  operationId: readStorageProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/cdi.kubevirt.io/v1beta1/storageprofiles/{name}\n  method: patch\n  operationId: patchStorageProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachines\n  method: get\n  operationId: listNamespacedVirtualMachine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachines\n  method: post\n  operationId: createNamespacedVirtualMachine\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachines/{name}\n  method: get\n  operationId: readNamespacedVirtualMachine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachines/{name}\n  method: put\n  operationId: replaceNamespacedVirtualMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachines/{name}\n\
  \  method: patch\n  operationId: patchNamespacedVirtualMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachines/{name}\n  method: delete\n  operationId: deleteNamespacedVirtualMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachines/{name}/start\n  method: put\n  operationId: startVirtualMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachines/{name}/stop\n  method: put\n  operationId: stopVirtualMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachines/{name}/restart\n  method: put\n  operationId: restartVirtualMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachines/{name}/migrate\n  method: put\n  operationId: migrateVirtualMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachineinstances\n  method: get\n  operationId: listNamespacedVirtualMachineInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachineinstances/{name}\n  method: get\n  operationId: readNamespacedVirtualMachineInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachineinstances/{name}/pause\n  method: put\n  operationId: pauseVirtualMachineInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachineinstances/{name}/unpause\n  method: put\n  operationId: unpauseVirtualMachineInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachineinstances/{name}/vnc\n  method: get\n  operationId: getVirtualMachineInstanceVNC\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachineinstances/{name}/console\n  method: get\n  operationId: getVirtualMachineInstanceConsole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachineinstancemigrations\n  method: get\n  operationId: listNamespacedVMIMigration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachineinstancemigrations\n  method: post\n  operationId: createNamespacedVMIMigration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachineinstancemigrations/{name}\n  method: get\n  operationId: readNamespacedVMIMigration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apis/kubevirt.io/v1/namespaces/{namespace}/virtualmachineinstancemigrations/{name}\n  method: delete\n  operationId: deleteNamespacedVMIMigration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubevirt/refs/heads/main/agentic-access/kubevirt-agentic-access.yml
summary_line: 32 operations · 18 acting · 1 human-in-the-loop
tags:
- Cloud Native
- Incubating
- Kubernetes
- Migration
- Virtual Machines
- Virtualization
---
