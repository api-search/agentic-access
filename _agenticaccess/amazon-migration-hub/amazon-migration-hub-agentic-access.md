---
acting_count: 17
action_class_counts:
  acting: 17
api_specs:
- filename: amazon-migration-hub-openapi-original.yml
  format: yaml
  label: Amazon Migration Hub API
  slug: migration-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/openapi/amazon-migration-hub-openapi-original.yml
consequence_counts:
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Migration Hub Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Amazon Migration Hub exposes 17 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
slug: amazon-migration-hub-agentic-access
source_filename: amazon-migration-hub-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-migration-hub-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 17\n  by_consequence:\n    write: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /#X-Amz-Target=AWSMigrationHub.AssociateCreatedArtifact\n  method: post\n  operationId: AssociateCreatedArtifact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.AssociateDiscoveredResource\n  method: post\n\
  \  operationId: AssociateDiscoveredResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.CreateProgressUpdateStream\n  method: post\n  operationId: CreateProgressUpdateStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.DeleteProgressUpdateStream\n  method: post\n  operationId: DeleteProgressUpdateStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.DescribeApplicationState\n  method: post\n  operationId: DescribeApplicationState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.DescribeMigrationTask\n  method: post\n  operationId: DescribeMigrationTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.DisassociateCreatedArtifact\n  method:\
  \ post\n  operationId: DisassociateCreatedArtifact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.DisassociateDiscoveredResource\n  method: post\n  operationId: DisassociateDiscoveredResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.ImportMigrationTask\n  method: post\n  operationId: ImportMigrationTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.ListApplicationStates\n  method: post\n  operationId: ListApplicationStates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.ListCreatedArtifacts\n  method: post\n  operationId: ListCreatedArtifacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.ListDiscoveredResources\n  method: post\n  operationId:\
  \ ListDiscoveredResources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.ListMigrationTasks\n  method: post\n  operationId: ListMigrationTasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.ListProgressUpdateStreams\n  method: post\n  operationId: ListProgressUpdateStreams\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.NotifyApplicationState\n  method: post\n  operationId: NotifyApplicationState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.NotifyMigrationTaskState\n  method: post\n  operationId: NotifyMigrationTaskState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSMigrationHub.PutResourceAttributes\n  method: post\n  operationId: PutResourceAttributes\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/agentic-access/amazon-migration-hub-agentic-access.yml
summary_line: 17 operations · 17 acting
tags:
- Broadcasting
- Media Processing
- Media
---
