---
acting_count: 26
action_class_counts:
  acting: 26
  connected: 18
api_specs:
- filename: fountain-com-openapi.yml
  format: yaml
  label: Fountain Applicants API
  slug: fountain-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-openapi.yml
- filename: fountain-com-openapi.yml
  format: yaml
  label: Fountain Openings API
  slug: fountain-openings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-openapi.yml
- filename: fountain-com-openapi.yml
  format: yaml
  label: Fountain Positions API
  slug: fountain-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-openapi.yml
- filename: fountain-com-openapi.yml
  format: yaml
  label: Fountain Stages API
  slug: fountain-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-openapi.yml
- filename: fountain-com-openapi.yml
  format: yaml
  label: Fountain Scheduling API
  slug: fountain-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-openapi.yml
- filename: fountain-com-openapi.yml
  format: yaml
  label: Fountain Labels API
  slug: fountain-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-openapi.yml
- filename: fountain-com-openapi.yml
  format: yaml
  label: Fountain Documents API
  slug: fountain-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-openapi.yml
- filename: fountain-com-openapi.yml
  format: yaml
  label: Fountain Webhooks API
  slug: fountain-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-openapi.yml
- filename: fountain-com-openapi.yml
  format: yaml
  label: Fountain Workers API
  slug: fountain-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-openapi.yml
consequence_counts:
  read: 18
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fountain Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 44
overview: 'Fountain exposes 44 API operations that an AI agent could call, of which 26 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 26 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fountain
provider_slug: fountain-com
slug: fountain-com-agentic-access
source_filename: fountain-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fountain-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 18\n    acting: 26\n  by_consequence:\n    read: 18\n    write: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /applicants\n  method: get\n  operationId: listApplicants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants\n  method: post\n  operationId: createApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{id}\n  method: get\n  operationId: getApplicant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/{id}\n  method: put\n  operationId: updateApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{id}\n  method: delete\n  operationId: deleteApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /applicants/{id}/advance\n  method: put\n  operationId: advanceApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/advance\n  method: post\n  operationId: bulkAdvanceApplicants\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{id}/transitions\n  method: get\n  operationId: getApplicantTransitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/notify\n \
  \ method: post\n  operationId: notifyApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{id}/duplicates\n  method: get\n  operationId: getDuplicateApplicants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funnels\n  method: get\n  operationId: listOpenings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funnels\n  method: post\n  operationId: createOpening\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /funnels/{id}\n  method: get\n  operationId: getOpening\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funnels/{id}\n  method: put\n  operationId: updateOpening\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /funnels/{id}\n  method: delete\n  operationId: deleteOpening\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /funnels/{funnel_id}/stages\n  method: get\n  operationId: listOpeningStages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positions\n  method: get\n  operationId: listPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /positions\n  method: post\n  operationId: createPosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /positions/{id}\n  method: get\n  operationId: getPosition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /positions/{id}\n  method: put\n  operationId: updatePosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /positions/{id}\n  method: delete\n  operationId: deletePosition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /stages/{id}\n  method: get\n  operationId: getStage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stages/{id}/available-slots\n  method: get\n  operationId: listStageAvailableSlots\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stages/{stage_id}/labels\n  method: get\n  operationId: listStageLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/{id}/labels\n  method: get\n  operationId: listApplicantLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applicants/{id}/labels/{title}\n  method: put\n  operationId: updateApplicantLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /available-slots\n\
  \  method: post\n  operationId: createAvailableSlots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /available-slots/{id}\n  method: patch\n  operationId: updateAvailableSlot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /available-slots/{id}\n  method: delete\n  operationId: deleteAvailableSlot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /available-slots/{id}/confirm\n  method: post\n  operationId: bookAvailableSlot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /booked-slots/{id}/cancel\n  method: post\n  operationId: cancelBookedSlot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{id}/secure-documents\n  method: get\n  operationId: getApplicantFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /applicants/{id}/secure-documents-upload\n  method: post\n  operationId: uploadApplicantFileToS3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{id}/secure-documents-link-upload\n  method: post\n  operationId: linkApplicantS3Files\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applicants/{id}/secure-documents-approve\n  method: post\n  operationId: approveApplicantDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-settings\n  method: get\n  operationId: listWebhookSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook-settings\n  method: post\n  operationId: createWebhookSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook-settings/{id}\n  method: get\n  operationId: getWebhookSetting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook-settings/{id}\n\
  \  method: delete\n  operationId: deleteWebhookSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers\n  method: get\n  operationId: listWorkers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{id}\n  method: get\n  operationId: getWorker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{id}\n  method: patch\n  operationId: updateWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{id}/activate\n  method: post\n  operationId: activateWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{id}/deactivate\n  method: post\n  operationId: deactivateWorker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/agentic-access/fountain-com-agentic-access.yml
summary_line: 44 operations · 26 acting
tags:
- Hiring
- Recruiting
- Applicant Tracking
- Frontline Hiring
- Hourly Workforce
- HR Tech
- Onboarding
---
