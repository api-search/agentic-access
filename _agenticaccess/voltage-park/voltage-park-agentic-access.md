---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 25
api_specs:
- filename: voltage-park-openapi.yml
  format: yaml
  label: Voltage Park Virtual Machines API
  slug: voltage-park-virtual-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-openapi.yml
- filename: voltage-park-openapi.yml
  format: yaml
  label: Voltage Park Bare Metal & Clusters API
  slug: voltage-park-bare-metal-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-openapi.yml
- filename: voltage-park-openapi.yml
  format: yaml
  label: Voltage Park SSH Keys API
  slug: voltage-park-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-openapi.yml
- filename: voltage-park-openapi.yml
  format: yaml
  label: Voltage Park Storage API
  slug: voltage-park-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-openapi.yml
- filename: voltage-park-openapi.yml
  format: yaml
  label: Voltage Park Locations & HostNodes API
  slug: voltage-park-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-openapi.yml
- filename: voltage-park-openapi.yml
  format: yaml
  label: Voltage Park Billing API
  slug: voltage-park-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-openapi.yml
- filename: voltage-park-openapi.yml
  format: yaml
  label: Voltage Park Organization API
  slug: voltage-park-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/openapi/voltage-park-openapi.yml
consequence_counts:
  physical: 2
  read: 25
  safety-critical: 7
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 7
kind: agentic-access
layout: agentic-access
method: generated
name: Voltage Park Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /bare-metal/{baremetal_rental_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /bare-metal/{baremetal_rental_id}/power-status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /bare-metal/{baremetal_rental_id}/reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /storage/{storage_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /virtual-machines/{virtual_machine_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /virtual-machines/{virtual_machine_id}/power-status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /virtual-machines/{virtual_machine_id}/relocate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bare-metal/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /virtual-machines/instant
operation_count: 48
overview: 'Voltage Park exposes 48 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 14 write, 2 physical, and 7 safety-critical.


  7 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Voltage Park
provider_slug: voltage-park
slug: voltage-park-agentic-access
source_filename: voltage-park-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/voltage-park-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 48\n  by_action_class:\n    connected: 25\n    acting: 23\n  by_consequence:\n    read: 25\n    physical: 2\n    write: 14\n    safety-critical: 7\n  human_in_the_loop_required: 7\noperations:\n- path: /virtual-machines/instant/locations\n  method: get\n  operationId: getInstantVmLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /virtual-machines/instant/locations/{location_id}\n  method: get\n  operationId: getInstantVmLocationDetails\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /virtual-machines/instant\n  method: post\n  operationId: deployInstantVm\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virtual-machines/\n  method: get\n  operationId: listVirtualMachines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /virtual-machines/{virtual_machine_id}\n  method: get\n  operationId: getVirtualMachine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /virtual-machines/{virtual_machine_id}\n\
  \  method: patch\n  operationId: modifyVirtualMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virtual-machines/{virtual_machine_id}\n  method: delete\n  operationId: terminateVirtualMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /virtual-machines/{virtual_machine_id}/power-status\n  method: put\n  operationId: setVirtualMachinePowerStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /virtual-machines/{virtual_machine_id}/relocate\n  method: post\n  operationId: relocateVirtualMachine\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /virtual-machines/{virtual_machine_id}/port-forward\n  method: post\n  operationId: createPortForward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /virtual-machines/{virtual_machine_id}/port-forward\n  method: delete\n  operationId: deletePortForward\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bare-metal/locations\n  method: get\n  operationId: listBareMetalLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bare-metal/detailed-locations\n  method: get\n  operationId: listDetailedBareMetalLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bare-metal/\n  method: post\n  operationId: provisionBareMetal\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bare-metal/\n  method: get\n  operationId: listBareMetalRentals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bare-metal/kubernetes\n  method: get\n  operationId: listKubernetes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bare-metal/kubernetes/{cluster_id}/health\n  method: get\n  operationId: getKubernetesHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bare-metal/kubernetes/{cluster_id}/slurm-user\n\
  \  method: post\n  operationId: upsertSlurmUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bare-metal/kubernetes/{cluster_id}/addons/{addon}\n  method: get\n  operationId: getKubernetesAddon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bare-metal/{baremetal_rental_id}\n  method: get\n  operationId: getBareMetalRental\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bare-metal/{baremetal_rental_id}\n  method: delete\n  operationId: terminateBareMetalRental\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bare-metal/{baremetal_rental_id}\n  method: patch\n  operationId: modifyBareMetalRental\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bare-metal/{baremetal_rental_id}/power-status\n  method: put\n  operationId: setBareMetalPowerStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /bare-metal/{baremetal_rental_id}/reboot\n  method: post\n  operationId: rebootBareMetalNodes\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /bare-metal/{baremetal_rental_id}/remove-nodes\n  method: patch\n  operationId: removeBareMetalNodes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/\n  method: patch\n  operationId: updateOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/ssh-keys\n  method: get\n  operationId: listSshKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/ssh-keys\n  method: post\n  operationId: addSshKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/ssh-keys/{ssh_key_id}\n\
  \  method: delete\n  operationId: removeSshKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/address\n  method: get\n  operationId: getOrganizationAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/address\n  method: put\n  operationId: setOrganizationAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/hourly-rate\n  method: get\n  operationId: getStorageHourlyRate\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/\n  method: post\n  operationId: createStorage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/\n  method: get\n  operationId: listStorage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/{storage_id}\n  method: get\n  operationId: getStorage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/{storage_id}\n  method: patch\n  operationId: updateStorage\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/{storage_id}\n  method: delete\n  operationId: terminateStorage\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /storage/{storage_id}/nfs-squash\n  method: patch\n  operationId: updateNfsSquash\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /locations/\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{location_id}\n  method: get\n  operationId: getLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hostnodes/{hostnode_id}\n  method: get\n  operationId: getHostNode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instant-deploy-presets/\n  method: get\n  operationId: listInstantDeployPresets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instant-deploy-presets/{instant_deploy_preset_id}\n  method: get\n  operationId:\
  \ getInstantDeployPreset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/hourly-rate\n  method: get\n  operationId: getHourlyRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/reports/{year}/{month}/transactions\n  method: get\n  operationId: getMonthlyTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /validate/cloudinit\n  method: post\n  operationId: validateCloudInit\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltage-park/refs/heads/main/agentic-access/voltage-park-agentic-access.yml
summary_line: 48 operations · 23 acting · 7 human-in-the-loop
tags:
- GPU
- Cloud
- AI Infrastructure
- H100
- H200
- Bare Metal
---
