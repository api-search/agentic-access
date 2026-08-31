---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 1
api_specs:
- filename: cloudmersive-scan-api-openapi.yml
  format: yaml
  label: Cloudmersive Scan API
  slug: cloudmersive-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudmersive/refs/heads/main/openapi/cloudmersive-scan-api-openapi.yml
- filename: cloudmersive-scancloudstorage-api-openapi.yml
  format: yaml
  label: Cloudmersive ScanCloudStorage API
  slug: cloudmersive-scancloudstorage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudmersive/refs/heads/main/openapi/cloudmersive-scancloudstorage-api-openapi.yml
consequence_counts:
  read: 1
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cloudmersive Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Cloudmersive exposes 13 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cloudmersive
provider_slug: cloudmersive
slug: cloudmersive-agentic-access
source_filename: cloudmersive-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cloudmersive-virus-scan-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 12\n    connected: 1\n  by_consequence:\n    write: 12\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /virus/scan/file\n  method: post\n  operationId: Scan_File\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virus/scan/file/advanced\n  method: post\n  operationId: Scan_FileAdvanced\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virus/scan/website\n  method: post\n  operationId: Scan_Website\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virus/scan/cloud-storage/azure-blob/single\n  method: post\n  operationId: ScanCloudStorage_ScanAzureBlob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /virus/scan/cloud-storage/azure-blob/single/advanced\n  method: post\n  operationId: ScanCloudStorage_ScanAzureBlobAdvanced\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virus/scan/cloud-storage/azure-blob/single/advanced/batch-job\n  method: post\n  operationId: ScanCloudStorage_ScanAzureBlobAdvancedBatchJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virus/scan/cloud-storage/aws-s3/single\n  method: post\n  operationId: ScanCloudStorage_ScanAwsS3File\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virus/scan/cloud-storage/aws-s3/single/advanced\n  method: post\n  operationId: ScanCloudStorage_ScanAwsS3FileAdvanced\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virus/scan/cloud-storage/sharepoint-online/site/single\n  method: post\n  operationId: ScanCloudStorage_ScanSharePointOnlineFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /virus/scan/cloud-storage/sharepoint-online/site/advanced\n  method: post\n  operationId: ScanCloudStorage_ScanSharePointOnlineFileAdvanced\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virus/scan/cloud-storage/gcp-storage/single\n  method: post\n  operationId: ScanCloudStorage_ScanGcpStorageFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virus/scan/cloud-storage/gcp-storage/single/advanced\n  method: post\n  operationId: ScanCloudStorage_ScanGcpStorageFileAdvanced\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /virus/scan/cloud-storage/batch-job/status\n  method: get\n  operationId: ScanCloudStorage_GetAsyncJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudmersive/refs/heads/main/agentic-access/cloudmersive-agentic-access.yml
summary_line: 13 operations · 12 acting
tags:
- Barcodes
- Conversions
- Documents
- Image Recognition
- Natural Language
- OCR
- Processing
- Validation
- Virus Scanning
---
