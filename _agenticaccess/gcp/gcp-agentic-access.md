---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 9
api_specs:
- filename: rest
  format: yaml
  label: Compute Engine API
  slug: compute-engine
  spec_type: OpenAPI
  url: https://compute.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Storage API
  slug: cloud-storage
  spec_type: OpenAPI
  url: https://storage.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Functions API
  slug: cloud-functions
  spec_type: OpenAPI
  url: https://cloudfunctions.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Pub/Sub API
  slug: cloud-pubsub
  spec_type: OpenAPI
  url: https://pubsub.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: BigQuery API
  slug: bigquery
  spec_type: OpenAPI
  url: https://bigquery.googleapis.com/$discovery/rest?version=v2
- filename: rest
  format: yaml
  label: Cloud Vision API
  slug: cloud-vision
  spec_type: OpenAPI
  url: https://vision.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Natural Language API
  slug: cloud-natural-language
  spec_type: OpenAPI
  url: https://language.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Kubernetes Engine API
  slug: kubernetes-engine
  spec_type: OpenAPI
  url: https://container.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud SQL Admin API
  slug: cloud-sql
  spec_type: OpenAPI
  url: https://sqladmin.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Firestore API
  slug: cloud-firestore
  spec_type: OpenAPI
  url: https://firestore.googleapis.com/$discovery/rest?version=v1
consequence_counts:
  read: 9
  safety-critical: 2
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Gcp Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /projects/{project}/zones/{zone}/instances/{instance}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /projects/{project}/zones/{zone}/instances/{instance}/stop
operation_count: 18
overview: 'Google Cloud Platform APIs exposes 18 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 7 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Platform APIs
provider_slug: gcp
slug: gcp-agentic-access
source_filename: gcp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gcp-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 9\n    acting: 9\n  by_consequence:\n    read: 9\n    write: 7\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /projects/{project}/zones/{zone}/instances\n  method: get\n  operationId: listInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/zones/{zone}/instances\n  method: post\n  operationId: insertInstance\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/zones/{zone}/instances/{instance}\n  method: get\n  operationId: getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/zones/{zone}/instances/{instance}\n  method: delete\n  operationId: deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/zones/{zone}/instances/{instance}/start\n  method: post\n  operationId: startInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/zones/{zone}/instances/{instance}/stop\n  method: post\n  operationId: stopInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/zones/{zone}/instances/{instance}/reset\n  method: post\n  operationId: resetInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/zones/{zone}/disks\n  method: get\n  operationId: listDisks\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/zones/{zone}/disks\n  method: post\n  operationId: insertDisk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/zones/{zone}/disks/{disk}\n  method: get\n  operationId: getDisk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n\
  - path: /projects/{project}/zones/{zone}/disks/{disk}\n  method: delete\n  operationId: deleteDisk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/images\n  method: get\n  operationId: listImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/snapshots\n  method: get\n  operationId: listSnapshots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/networks\n  method: get\n  operationId: listNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/networks\n  method: post\n  operationId: insertNetwork\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n\
  - path: /projects/{project}/global/firewalls\n  method: get\n  operationId: listFirewalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/global/firewalls\n  method: post\n  operationId: insertFirewall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n- path: /projects/{project}/zones/{zone}/machineTypes\n  method: get\n  operationId: listMachineTypes\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - https://www.googleapis.com/auth/cloud-platform\n    - https://www.googleapis.com/auth/compute\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/agentic-access/gcp-agentic-access.yml
summary_line: 18 operations · 9 acting · 2 human-in-the-loop
tags:
- Cloud Computing
- Databases
- Infrastructure
- Machine Learning
- Networking
- Security
- Serverless
- Storage
---
