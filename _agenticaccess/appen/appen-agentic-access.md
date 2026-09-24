---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 4
api_specs:
- filename: appen-download-api-openapi.yml
  format: yaml
  label: Appen Download API
  slug: appen-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-download-api-openapi.yml
- filename: appen-internal-contributors-api-openapi.yml
  format: yaml
  label: Appen Internal Contributors API
  slug: appen-internal-contributors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-internal-contributors-api-openapi.yml
- filename: appen-jobs-api-openapi.yml
  format: yaml
  label: Appen Jobs API
  slug: appen-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-jobs-api-openapi.yml
- filename: appen-projects-api-openapi.yml
  format: yaml
  label: Appen Projects API
  slug: appen-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-projects-api-openapi.yml
- filename: appen-route-units-api-openapi.yml
  format: yaml
  label: Appen Route Units API
  slug: appen-route-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-route-units-api-openapi.yml
- filename: appen-test-questions-api-openapi.yml
  format: yaml
  label: Appen Test Questions API
  slug: appen-test-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-test-questions-api-openapi.yml
- filename: appen-upload-api-openapi.yml
  format: yaml
  label: Appen Upload API
  slug: appen-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-upload-api-openapi.yml
consequence_counts:
  physical: 1
  read: 4
  write: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Appen Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/project-flow/projects/send-to-job
operation_count: 32
overview: 'Appen exposes 32 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 27 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Appen
provider_slug: appen
slug: appen-agentic-access
source_filename: appen-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: generated\nsource: openapi/appen-openapi-remote.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    acting: 28\n    connected: 4\n  by_consequence:\n    write: 27\n    read: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/jobs/jobs.json\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/jobs/copy-job\n  method: post\n  operationId: copyJob\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/jobs/status\n  method: get\n  operationId: getJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/jobs/update\n  method: put\n  operationId: updateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/jobs/jobStatusById\n  method: get\n  operationId: getJobStatusById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/jobs/pause\n  method: post\n  operationId: pauseJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/jobs/upload.json\n  method: post\n  operationId: uploadDatasetToProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/jobs/upload/status\n  method: get\n  operationId: getUploadStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/project-flow/projects\n\
  \  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/units\n  method: post\n  operationId: listProjectUnits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/copy\n  method: post\n  operationId: copyProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/send-to-job\n  method: post\n  operationId: sendUnitsToJob\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/jobs/launch\n  method: post\n  operationId: launchJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/jobs/download.csv\n  method: post\n  operationId: downloadCsvFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/jobs/dataset-download.csv\n  method: post\n  operationId: downloadDatasetCsvFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/add-test-question\n  method: post\n  operationId: addTestQuestionsToJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/upload-test-question\n  method:\
  \ post\n  operationId: uploadTestQuestions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/update-tq-by-project\n  method: post\n  operationId: updateTestQuestions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/project-status\n  method: get\n  operationId: getProjectStatusV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/project-flow/projects/update-project-settings\n\
  \  method: put\n  operationId: updateProjectSettingsV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/internalcontributor/add-contributor\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/contributor/internalcontributor/upload\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/internalcontributor/edit-contributor\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/internalcontributor/list\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/internalcontributor/create-contributor-group\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/internalcontributor/add-contributors-to-existing-group\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/internalcontributor/list-all-contributor-groups\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/internalcontributor/assign-job\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/internalcontributor/un-assign-job\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/internalcontributor/delete-contributor\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/internalcontributor/delete-contributor-group\n\
  \  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/project-flow/projects/internalcontributor/download-contributors\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/agentic-access/appen-agentic-access.yml
summary_line: 32 operations · 28 acting
tags:
- AI
- Data
- Annotation
- TrainingData
- Enterprise
---
