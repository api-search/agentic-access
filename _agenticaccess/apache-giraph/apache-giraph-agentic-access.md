---
acting_count: 0
action_class_counts:
  connected: 3
api_specs:
- filename: apache-giraph-job-openapi.yml
  format: yaml
  label: Apache Giraph Job Monitoring API
  slug: apache-giraph-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-giraph/refs/heads/main/openapi/apache-giraph-job-openapi.yml
consequence_counts:
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apache Giraph Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Apache Giraph exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apache Giraph
provider_slug: apache-giraph
slug: apache-giraph-agentic-access
source_filename: apache-giraph-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/apache-giraph-job-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 3\n  by_consequence:\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /ws/v1/cluster/apps\n  method: get\n  operationId: listGiraphJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/v1/cluster/apps/{appId}\n  method: get\n  operationId: getGiraphJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ws/v1/cluster/metrics\n  method: get\n\
  \  operationId: getClusterMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-giraph/refs/heads/main/agentic-access/apache-giraph-agentic-access.yml
summary_line: 3 operations
tags:
- Apache
- Big Data
- BSP
- Graph Processing
- Hadoop
- Open Source
- Retired
---
