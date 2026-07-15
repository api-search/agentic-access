---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: amazon-rds-openapi.yml
  format: yaml
  label: Amazon RDS API
  slug: amazon-rds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/openapi/amazon-rds-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Rds Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Amazon RDS exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon RDS
provider_slug: amazon-rds
slug: amazon-rds-agentic-access
source_filename: amazon-rds-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-rds-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /?Action=CreateDBInstance\n  method: get\n  operationId: createDBInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeDBInstances\n  method: get\n  operationId: describeDBInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=ModifyDBInstance\n\
  \  method: get\n  operationId: modifyDBInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DeleteDBInstance\n  method: get\n  operationId: deleteDBInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=RebootDBInstance\n  method: get\n  operationId: rebootDBInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=CreateDBSnapshot\n  method: get\n  operationId: createDBSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeDBSnapshots\n  method: get\n  operationId: describeDBSnapshots\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DeleteDBSnapshot\n  method: get\n  operationId: deleteDBSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=CreateDBCluster\n  method: get\n  operationId: createDBCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DescribeDBClusters\n  method: get\n  operationId: describeDBClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /?Action=DeleteDBCluster\n  method: get\n  operationId: deleteDBCluster\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /?Action=DescribeDBEngineVersions\n  method: get\n  operationId: describeDBEngineVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/agentic-access/amazon-rds-agentic-access.yml
summary_line: 12 operations
tags:
- Cloud Databases
- Database Service
- DBaaS
- Managed Databases
- Relational Databases
---
