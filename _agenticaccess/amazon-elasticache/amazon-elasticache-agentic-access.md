---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: amazon-elasticache-amazon-elasticache-api-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Amazon ElastiCache API
  slug: amazon-elasticache-amazon-elasticache-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-amazon-elasticache-api-api-openapi.yml
- filename: amazon-elasticache-cache-parameter-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Cache Parameter Group API
  slug: amazon-elasticache-cache-parameter-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-cache-parameter-group-api-openapi.yml
- filename: amazon-elasticache-cache-security-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Cache Security Group API
  slug: amazon-elasticache-cache-security-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-cache-security-group-api-openapi.yml
- filename: amazon-elasticache-cache-subnet-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Cache Subnet Group API
  slug: amazon-elasticache-cache-subnet-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-cache-subnet-group-api-openapi.yml
- filename: amazon-elasticache-global-replication-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Global Replication Group API
  slug: amazon-elasticache-global-replication-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-global-replication-group-api-openapi.yml
- filename: amazon-elasticache-migration-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Migration API
  slug: amazon-elasticache-migration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-migration-api-openapi.yml
- filename: amazon-elasticache-operations-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Operations API
  slug: amazon-elasticache-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-operations-api-openapi.yml
- filename: amazon-elasticache-serverless-cache-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Serverless Cache API
  slug: amazon-elasticache-serverless-cache-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-serverless-cache-api-openapi.yml
- filename: amazon-elasticache-serverless-cache-snapshot-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Serverless Cache Snapshot API
  slug: amazon-elasticache-serverless-cache-snapshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-serverless-cache-snapshot-api-openapi.yml
- filename: amazon-elasticache-snapshot-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Snapshot API
  slug: amazon-elasticache-snapshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-snapshot-api-openapi.yml
- filename: amazon-elasticache-tag-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Tag API
  slug: amazon-elasticache-tag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-tag-api-openapi.yml
- filename: amazon-elasticache-update-action-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache Update Action API
  slug: amazon-elasticache-update-action-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-update-action-api-openapi.yml
- filename: amazon-elasticache-user-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache User API
  slug: amazon-elasticache-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-user-api-openapi.yml
- filename: amazon-elasticache-user-group-api-openapi.yml
  format: yaml
  label: Amazon ElastiCache Elasticache User Group API
  slug: amazon-elasticache-user-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-elasticache/openapi/amazon-elasticache-user-group-api-openapi.yml
consequence_counts:
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Elasticache Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Amazon ElastiCache exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon ElastiCache
provider_slug: amazon-elasticache
slug: amazon-elasticache-agentic-access
source_filename: amazon-elasticache-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-elasticache-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    write: 3\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: createCacheCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: describeCacheClusters\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#DeleteCacheCluster\n  method: post\n  operationId: deleteCacheCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#CreateReplicationGroup\n  method: post\n  operationId: createReplicationGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeReplicationGroups\n  method: get\n  operationId: describeReplicationGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/amazon-elasticache/agentic-access/amazon-elasticache-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- Amazon Web Services
- Caching
- Database
- ElastiCache
- In-Memory
- Memcached
- Redis
---
