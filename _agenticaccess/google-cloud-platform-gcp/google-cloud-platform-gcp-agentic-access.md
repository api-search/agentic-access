---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: rest
  format: yaml
  label: Compute Engine API
  slug: compute-engine-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/compute/v1/rest
- filename: rest
  format: yaml
  label: Cloud Storage API
  slug: cloud-storage-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/storage/v1/rest
- filename: rest
  format: yaml
  label: BigQuery API
  slug: bigquery-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/bigquery/v2/rest
- filename: rest
  format: yaml
  label: Cloud Functions API
  slug: cloud-functions-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/cloudfunctions/v2/rest
- filename: rest
  format: yaml
  label: Kubernetes Engine API
  slug: kubernetes-engine-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/container/v1/rest
- filename: rest
  format: yaml
  label: Cloud Pub/Sub API
  slug: cloud-pubsub-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/pubsub/v1/rest
- filename: rest
  format: yaml
  label: Cloud Vision API
  slug: cloud-vision-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/vision/v1/rest
- filename: rest
  format: yaml
  label: Cloud SQL Admin API
  slug: cloud-sql-admin-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/sqladmin/v1/rest
- filename: rest
  format: yaml
  label: Cloud Run API
  slug: cloud-run-api
  spec_type: OpenAPI
  url: https://www.googleapis.com/discovery/v1/apis/run/v2/rest
consequence_counts:
  read: 6
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Platform Gcp Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Google Cloud Platform exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform-gcp
slug: google-cloud-platform-gcp-agentic-access
source_filename: google-cloud-platform-gcp-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-cloud-platform-gcp-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 6\n    acting: 4\n  by_consequence:\n    read: 6\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/{project}/zones/{zone}/instances\n  method: get\n  operationId: listInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - compute\n- path: /projects/{project}/zones/{zone}/instances\n  method: post\n  operationId: insertInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - compute\n- path: /projects/{project}/zones/{zone}/instances/{instance}\n  method: get\n  operationId: getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - compute\n- path: /projects/{project}/zones/{zone}/instances/{instance}\n  method: delete\n  operationId: deleteInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - compute\n- path:\
  \ /projects/{project}/zones/{zone}/disks\n  method: get\n  operationId: listDisks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - compute\n- path: /projects/{project}/zones/{zone}/disks\n  method: post\n  operationId: insertDisk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - compute\n- path: /projects/{project}/global/networks\n  method: get\n  operationId: listNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - compute\n- path: /projects/{project}/global/firewalls\n\
  \  method: get\n  operationId: listFirewalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - compute\n- path: /projects/{project}/global/firewalls\n  method: post\n  operationId: insertFirewall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - compute\n- path: /projects/{project}/zones/{zone}/machineTypes\n  method: get\n  operationId: listMachineTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - compute\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform-gcp/refs/heads/main/agentic-access/google-cloud-platform-gcp-agentic-access.yml
summary_line: 10 operations · 4 acting
tags:
- Cloud Computing
- Data Analytics
- IaaS
- Machine Learning
- PaaS
- SaaS
- Serverless
---
