---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 4
api_specs:
- filename: vmwareengine-openapi.yml
  format: yaml
  label: Google Cloud VMware Engine API
  slug: google-cloud-vmware-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-vmware-engine/refs/heads/main/openapi/vmwareengine-openapi.yml
consequence_counts:
  read: 4
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Vmware Engine Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Google Cloud VMware Engine exposes 7 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud VMware Engine
provider_slug: google-cloud-vmware-engine
slug: google-cloud-vmware-engine-agentic-access
source_filename: google-cloud-vmware-engine-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vmwareengine-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 4\n    acting: 3\n  by_consequence:\n    read: 4\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/{project}/locations/{location}/privateClouds\n  method: get\n  operationId: listPrivateClouds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /projects/{project}/locations/{location}/privateClouds\n  method: post\n  operationId: createPrivateCloud\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /projects/{project}/locations/{location}/privateClouds/{privateCloudId}\n  method: get\n  operationId: getPrivateCloud\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /projects/{project}/locations/{location}/privateClouds/{privateCloudId}\n  method: delete\n  operationId: deletePrivateCloud\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /projects/{project}/locations/{location}/privateClouds/{privateCloudId}/clusters\n  method: get\n  operationId: listClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /projects/{project}/locations/{location}/privateClouds/{privateCloudId}/clusters\n  method: post\n  operationId: createCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n- path: /projects/{project}/locations/{location}/networkPolicies\n\
  \  method: get\n  operationId: listNetworkPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-vmware-engine/refs/heads/main/agentic-access/google-cloud-vmware-engine-agentic-access.yml
summary_line: 7 operations · 3 acting
tags:
- Compute
- Google Cloud
- Migration
- Private Cloud
- Virtualization
- VMware
---
