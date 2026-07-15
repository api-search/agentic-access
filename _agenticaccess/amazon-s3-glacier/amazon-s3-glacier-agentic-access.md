---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 3
api_specs:
- filename: amazon-s3-glacier-openapi.yml
  format: yaml
  label: Amazon S3 Glacier API
  slug: amazon-s3-glacier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-s3-glacier/refs/heads/main/openapi/amazon-s3-glacier-openapi.yml
consequence_counts:
  read: 3
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon S3 Glacier Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Amazon S3 Glacier exposes 7 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon S3 Glacier
provider_slug: amazon-s3-glacier
slug: amazon-s3-glacier-agentic-access
source_filename: amazon-s3-glacier-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-s3-glacier-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 3\n    acting: 4\n  by_consequence:\n    read: 3\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /{accountId}/vaults\n  method: get\n  operationId: listVaults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{accountId}/vaults/{vaultName}\n  method: put\n  operationId: createVault\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{accountId}/vaults/{vaultName}\n  method: get\n  operationId: describeVault\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{accountId}/vaults/{vaultName}\n  method: delete\n  operationId: deleteVault\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{accountId}/vaults/{vaultName}/archives\n  method: post\n  operationId: uploadArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{accountId}/vaults/{vaultName}/jobs\n  method: post\n  operationId: initiateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{accountId}/vaults/{vaultName}/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3-glacier/refs/heads/main/agentic-access/amazon-s3-glacier-agentic-access.yml
summary_line: 7 operations · 4 acting
tags:
- Archive
- Backup
- Storage
---
