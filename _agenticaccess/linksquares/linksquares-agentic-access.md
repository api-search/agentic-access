---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 12
api_specs:
- filename: linksquares-openapi.yml
  format: yaml
  label: LinkSquares Analyze Agreements API
  slug: linksquares-analyze-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linksquares/refs/heads/main/openapi/linksquares-openapi.yml
- filename: linksquares-openapi.yml
  format: yaml
  label: LinkSquares Analyze Metadata and Smart Values API
  slug: linksquares-analyze-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linksquares/refs/heads/main/openapi/linksquares-openapi.yml
- filename: linksquares-openapi.yml
  format: yaml
  label: LinkSquares Finalize Workflow API
  slug: linksquares-finalize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linksquares/refs/heads/main/openapi/linksquares-openapi.yml
consequence_counts:
  read: 12
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Linksquares Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'LinkSquares exposes 18 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LinkSquares
provider_slug: linksquares
slug: linksquares-agentic-access
source_filename: linksquares-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/linksquares-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 12\n    acting: 6\n  by_consequence:\n    read: 12\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/analyze/v1/me\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/analyze/v1/agreements\n  method: get\n  operationId: listAgreements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/analyze/v1/agreements\n\
  \  method: post\n  operationId: createAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analyze/v1/agreements/{agreement_id}\n  method: get\n  operationId: getAgreement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/analyze/v2/agreements/{agreement_id}\n  method: patch\n  operationId: updateAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analyze/v1/agreements/{agreement_id}/hierarchy\n\
  \  method: get\n  operationId: getAgreementHierarchy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/analyze/v1/agreements/{agreement_id}/terms\n  method: get\n  operationId: getAgreementTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/analyze/v2/agreements/{agreement_id}/terms/{term_id}\n  method: patch\n  operationId: updateAgreementTerm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analyze/v1/agreement_types\n  method: get\n  operationId: listAgreementTypes\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/analyze/v1/agreements/{agreement_id}/attachments\n  method: post\n  operationId: addAgreementAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/analyze/v2/agreements/{agreement_id}/attachments\n  method: get\n  operationId: listAgreementAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/analyze/v2/agreements/{agreement_id}/attachments/{attachment_id}/download\n  method: get\n  operationId: downloadAgreementAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /api/analyze/v1/uploads/{upload_id}\n  method: get\n  operationId: getUpload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/finalize/v1/templates\n  method: get\n  operationId: listFinalizeTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/finalize/v1/tasks\n  method: get\n  operationId: listFinalizeTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/finalize/v1/tasks/{task_id}\n  method: get\n  operationId: getFinalizeTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/finalize/v1/tasks/{task_id}\n\
  \  method: patch\n  operationId: approveFinalizeTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/finalize/v1/agreements\n  method: post\n  operationId: createFinalizeAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linksquares/refs/heads/main/agentic-access/linksquares-agentic-access.yml
summary_line: 18 operations · 6 acting
tags:
- Contract Management
- Contract Lifecycle Management
- CLM
- Contracts
- AI
- Legal
- Agreements
- Document Management
- Contract Analytics
---
