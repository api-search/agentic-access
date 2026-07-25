---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 10
api_specs:
- filename: agorapulse-calendar-notes-api-openapi.yml
  format: yaml
  label: Agorapulse Calendar Notes API
  slug: agorapulse-calendar-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-calendar-notes-api-openapi.yml
- filename: agorapulse-inbox-conversations-api-openapi.yml
  format: yaml
  label: Agorapulse Inbox conversations API
  slug: agorapulse-inbox-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-inbox-conversations-api-openapi.yml
- filename: agorapulse-inbox-items-api-openapi.yml
  format: yaml
  label: Agorapulse Inbox items API
  slug: agorapulse-inbox-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-inbox-items-api-openapi.yml
- filename: agorapulse-inbox-reply-api-openapi.yml
  format: yaml
  label: Agorapulse Inbox reply API
  slug: agorapulse-inbox-reply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-inbox-reply-api-openapi.yml
- filename: agorapulse-openapi-api-openapi.yml
  format: yaml
  label: Agorapulse OpenAPI API
  slug: agorapulse-openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-openapi-api-openapi.yml
- filename: agorapulse-organization-api-openapi.yml
  format: yaml
  label: Agorapulse Organization API
  slug: agorapulse-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-organization-api-openapi.yml
- filename: agorapulse-profile-api-openapi.yml
  format: yaml
  label: Agorapulse Profile API
  slug: agorapulse-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-profile-api-openapi.yml
- filename: agorapulse-report-api-openapi.yml
  format: yaml
  label: Agorapulse Report API
  slug: agorapulse-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-report-api-openapi.yml
- filename: agorapulse-simple-drafts-api-openapi.yml
  format: yaml
  label: Agorapulse Simple Drafts API
  slug: agorapulse-simple-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-simple-drafts-api-openapi.yml
- filename: agorapulse-simple-scheduling-api-openapi.yml
  format: yaml
  label: Agorapulse Simple Scheduling API
  slug: agorapulse-simple-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-simple-scheduling-api-openapi.yml
- filename: agorapulse-studio-media-api-openapi.yml
  format: yaml
  label: Agorapulse Studio Media API
  slug: agorapulse-studio-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-studio-media-api-openapi.yml
- filename: agorapulse-workspace-api-openapi.yml
  format: yaml
  label: Agorapulse Workspace API
  slug: agorapulse-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-workspace-api-openapi.yml
consequence_counts:
  read: 10
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agorapulse Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Agorapulse exposes 18 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agorapulse
provider_slug: agorapulse
slug: agorapulse-agentic-access
source_filename: agorapulse-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/agorapulse-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 10\n    acting: 8\n  by_consequence:\n    read: 10\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1.0/report/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/report/organizations/{organizationId}/workspaces/{workspaceId}/profiles/{profileUid}/insights/audience\n  method: get\n  operationId: getAudience\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/report/organizations/{organizationId}/workspaces/{workspaceId}/profiles/{profileUid}/insights/communitymanagement\n  method: get\n  operationId: getCommunityManagement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/report/organizations/{organizationId}/workspaces/{workspaceId}/profiles/{profileUid}/insights/content\n  method: get\n  operationId: getContentReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/core/organizations\n  method: get\n  operationId: getManagerOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/core/organizations/{organizationId}/workspaces\n  method: get\n\
  \  operationId: getOrganizationWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/core/organizations/{organizationId}/workspaces/{workspaceId}/profiles\n  method: get\n  operationId: getWorkspaceProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/publishing/organizations/{organizationId}/workspaces/{workspaceId}/notes\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/publishing/organizations/{organizationId}/workspaces/{workspaceId}/notes\n  method: post\n  operationId: save\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/publishing/organizations/{organizationId}/workspaces/{workspaceId}/notes/{uid}\n  method: put\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/publishing/organizations/{organizationId}/workspaces/{workspaceId}/notes/{uid}\n  method: delete\n  operationId: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/publishing/organizations/{organizationId}/workspaces/{workspaceId}/simple-drafts\n\
  \  method: post\n  operationId: save_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/publishing/organizations/{organizationId}/workspaces/{workspaceId}/simple-schedule-posts\n  method: post\n  operationId: save_2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/publishing/organizations/{organizationId}/workspaces/{workspaceId}/simple-schedule-posts:publish-now\n  method: post\n  operationId: publishNow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/library/organizations/{organizationId}/workspaces/{workspaceId}/studio/media/upload\n  method: post\n  operationId: requestUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/inbox/organizations/{organizationId}/workspaces/{workspaceId}/accounts/{accountUid}/conversations/{conversationId}/messages\n  method: get\n  operationId: getMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/inbox/organizations/{organizationId}/workspaces/{workspaceId}/accounts/{accountUid}/reply\n\
  \  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/inbox/organizations/{organizationId}/workspaces/{workspaceId}/items\n  method: get\n  operationId: findItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/agentic-access/agorapulse-agentic-access.yml
summary_line: 18 operations · 8 acting
tags:
- Social Media Management
- Social Media
- CRM
- Analytics
- Publishing
- Inbox Management
- Social Listening
---
