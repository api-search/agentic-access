---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 16
api_specs:
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore CDN API
  slug: cdn
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Cloud API
  slug: cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Object Storage API
  slug: storage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore DNS API
  slug: dns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Streaming API
  slug: streaming
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Everywhere Inference API
  slug: inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore Security & WAAP API
  slug: security-waap
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
- filename: gcore-openapi.yml
  format: yaml
  label: Gcore FastEdge API
  slug: fastedge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/openapi/gcore-openapi.yml
consequence_counts:
  physical: 2
  read: 16
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gcore Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cloud/v3/inference/{project_id}/deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /storage/provisioning/v1/storage
operation_count: 31
overview: 'Gcore exposes 31 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 13 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gcore
provider_slug: gcore
slug: gcore-agentic-access
source_filename: gcore-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gcore-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 16\n    acting: 15\n  by_consequence:\n    read: 16\n    write: 13\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /cdn/resources\n  method: get\n  operationId: listCdnResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cdn/resources\n  method: post\n  operationId: createCdnResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cdn/resources/{resource_id}\n  method: get\n  operationId: getCdnResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cdn/resources/{resource_id}\n  method: put\n  operationId: updateCdnResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cdn/resources/{resource_id}\n  method: delete\n  operationId: deleteCdnResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cdn/resources/{resource_id}/rules\n  method: get\n  operationId: listCdnRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cdn/resources/{resource_id}/rules\n  method: post\n  operationId: createCdnRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cdn/resources/{resource_id}/purge\n  method: post\n  operationId: purgeCdnResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /cdn/public-ip-list\n  method: get\n  operationId: getCdnPublicIpList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cloud/v1/instances/{project_id}/{region_id}\n  method: get\n  operationId: listInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cloud/v1/instances/{project_id}/{region_id}\n  method: post\n  operationId: createInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cloud/v1/instances/{project_id}/{region_id}/{instance_id}\n  method: get\n  operationId: getInstance\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cloud/v1/instances/{project_id}/{region_id}/{instance_id}\n  method: delete\n  operationId: deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cloud/v1/volumes/{project_id}/{region_id}\n  method: get\n  operationId: listVolumes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cloud/v1/volumes/{project_id}/{region_id}\n  method: post\n  operationId: createVolume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cloud/v1/networks/{project_id}/{region_id}\n  method: get\n  operationId: listNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cloud/v3/inference/{project_id}/deployments\n  method: get\n  operationId: listInferenceDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cloud/v3/inference/{project_id}/deployments\n  method: post\n  operationId: createInferenceDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /storage/provisioning/v1/storage\n  method: get\n  operationId: listStorages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /storage/provisioning/v1/storage\n  method: post\n  operationId: createStorage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dns/v2/zones\n  method: get\n  operationId: listZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dns/v2/zones\n  method: post\n  operationId:\
  \ createZone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dns/v2/zones/{zoneName}/{rrsetName}/{rrsetType}\n  method: post\n  operationId: createRRset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streaming/videos\n  method: get\n  operationId: listVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streaming/videos\n  method: post\n  operationId: createVideo\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streaming/videos/{video_id}\n  method: get\n  operationId: getVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streaming/streams\n  method: get\n  operationId: listStreams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streaming/streams\n  method: post\n  operationId: createStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /waap/v1/domains\n  method: get\n  operationId: listWaapDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fastedge/v1/apps\n  method: get\n  operationId: listFastEdgeApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fastedge/v1/apps\n  method: post\n  operationId: createFastEdgeApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gcore/refs/heads/main/agentic-access/gcore-agentic-access.yml
summary_line: 31 operations · 15 acting
tags:
- Edge Cloud
- CDN
- Streaming
- Edge AI
- Infrastructure
---
