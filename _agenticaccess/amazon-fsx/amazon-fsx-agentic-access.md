---
acting_count: 1
action_class_counts:
  acting: 1
api_specs:
- filename: amazon-fsx-filesystems-api-openapi.yml
  format: yaml
  label: Amazon FSx Filesystems API
  slug: amazon-fsx-filesystems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-filesystems-api-openapi.yml
- filename: amazon-fsx-backup-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Backup API
  slug: amazon-fsx-backup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-backup-api-openapi.yml
- filename: amazon-fsx-data-repository-association-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Data Repository Association API
  slug: amazon-fsx-data-repository-association-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-data-repository-association-api-openapi.yml
- filename: amazon-fsx-data-repository-task-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Data Repository Task API
  slug: amazon-fsx-data-repository-task-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-data-repository-task-api-openapi.yml
- filename: amazon-fsx-file-cache-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx File Cache API
  slug: amazon-fsx-file-cache-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-file-cache-api-openapi.yml
- filename: amazon-fsx-file-system-aliase-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx File System Aliase API
  slug: amazon-fsx-file-system-aliase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-file-system-aliase-api-openapi.yml
- filename: amazon-fsx-operations-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Operations API
  slug: amazon-fsx-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-operations-api-openapi.yml
- filename: amazon-fsx-snapshot-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Snapshot API
  slug: amazon-fsx-snapshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-snapshot-api-openapi.yml
- filename: amazon-fsx-storage-virtual-machine-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Storage Virtual Machine API
  slug: amazon-fsx-storage-virtual-machine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-storage-virtual-machine-api-openapi.yml
- filename: amazon-fsx-volume-api-openapi.yml
  format: yaml
  label: Amazon FSx Fsx Volume API
  slug: amazon-fsx-volume-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-fsx/openapi/amazon-fsx-volume-api-openapi.yml
consequence_counts:
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Fsx Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 1
overview: 'Amazon FSx exposes 1 API operation that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon FSx
provider_slug: amazon-fsx
slug: amazon-fsx-agentic-access
source_filename: amazon-fsx-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-fsx-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1\n  by_action_class:\n    acting: 1\n  by_consequence:\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: CreateFileSystem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/amazon-fsx/agentic-access/amazon-fsx-agentic-access.yml
summary_line: 1 operation · 1 acting
tags:
- Amazon Web Services
- Filesystem
- Lustre
- NetApp
- OpenZFS
- Storage
- Windows
---
