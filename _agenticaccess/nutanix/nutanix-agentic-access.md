---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 23
api_specs:
- filename: nutanix-alerts-api-openapi.yml
  format: yaml
  label: Nutanix Alerts API
  slug: nutanix-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-alerts-api-openapi.yml
- filename: nutanix-categories-api-openapi.yml
  format: yaml
  label: Nutanix Categories API
  slug: nutanix-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-categories-api-openapi.yml
- filename: nutanix-clusters-api-openapi.yml
  format: yaml
  label: Nutanix Clusters API
  slug: nutanix-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-clusters-api-openapi.yml
- filename: nutanix-hosts-api-openapi.yml
  format: yaml
  label: Nutanix Hosts API
  slug: nutanix-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-hosts-api-openapi.yml
- filename: nutanix-images-api-openapi.yml
  format: yaml
  label: Nutanix Images API
  slug: nutanix-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-images-api-openapi.yml
- filename: nutanix-network-security-rules-api-openapi.yml
  format: yaml
  label: Nutanix Network Security Rules API
  slug: nutanix-network-security-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-network-security-rules-api-openapi.yml
- filename: nutanix-projects-api-openapi.yml
  format: yaml
  label: Nutanix Projects API
  slug: nutanix-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-projects-api-openapi.yml
- filename: nutanix-protection-domains-api-openapi.yml
  format: yaml
  label: Nutanix Protection Domains API
  slug: nutanix-protection-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-protection-domains-api-openapi.yml
- filename: nutanix-snapshots-api-openapi.yml
  format: yaml
  label: Nutanix Snapshots API
  slug: nutanix-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-snapshots-api-openapi.yml
- filename: nutanix-storage-containers-api-openapi.yml
  format: yaml
  label: Nutanix Storage Containers API
  slug: nutanix-storage-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-storage-containers-api-openapi.yml
- filename: nutanix-storage-pools-api-openapi.yml
  format: yaml
  label: Nutanix Storage Pools API
  slug: nutanix-storage-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-storage-pools-api-openapi.yml
- filename: nutanix-subnets-api-openapi.yml
  format: yaml
  label: Nutanix Subnets API
  slug: nutanix-subnets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-subnets-api-openapi.yml
- filename: nutanix-virtual-disks-api-openapi.yml
  format: yaml
  label: Nutanix Virtual Disks API
  slug: nutanix-virtual-disks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-virtual-disks-api-openapi.yml
- filename: nutanix-vms-api-openapi.yml
  format: yaml
  label: Nutanix VMs API
  slug: nutanix-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-vms-api-openapi.yml
- filename: nutanix-webhooks-api-openapi.yml
  format: yaml
  label: Nutanix Webhooks API
  slug: nutanix-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-webhooks-api-openapi.yml
consequence_counts:
  read: 23
  write: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nutanix Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 54
overview: 'Nutanix exposes 54 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read and 31 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nutanix
provider_slug: nutanix
slug: nutanix-agentic-access
source_filename: nutanix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nutanix-prism-central-v3-openapi.yml, openapi/nutanix-prism-element-v2-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    acting: 31\n    connected: 23\n  by_consequence:\n    write: 31\n    read: 23\n  human_in_the_loop_required: 0\noperations:\n- path: /vms/list\n  method: post\n  operationId: listVms\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vms\n  method: post\n  operationId: createVm\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vms/{uuid}\n  method: get\n  operationId: getVm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vms/{uuid}\n  method: put\n  operationId: updateVm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vms/{uuid}\n  method: delete\n  operationId: deleteVm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters/list\n  method: post\n  operationId: listClusters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters/{uuid}\n  method: get\n  operationId: getCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subnets/list\n  method: post\n  operationId: listSubnets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /subnets\n  method: post\n  operationId: createSubnet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subnets/{uuid}\n  method: get\n  operationId: getSubnet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subnets/{uuid}\n  method: put\n  operationId: updateSubnet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subnets/{uuid}\n  method: delete\n  operationId: deleteSubnet\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/list\n  method: post\n  operationId: listImages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images\n  method: post\n  operationId: createImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /images/{uuid}\n  method: get\n  operationId:\
  \ getImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images/{uuid}\n  method: delete\n  operationId: deleteImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /categories/{name}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{name}\n  method: put\n  operationId: updateCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /categories/{name}\n  method: delete\n  operationId: deleteCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /categories/{name}/{value}\n  method: put\n  operationId: updateCategoryValue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /categories/{name}/{value}\n  method: delete\n  operationId: deleteCategoryValue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/list\n  method: post\n  operationId: listProjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{uuid}\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hosts/list\n  method: post\n  operationId: listHosts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /hosts/{uuid}\n  method: get\n  operationId: getHost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network_security_rules/list\n  method: post\n  operationId: listNetworkSecurityRules\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network_security_rules\n  method: post\n  operationId: createNetworkSecurityRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /network_security_rules/{uuid}\n  method: get\n  operationId: getNetworkSecurityRule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network_security_rules/{uuid}\n  method: put\n  operationId: updateNetworkSecurityRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network_security_rules/{uuid}\n  method: delete\n  operationId: deleteNetworkSecurityRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/list\n\
  \  method: post\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{uuid}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{uuid}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{uuid}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cluster\n  method: get\n  operationId: getCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage_containers\n  method: get\n  operationId: listStorageContainers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /storage_containers\n  method: post\n  operationId: createStorageContainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage_containers/{id}\n  method: get\n  operationId: getStorageContainer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage_containers/{id}\n  method: put\n  operationId: updateStorageContainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage_containers/{id}\n\
  \  method: delete\n  operationId: deleteStorageContainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage_pools\n  method: get\n  operationId: listStoragePools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage_pools/{id}\n  method: get\n  operationId: getStoragePool\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hosts\n  method: get\n  operationId: listHosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hosts/{id}\n \
  \ method: get\n  operationId: getHost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vms\n  method: get\n  operationId: listVms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vms/{id}\n  method: get\n  operationId: getVm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vms/{id}/set_power_state\n  method: post\n  operationId: setVmPowerState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virtual_disks\n  method: get\n  operationId:\
  \ listVirtualDisks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /protection_domains\n  method: get\n  operationId: listProtectionDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /protection_domains\n  method: post\n  operationId: createProtectionDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /snapshots\n  method: get\n  operationId: listSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts\n  method: get\n \
  \ operationId: listAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts/{id}\n  method: get\n  operationId: getAlert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/agentic-access/nutanix-agentic-access.yml
summary_line: 54 operations · 31 acting
tags:
- Cloud Management
- Hyperconverged
- Infrastructure
- Virtualization
- Kubernetes
- Database
---
