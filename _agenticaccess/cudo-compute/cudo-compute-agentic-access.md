---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 27
api_specs:
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Virtual Machines API
  slug: virtual-machines
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Machine Types API
  slug: machine-types
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Data Centers API
  slug: data-centers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Disks & Storage API
  slug: disks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Networks API
  slug: networks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Images API
  slug: images
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute SSH Keys API
  slug: ssh-keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Billing API
  slug: billing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
consequence_counts:
  read: 27
  safety-critical: 4
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Cudo Compute Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/projects/{projectId}/networks/{id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/projects/{projectId}/vms/{id}/reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/projects/{projectId}/vms/{id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/projects/{projectId}/vms/{id}/terminate
operation_count: 49
overview: 'CUDO Compute exposes 49 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 18 write, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CUDO Compute
provider_slug: cudo-compute
slug: cudo-compute-agentic-access
source_filename: cudo-compute-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cudo-compute-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    acting: 22\n    connected: 27\n  by_consequence:\n    write: 18\n    read: 27\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /v1/projects/{projectId}/vm\n  method: post\n  operationId: createVM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/vms\n  method: get\n  operationId: listVMs\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/vms/{id}\n  method: get\n  operationId: getVM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/vms/{id}/start\n  method: post\n  operationId: startVM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/vms/{id}/stop\n  method: post\n  operationId: stopVM\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{projectId}/vms/{id}/reboot\n  method: post\n  operationId: rebootVM\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{projectId}/vms/{id}/resize\n  method: post\n  operationId: resizeVM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/vms/{id}/terminate\n  method: post\n  operationId: terminateVM\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{projectId}/vms/{id}/connect\n  method: get\n  operationId: connectVM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/vms/{id}/monitor\n  method: get\n  operationId: monitorVM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vms/gpu-models\n  method: get\n  operationId: listVMGpuModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vms/machine-types\n\
  \  method: get\n  operationId: listVMMachineTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data-centers/{dataCenterId}/machine-types\n  method: get\n  operationId: listDataCenterMachineTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data-centers/{dataCenterId}/machine-type-prices\n  method: get\n  operationId: listMachineTypePrices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data-centers\n  method: get\n  operationId: listDataCenters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/data-centers/{id}\n  method: get\n  operationId: getDataCenter\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/regions\n  method: get\n  operationId: listRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/disks\n  method: get\n  operationId: listDisks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/disks\n  method: post\n  operationId: createStorageDisk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/disks/{id}\n  method:\
  \ get\n  operationId: getDisk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/disks/{id}\n  method: delete\n  operationId: deleteDisk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/disk/{id}/attach\n  method: patch\n  operationId: attachStorageDisk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/disk/{id}/detach\n  method: put\n  operationId:\
  \ detachStorageDisk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/disks/{id}/snapshots\n  method: get\n  operationId: listDiskSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/disks/{id}/snapshots\n  method: post\n  operationId: createDiskSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/disks/{id}/snapshots\n  method: delete\n\
  \  operationId: deleteDiskSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/networks\n  method: get\n  operationId: listNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/networks\n  method: post\n  operationId: createNetwork\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/networks/{id}\n  method: get\n  operationId: getNetwork\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/networks/{id}\n  method: delete\n  operationId: deleteNetwork\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/networks/{id}/start\n  method: post\n  operationId: startNetwork\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/networks/{id}/stop\n  method: post\n  operationId: stopNetwork\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/projects/{projectId}/networks/security-groups\n  method: get\n  operationId: listSecurityGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/images\n  method: get\n  operationId: listPrivateVMImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/images\n  method: post\n  operationId: createPrivateVMImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/images/{id}\n  method: get\n  operationId: getPrivateVMImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/projects/{projectId}/images/{id}\n  method: delete\n  operationId: deletePrivateVMImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/vms/public-images\n  method: get\n  operationId: listPublicVMImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /v1/ssh-keys\n  method: get\n  operationId: listSSHKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ssh-keys\n  method: post\n  operationId: createSSHKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ssh-keys/{id}\n  method: get\n  operationId: getSSHKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ssh-keys/{id}\n  method: delete\n  operationId: deleteSSHKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/project/{projectId}/ssh-keys\n  method: get\n  operationId: listProjectSSHKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing-accounts\n  method: get\n  operationId: listBillingAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing-accounts\n  method: post\n  operationId: createBillingAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing-accounts/{id}\n  method: get\n  operationId:\
  \ getBillingAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing-accounts/{id}\n  method: delete\n  operationId: deleteBillingAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing-accounts/{id}/details\n  method: get\n  operationId: getBillingAccountDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing-accounts/invoices\n  method: get\n  operationId: listBillingAccountInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/agentic-access/cudo-compute-agentic-access.yml
summary_line: 49 operations · 22 acting · 4 human-in-the-loop
tags:
- GPU
- Cloud Compute
- Infrastructure
- Virtual Machines
- Marketplace
---
