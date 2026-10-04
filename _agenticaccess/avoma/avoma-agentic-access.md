---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 36
api_specs:
- filename: avoma-calls-api-openapi.yml
  format: yaml
  label: Avoma Calls API
  slug: avoma-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-calls-api-openapi.yml
- filename: avoma-custom-category-api-openapi.yml
  format: yaml
  label: Avoma Custom Category API
  slug: avoma-custom-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-custom-category-api-openapi.yml
- filename: avoma-engagement-analytics-api-openapi.yml
  format: yaml
  label: Avoma Engagement Analytics API
  slug: avoma-engagement-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-engagement-analytics-api-openapi.yml
- filename: avoma-meeting-outcomes-api-openapi.yml
  format: yaml
  label: Avoma Meeting Outcomes API
  slug: avoma-meeting-outcomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-meeting-outcomes-api-openapi.yml
- filename: avoma-meeting-types-api-openapi.yml
  format: yaml
  label: Avoma Meeting Types API
  slug: avoma-meeting-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-meeting-types-api-openapi.yml
- filename: avoma-meetings-api-openapi.yml
  format: yaml
  label: Avoma Meetings API
  slug: avoma-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-meetings-api-openapi.yml
- filename: avoma-meetings-sentiments-api-openapi.yml
  format: yaml
  label: Avoma Meetings Sentiments API
  slug: avoma-meetings-sentiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-meetings-sentiments-api-openapi.yml
- filename: avoma-notes-api-openapi.yml
  format: yaml
  label: Avoma Notes API
  slug: avoma-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-notes-api-openapi.yml
- filename: avoma-recording-api-openapi.yml
  format: yaml
  label: Avoma Recording API
  slug: avoma-recording-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-recording-api-openapi.yml
- filename: avoma-revenue-intelligence-beta-api-openapi.yml
  format: yaml
  label: Avoma Revenue Intelligence [Beta] API
  slug: avoma-revenue-intelligence-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-revenue-intelligence-beta-api-openapi.yml
- filename: avoma-scorecard-evaluations-api-openapi.yml
  format: yaml
  label: Avoma Scorecard Evaluations API
  slug: avoma-scorecard-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-scorecard-evaluations-api-openapi.yml
- filename: avoma-scorecards-api-openapi.yml
  format: yaml
  label: Avoma Scorecards API
  slug: avoma-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-scorecards-api-openapi.yml
- filename: avoma-smart-category-api-openapi.yml
  format: yaml
  label: Avoma Smart Category API
  slug: avoma-smart-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-smart-category-api-openapi.yml
- filename: avoma-snippets-api-openapi.yml
  format: yaml
  label: Avoma Snippets API
  slug: avoma-snippets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-snippets-api-openapi.yml
- filename: avoma-templates-api-openapi.yml
  format: yaml
  label: Avoma Templates API
  slug: avoma-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-templates-api-openapi.yml
- filename: avoma-transcriptions-api-openapi.yml
  format: yaml
  label: Avoma Transcriptions API
  slug: avoma-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-transcriptions-api-openapi.yml
- filename: avoma-users-api-openapi.yml
  format: yaml
  label: Avoma Users API
  slug: avoma-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-users-api-openapi.yml
- filename: avoma-webhooks-api-openapi.yml
  format: yaml
  label: Avoma Webhooks API
  slug: avoma-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-webhooks-api-openapi.yml
consequence_counts:
  read: 36
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Avoma Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 59
overview: 'Avoma exposes 59 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 read and 23 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Avoma
provider_slug: avoma
slug: avoma-agentic-access
source_filename: avoma-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: generated\nsource: openapi/avoma-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 59\n  by_action_class:\n    connected: 36\n    acting: 23\n  by_consequence:\n    read: 36\n    write: 23\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/calls/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calls/\n  method: post\n  operationId: createExtCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v1/calls/{external_id}/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calls/{external_id}/\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/custom_categories/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/custom_categories/{uuid}/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meeting_segments/\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meeting_sentiments/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meetings/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meetings/{meeting_uuid}/insights/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meetings/{uuid}/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meetings/{uuid}/drop/\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notes/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recordings/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recordings/{uuid}/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scorecard_evaluations/\n  method: get\n  operationId: scorecard_evaluations_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scorecards/\n  method: get\n  operationId: scorecards_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scorecards/{uuid}/\n  method: get\n  operationId: scorecards_retrieve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/smart_categories/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/smart_categories/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/smart_categories/{uuid}/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/smart_categories/{uuid}/\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/template/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/template/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/template/{uuid}/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/template/{uuid}/\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transcriptions/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcriptions/{uuid}/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meeting_type/\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meeting_type/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/meeting_type/{uuid}/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meeting_type/{uuid}/\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/meeting_type/{uuid}/\n\
  \  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/meeting_outcome/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meeting_outcome/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/meeting_outcome/{uuid}/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/meeting_outcome/{uuid}/\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/meeting_outcome/{uuid}/\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{uuid}/\n  method: get\n  operationId: Get User\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/engagement/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/engagement/{user_uuid}/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/engagement/summary/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/engagement/{user_uuid}/summary/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/snippets/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: v1/revenue_intel/timeline/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/revenue_intel/timeline_details/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/ainote/\n\
  \  method: post\n  operationId: webhookEventAinote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/meeting_booked_via_scheduler/\n  method: post\n  operationId: webhookEventMeetingBookedViaScheduler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/meeting_booked_via_scheduler_canceled/\n  method: post\n  operationId: webhookEventMeetingBookedViaSchedulerCanceled\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/meeting_booked_via_scheduler_rescheduled/\n  method: post\n  operationId: webhookEventMeetingBookedViaSchedulerRescheduled\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/new_conversation/\n  method: post\n  operationId: webhookEventNewConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/signing-secret/\n  method: delete\n  operationId:\
  \ clearWebhookSigningSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/signing-secret/\n  method: get\n  operationId: getWebhookSigningSecret\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/signing-secret/\n  method: patch\n  operationId: setWebhookSigningSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/signing-secret/rotate/\n  method: post\n  operationId: rotateWebhookSigningSecret\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{uuid}/\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/agentic-access/avoma-agentic-access.yml
summary_line: 59 operations · 23 acting
tags:
- Artificial Intelligence
- Meeting Assistant
- Sales Enablement
- Automation
- Productivity
---
