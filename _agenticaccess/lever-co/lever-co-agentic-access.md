---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 29
api_specs:
- filename: lever-webhooks-asyncapi.yml
  format: yaml
  label: Lever Webhooks
  slug: lever-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-webhooks-asyncapi.yml
- filename: lever-co-applications-api-openapi.yml
  format: yaml
  label: Lever Applications API
  slug: lever-co-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-applications-api-openapi.yml
- filename: lever-co-archive-reasons-api-openapi.yml
  format: yaml
  label: Lever Archive Reasons API
  slug: lever-co-archive-reasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-archive-reasons-api-openapi.yml
- filename: lever-co-audit-events-api-openapi.yml
  format: yaml
  label: Lever Audit Events API
  slug: lever-co-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-audit-events-api-openapi.yml
- filename: lever-co-eeo-responses-api-openapi.yml
  format: yaml
  label: Lever EEO Responses API
  slug: lever-co-eeo-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-eeo-responses-api-openapi.yml
- filename: lever-co-feedback-api-openapi.yml
  format: yaml
  label: Lever Feedback API
  slug: lever-co-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-feedback-api-openapi.yml
- filename: lever-co-files-api-openapi.yml
  format: yaml
  label: Lever Files API
  slug: lever-co-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-files-api-openapi.yml
- filename: lever-co-interviews-api-openapi.yml
  format: yaml
  label: Lever Interviews API
  slug: lever-co-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-interviews-api-openapi.yml
- filename: lever-co-notes-api-openapi.yml
  format: yaml
  label: Lever Notes API
  slug: lever-co-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-notes-api-openapi.yml
- filename: lever-co-offers-api-openapi.yml
  format: yaml
  label: Lever Offers API
  slug: lever-co-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-offers-api-openapi.yml
- filename: lever-co-opportunities-api-openapi.yml
  format: yaml
  label: Lever Opportunities API
  slug: lever-co-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-opportunities-api-openapi.yml
- filename: lever-co-panels-api-openapi.yml
  format: yaml
  label: Lever Panels API
  slug: lever-co-panels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-panels-api-openapi.yml
- filename: lever-co-postings-api-openapi.yml
  format: yaml
  label: Lever Postings API
  slug: lever-co-postings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-postings-api-openapi.yml
- filename: lever-co-requisitions-api-openapi.yml
  format: yaml
  label: Lever Requisitions API
  slug: lever-co-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-requisitions-api-openapi.yml
- filename: lever-co-sources-api-openapi.yml
  format: yaml
  label: Lever Sources API
  slug: lever-co-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-sources-api-openapi.yml
- filename: lever-co-stages-api-openapi.yml
  format: yaml
  label: Lever Stages API
  slug: lever-co-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-stages-api-openapi.yml
- filename: lever-co-tags-api-openapi.yml
  format: yaml
  label: Lever Tags API
  slug: lever-co-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-tags-api-openapi.yml
- filename: lever-co-users-api-openapi.yml
  format: yaml
  label: Lever Users API
  slug: lever-co-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-users-api-openapi.yml
- filename: lever-co-webhooks-api-openapi.yml
  format: yaml
  label: Lever Webhooks API
  slug: lever-co-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-co-webhooks-api-openapi.yml
consequence_counts:
  read: 29
  write: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lever Co Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 53
overview: 'Lever exposes 53 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read and 24 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lever
provider_slug: lever-co
slug: lever-co-agentic-access
source_filename: lever-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lever-data-api-openapi.yml, openapi/lever-postings-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    connected: 29\n    acting: 24\n  by_consequence:\n    read: 29\n    write: 24\n  human_in_the_loop_required: 0\noperations:\n- path: /opportunities\n  method: get\n  operationId: listOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities\n  method: post\n  operationId: createOpportunity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities/{id}\n  method: get\n  operationId: getOpportunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{id}\n  method: put\n  operationId: updateOpportunity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities/{id}/applications\n  method: get\n  operationId: listApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{id}/interviews\n\
  \  method: get\n  operationId: listInterviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{id}/interviews\n  method: post\n  operationId: createInterview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities/{id}/interviews/{interviewId}\n  method: put\n  operationId: updateInterview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities/{id}/interviews/{interviewId}\n  method:\
  \ delete\n  operationId: deleteInterview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities/{id}/feedback\n  method: get\n  operationId: listFeedback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{id}/feedback\n  method: post\n  operationId: createFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities/{id}/notes\n  method: get\n  operationId: listNotes\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{id}/notes\n  method: post\n  operationId: createNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /postings\n  method: get\n  operationId: listPostings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /postings\n  method: post\n  operationId: createPosting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /postings/{id}\n  method: get\n  operationId: getPosting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /postings/{id}\n  method: put\n  operationId: updatePosting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /requisitions\n  method: get\n  operationId: listRequisitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /requisitions\n  method: post\n  operationId: createRequisition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /requisitions/{id}\n  method: put\n  operationId: updateRequisition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /requisitions/{id}\n  method: delete\n  operationId: deleteRequisition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /offers\n  method: get\n  operationId: listOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stages\n  method: get\n  operationId: listStages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stages/{id}\n  method: get\n  operationId: getStage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /archive_reasons\n  method: get\n  operationId: listArchiveReasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /archive_reasons/{id}\n  method: get\n  operationId: getArchiveReason\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sources\n  method: get\n  operationId: listSources\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{id}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{id}\n  method: get\n  operationId:\
  \ getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method: put\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /panels\n  method: get\n  operationId: listPanels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /panels\n  method: post\n  operationId: createPanel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /panels/{id}\n  method: put\n  operationId: updatePanel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /panels/{id}\n  method: delete\n  operationId: deletePanel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{id}\n  method: put\n  operationId: updateContact\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referrals\n  method: get\n  operationId: listReferrals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eeo/responses\n  method: get\n  operationId: listEeoResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eeo/responses/pii\n  method: get\n  operationId: listEeoResponsesPii\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audit_events\n  method: get\n  operationId: listAuditEvents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{site}\n  method: get\n  operationId: listPublicPostings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{site}/{postingId}\n  method: get\n  operationId: getPublicPosting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{site}/{postingId}\n  method: post\n  operationId: submitApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/agentic-access/lever-co-agentic-access.yml
summary_line: 53 operations · 24 acting
tags:
- Applicant Tracking
- ATS
- CRM
- Recruiting
- Hiring
- Talent Acquisition
- Human Resources
- HR Tech
- Postings
- Webhook
- Authentication
---
