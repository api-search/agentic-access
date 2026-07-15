---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 21
api_specs:
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Devices API
  slug: eiger-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Builds API
  slug: eiger-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Print Jobs API
  slug: eiger-print-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Parts API
  slug: eiger-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Printed Parts API
  slug: eiger-printed-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
- filename: markforged-openapi.yml
  format: yaml
  label: Eiger Organizations API
  slug: eiger-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/openapi/markforged-openapi.yml
consequence_counts:
  physical: 3
  read: 21
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Markforged Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /builds/approved
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /backlog/{build_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /devices/{device_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /job-requests/{build_id}
operation_count: 30
overview: 'Markforged exposes 30 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 5 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Markforged
provider_slug: markforged
slug: markforged-agentic-access
source_filename: markforged-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/markforged-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 21\n    acting: 9\n  by_consequence:\n    read: 21\n    physical: 3\n    write: 5\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /devices\n  method: get\n  operationId: listDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{device_id}\n  method: get\n  operationId: getDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /devices/{device_id}\n  method: post\n  operationId: sendBuildToPrinter\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /devices/{device_id}/queue\n  method: get\n  operationId: listDeviceQueue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{device_id}/queue\n  method: post\n  operationId: addBuildToQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /devices/{device_id}/queue/{queued_job_id}\n  method: get\n  operationId: getQueuedJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices/{device_id}/queue/{queued_job_id}\n  method: delete\n  operationId: removeQueuedJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /builds\n  method: get\n  operationId: listBuilds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /builds/{build_id}\n  method: get\n  operationId: getBuild\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /builds/approved\n  method: get\n  operationId: listApprovedBuilds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /builds/approved\n  method: put\n  operationId: updateApprovedBuilds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /builds/approved\n  method: delete\n  operationId: disableBuildApprovals\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /backlog/{build_id}\n  method: post\n  operationId: sendBuildToBacklog\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job-requests/{build_id}\n  method: post\n  operationId: addJobRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job-requests/{build_id}\n  method: delete\n  operationId: removeJobRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /print_jobs\n  method: get\n  operationId: listPrintJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /print_jobs/{print_job_id}\n  method: get\n  operationId: getPrintJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /print_jobs/{print_job_id}/scan_report\n  method: get\n  operationId: getPrintJobScanReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parts/{part_id}\n  method: get\n  operationId: getPart\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parts/upload_stl\n  method: post\n  operationId: uploadStl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /parts/slice_status/{slice_job_id}\n  method: get\n  operationId: getSliceStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /parts/settings_presets\n  method: get\n  operationId: listSettingsPresets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /part_versions/{part_version_id}\n  method: get\n  operationId: getPartVersion\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /part_versions/{part_version_id}/download\n  method: get\n  operationId: getPartVersionDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /printed_parts\n  method: get\n  operationId: listPrintedParts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /printed_parts/{printed_part_id}\n  method: get\n  operationId: getPrintedPart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /printed_parts/{printed_part_id}/scan_report\n  method: get\n  operationId: getPrintedPartScanReport\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_id}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dashboard/custom_analytics_csv\n  method: get\n  operationId: getCustomAnalyticsCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/markforged/refs/heads/main/agentic-access/markforged-agentic-access.yml
summary_line: 30 operations · 9 acting · 1 human-in-the-loop
tags:
- 3D Printing
- Additive Manufacturing
- Industrial
- Eiger
- Fleet Management
---
