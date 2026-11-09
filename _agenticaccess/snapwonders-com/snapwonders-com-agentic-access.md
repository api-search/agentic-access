---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 20
api_specs:
- filename: snapwonders-com-analyse-api-openapi.yml
  format: yaml
  label: snapwonders-com Analyse API
  slug: snapwonders-com-analyse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-analyse-api-openapi.yml
- filename: snapwonders-com-convert-api-openapi.yml
  format: yaml
  label: snapwonders-com Convert API
  slug: snapwonders-com-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-convert-api-openapi.yml
- filename: snapwonders-com-hide-api-openapi.yml
  format: yaml
  label: snapwonders-com Hide API
  slug: snapwonders-com-hide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-hide-api-openapi.yml
- filename: snapwonders-com-mcp-api-openapi.yml
  format: yaml
  label: snapwonders-com MCP API
  slug: snapwonders-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-mcp-api-openapi.yml
- filename: snapwonders-com-media-upload-direct-api-openapi.yml
  format: yaml
  label: snapwonders-com Media Upload - Direct API
  slug: snapwonders-com-media-upload-direct-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-media-upload-direct-api-openapi.yml
- filename: snapwonders-com-media-upload-tus-resumable-api-openapi.yml
  format: yaml
  label: snapwonders-com Media Upload - TUS Resumable API
  slug: snapwonders-com-media-upload-tus-resumable-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-media-upload-tus-resumable-api-openapi.yml
- filename: snapwonders-com-reveal-api-openapi.yml
  format: yaml
  label: snapwonders-com Reveal API
  slug: snapwonders-com-reveal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-reveal-api-openapi.yml
- filename: snapwonders-com-status-api-openapi.yml
  format: yaml
  label: snapwonders-com Status API
  slug: snapwonders-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snapwonders-com/openapi/snapwonders-com-status-api-openapi.yml
consequence_counts:
  physical: 1
  read: 20
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Snapwonders Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/upload
operation_count: 33
overview: 'snapwonders-com exposes 33 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: snapwonders-com
provider_slug: snapwonders-com
slug: snapwonders-com-agentic-access
source_filename: snapwonders-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/snapwonders-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    acting: 13\n    connected: 20\n  by_consequence:\n    write: 12\n    read: 20\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/analyse/session\n  method: post\n  operationId: post_api_analyse_session_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analyse/session/{uid}/files\n  method: get\n  operationId: get_api_analyse_session_files\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/analyse/job\n  method: post\n  operationId: post_api_analyse_job_start\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analyse/job/{uid}\n  method: get\n  operationId: get_api_analyse_job_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/analyse/job/{uid}/results\n  method: get\n  operationId: get_api_analyse_job_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/analyse/result/{jobUid}\n\
  \  method: get\n  operationId: get_api_analyse_result_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/analyse/asset/{assetId}\n  method: get\n  operationId: get_api_analyse_asset_download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/convert/session\n  method: post\n  operationId: post_api_convert_session_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/convert/session/{uid}/files\n  method: get\n  operationId: get_api_convert_session_files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/convert/job\n  method: post\n  operationId: post_api_convert_job_start\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/convert/job/{uid}\n  method: get\n  operationId: get_api_convert_job_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/convert/job/{uid}/results\n  method: get\n  operationId: get_api_convert_job_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/convert/download/{assetId}\n  method: get\n  operationId: get_api_convert_download\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: get\n  operationId: get_api_mcp_endpoint_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  operationId: post_api_mcp_endpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp/\n  method: post\n  operationId: post_api_mcp_endpoint_slash\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/status\n  method: get\n  operationId: get_api_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/session\n  method: post\n  operationId: post_api_stego_session_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/session/{uid}/files\n  method: get\n  operationId: get_api_stego_session_files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/job\n  method: post\n  operationId: post_api_stego_job_start\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/job/{uid}\n  method: get\n  operationId: get_api_stego_job_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/job/{uid}/results\n  method: get\n  operationId: get_api_stego_job_results\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/job/download/{assetId}\n  method: get\n  operationId: get_api_stego_file_download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tus\n  method: get\n  operationId: get_app_upload_tus_api\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tus\n  method: post\n  operationId: post_app_upload_tus_api\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tus\n  method: options\n  operationId: options_app_upload_tus_api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tus/{tusId}\n  method: get\n  operationId: get_app_upload_tus_api_chunk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tus/{tusId}\n  method: post\n \
  \ operationId: post_app_upload_tus_api_chunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tus/{tusId}\n  method: delete\n  operationId: delete_app_upload_tus_api_chunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tus/{tusId}\n  method: options\n  operationId: options_app_upload_tus_api_chunk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tus/{tusId}\n  method: head\n  operationId: head_app_upload_tus_api_chunk\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tus/{tusId}\n  method: patch\n  operationId: patch_app_upload_tus_api_chunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/upload\n  method: post\n  operationId: post_app_upload_direct_api\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/snapwonders-com/agentic-access/snapwonders-com-agentic-access.yml
summary_line: 33 operations · 13 acting
tags:
- Forensics
- Steganography
- MediaConversion
- Privacy
- Open Source
---
