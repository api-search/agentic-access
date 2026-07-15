---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: allianz-future-cloud-platform-services.yaml
  format: yaml
  label: Allianz Future Cloud Platform Services API
  slug: platform-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/openapi/allianz-future-cloud-platform-services.yaml
- filename: allianz-future-cloud-platform-policy.yaml
  format: yaml
  label: Allianz Insurance Policy Microservice API
  slug: policy-microservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/openapi/allianz-future-cloud-platform-policy.yaml
consequence_counts:
  physical: 2
  read: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Allianz Future Cloud Platform Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /infrastructure/resources
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /services/{service_id}/deployments
operation_count: 8
overview: 'Allianz Future Cloud Platform exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 1 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
slug: allianz-future-cloud-platform-agentic-access
source_filename: allianz-future-cloud-platform-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/allianz-future-cloud-platform-services.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 5\n    acting: 3\n  by_consequence:\n    read: 5\n    write: 1\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /services\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services\n  method: post\n  operationId: registerService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/{service_id}\n  method: get\n  operationId: getService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{service_id}/deployments\n  method: get\n  operationId: listDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{service_id}/deployments\n  method: post\n  operationId: deployService\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /namespaces\n  method: get\n  operationId: listNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /observability/metrics\n  method: get\n  operationId: getMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /infrastructure/resources\n  method: post\n  operationId: provisionResource\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/agentic-access/allianz-future-cloud-platform-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
---
