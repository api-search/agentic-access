---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 27
api_specs:
- filename: vmware-clusters-api-openapi.yml
  format: yaml
  label: VMware Clusters API
  slug: vmware-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-clusters-api-openapi.yml
- filename: vmware-content-library-api-openapi.yml
  format: yaml
  label: VMware Content Library API
  slug: vmware-content-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-content-library-api-openapi.yml
- filename: vmware-datacenters-api-openapi.yml
  format: yaml
  label: VMware Datacenters API
  slug: vmware-datacenters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-datacenters-api-openapi.yml
- filename: vmware-datastores-api-openapi.yml
  format: yaml
  label: VMware Datastores API
  slug: vmware-datastores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-datastores-api-openapi.yml
- filename: vmware-folders-api-openapi.yml
  format: yaml
  label: VMware Folders API
  slug: vmware-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-folders-api-openapi.yml
- filename: vmware-hosts-api-openapi.yml
  format: yaml
  label: VMware Hosts API
  slug: vmware-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-hosts-api-openapi.yml
- filename: vmware-networks-api-openapi.yml
  format: yaml
  label: VMware Networks API
  slug: vmware-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-networks-api-openapi.yml
- filename: vmware-resource-pools-api-openapi.yml
  format: yaml
  label: VMware Resource Pools API
  slug: vmware-resource-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-resource-pools-api-openapi.yml
- filename: vmware-session-api-openapi.yml
  format: yaml
  label: VMware Session API
  slug: vmware-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-session-api-openapi.yml
- filename: vmware-storage-policies-api-openapi.yml
  format: yaml
  label: VMware Storage Policies API
  slug: vmware-storage-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-storage-policies-api-openapi.yml
- filename: vmware-tagging-api-openapi.yml
  format: yaml
  label: VMware Tagging API
  slug: vmware-tagging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-tagging-api-openapi.yml
- filename: vmware-vm-guest-api-openapi.yml
  format: yaml
  label: VMware VM Guest API
  slug: vmware-vm-guest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vm-guest-api-openapi.yml
- filename: vmware-vm-hardware-api-openapi.yml
  format: yaml
  label: VMware VM Hardware API
  slug: vmware-vm-hardware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vm-hardware-api-openapi.yml
- filename: vmware-vm-power-api-openapi.yml
  format: yaml
  label: VMware VM Power API
  slug: vmware-vm-power-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vm-power-api-openapi.yml
- filename: vmware-vms-api-openapi.yml
  format: yaml
  label: VMware VMs API
  slug: vmware-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vms-api-openapi.yml
consequence_counts:
  read: 27
  safety-critical: 3
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Vmware Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /session
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /vcenter/vm/{vm}/power?action=reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /vcenter/vm/{vm}/power?action=stop
operation_count: 49
overview: 'VMware exposes 49 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 19 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: VMware
provider_slug: vmware
slug: vmware-agentic-access
source_filename: vmware-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vmware-vsphere-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    acting: 22\n    connected: 27\n  by_consequence:\n    write: 19\n    safety-critical: 3\n    read: 27\n  human_in_the_loop_required: 3\noperations:\n- path: /session\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session\n  method: delete\n  operationId: deleteSession\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /session\n  method: get\n  operationId: getSessionInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/vm\n  method: get\n  operationId: listVMs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/vm\n  method: post\n  operationId: createVM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /vcenter/vm/{vm}\n  method: get\n  operationId: getVM\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/vm/{vm}\n  method: delete\n  operationId: deleteVM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcenter/vm/{vm}/power\n  method: get\n  operationId: getVMPowerState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/vm/{vm}/power?action=start\n  method: post\n  operationId: powerOnVM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcenter/vm/{vm}/power?action=stop\n  method: post\n  operationId: powerOffVM\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /vcenter/vm/{vm}/power?action=suspend\n  method: post\n  operationId: suspendVM\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcenter/vm/{vm}/power?action=reset\n  method: post\n  operationId:\
  \ resetVM\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /vcenter/vm/{vm}/hardware\n  method: get\n  operationId: getVMHardware\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/vm/{vm}/hardware\n  method: patch\n  operationId: updateVMHardware\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcenter/vm/{vm}/hardware/cpu\n  method: get\n  operationId: getVMCpu\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/vm/{vm}/hardware/cpu\n  method: patch\n  operationId: updateVMCpu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcenter/vm/{vm}/hardware/memory\n  method: get\n  operationId: getVMMemory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/vm/{vm}/hardware/memory\n  method: patch\n  operationId: updateVMMemory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcenter/vm/{vm}/hardware/disk\n  method: get\n  operationId: listVMDisks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/vm/{vm}/hardware/disk\n  method: post\n  operationId: createVMDisk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcenter/vm/{vm}/hardware/ethernet\n  method: get\n  operationId: listVMEthernet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/vm/{vm}/hardware/ethernet\n  method: post\n  operationId: createVMEthernet\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcenter/vm/{vm}/guest/identity\n  method: get\n  operationId: getVMGuestIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/vm/{vm}/guest/networking\n  method: get\n  operationId: getVMGuestNetworking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/host\n  method: get\n  operationId: listHosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/host/{host}\n  method: get\n  operationId:\
  \ getHost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/host/{host}/connect\n  method: post\n  operationId: connectHost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcenter/host/{host}/disconnect\n  method: post\n  operationId: disconnectHost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcenter/datastore\n  method: get\n  operationId: listDatastores\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/datastore/{datastore}\n  method: get\n  operationId: getDatastore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/cluster\n  method: get\n  operationId: listClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/cluster/{cluster}\n  method: get\n  operationId: getCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/network\n  method: get\n  operationId: listNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/datacenter\n\
  \  method: get\n  operationId: listDatacenters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/datacenter\n  method: post\n  operationId: createDatacenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcenter/datacenter/{datacenter}\n  method: get\n  operationId: getDatacenter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/datacenter/{datacenter}\n  method: delete\n  operationId: deleteDatacenter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcenter/folder\n  method: get\n  operationId: listFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vcenter/resource-pool\n  method: get\n  operationId: listResourcePools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content/library\n  method: get\n  operationId: listContentLibraries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content/library\n  method: post\n  operationId: createContentLibrary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /content/library/{library_id}\n  method: get\n  operationId: getContentLibrary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content/library/{library_id}\n  method: delete\n  operationId: deleteContentLibrary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vcenter/storage/policies\n  method: get\n  operationId: listStoragePolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /cis/tagging/category\n  method: get\n  operationId: listTagCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cis/tagging/category\n  method: post\n  operationId: createTagCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cis/tagging/tag\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cis/tagging/tag\n  method: post\n  operationId: createTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cis/tagging/tag-association?action=attach\n  method: post\n  operationId: attachTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/agentic-access/vmware-agentic-access.yml
summary_line: 49 operations · 22 acting · 3 human-in-the-loop
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
---
