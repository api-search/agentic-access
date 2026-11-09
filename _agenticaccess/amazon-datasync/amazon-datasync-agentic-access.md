---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 1
api_specs:
- filename: amazon-datasync-amazon-datasync-rest-api-api-openapi.yml
  format: yaml
  label: Amazon DataSync Amazon DataSync REST API
  slug: amazon-datasync-amazon-datasync-rest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-amazon-datasync-rest-api-api-openapi.yml
- filename: amazon-datasync-agent-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Agent API
  slug: amazon-datasync-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-agent-api-openapi.yml
- filename: amazon-datasync-location-azure-blob-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Azure Blob API
  slug: amazon-datasync-location-azure-blob-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-azure-blob-api-openapi.yml
- filename: amazon-datasync-location-ef-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Ef API
  slug: amazon-datasync-location-ef-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-ef-api-openapi.yml
- filename: amazon-datasync-location-fsx-lustre-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Fsx Lustre API
  slug: amazon-datasync-location-fsx-lustre-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-fsx-lustre-api-openapi.yml
- filename: amazon-datasync-location-fsx-ontap-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Fsx Ontap API
  slug: amazon-datasync-location-fsx-ontap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-fsx-ontap-api-openapi.yml
- filename: amazon-datasync-location-fsx-open-zf-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Fsx Open Zf API
  slug: amazon-datasync-location-fsx-open-zf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-fsx-open-zf-api-openapi.yml
- filename: amazon-datasync-location-fsx-window-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Fsx Window API
  slug: amazon-datasync-location-fsx-window-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-fsx-window-api-openapi.yml
- filename: amazon-datasync-location-hdf-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Hdf API
  slug: amazon-datasync-location-hdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-hdf-api-openapi.yml
- filename: amazon-datasync-location-nf-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Nf API
  slug: amazon-datasync-location-nf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-nf-api-openapi.yml
- filename: amazon-datasync-location-object-storage-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Object Storage API
  slug: amazon-datasync-location-object-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-object-storage-api-openapi.yml
- filename: amazon-datasync-location-smb-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Smb API
  slug: amazon-datasync-location-smb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-smb-api-openapi.yml
- filename: amazon-datasync-operations-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Operations API
  slug: amazon-datasync-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-operations-api-openapi.yml
- filename: amazon-datasync-task-execution-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Task Execution API
  slug: amazon-datasync-task-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-task-execution-api-openapi.yml
consequence_counts:
  read: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Datasync Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Amazon DataSync exposes 6 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon DataSync
provider_slug: amazon-datasync
slug: amazon-datasync-agentic-access
source_filename: amazon-datasync-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/amazon-datasync-amazon-datasync-rest-api-api-openapi.yml, openapi/amazon-datasync-create-agent-api-openapi.yml,\n  openapi/amazon-datasync-createlocations3-api-openapi.yml, openapi/amazon-datasync-describetask-api-openapi.yml,\n  openapi/amazon-datasync-listtasks-api-openapi.yml, openapi/amazon-datasync-starttaskexecution-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 5\n    connected: 1\n  by_consequence:\n    write: 5\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: createTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#CreateAgent\n  method: post\n  operationId: createAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#CreateLocationS3\n  method: post\n  operationId: createLocationS3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeTask\n  method: post\n  operationId: describeTask\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#ListTasks\n  method: post\n  operationId: listTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /#StartTaskExecution\n  method: post\n  operationId: startTaskExecution\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/amazon-datasync/agentic-access/amazon-datasync-agentic-access.yml
summary_line: 6 operations · 5 acting
tags:
- Amazon Web Services
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
---
