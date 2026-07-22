---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 5
api_specs:
- filename: localytics-campaigns-audiences-openapi.yml
  format: yaml
  label: Localytics Campaigns And Audience API
  slug: localytics-campaigns-and-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localytics/refs/heads/main/openapi/localytics-campaigns-audiences-openapi.yml
consequence_counts:
  read: 5
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Localytics Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Localytics exposes 13 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Localytics
provider_slug: localytics
slug: localytics-agentic-access
source_filename: localytics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/localytics-campaigns-audiences-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 8\n    connected: 5\n  by_consequence:\n    write: 8\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /orgs/{org_id}/apps/{app_id}/push/campaigns\n  method: post\n  operationId: CreatePushCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/{app_id}/push/campaigns/{campaign_id}\n  method:\
  \ get\n  operationId: GetPushCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/apps/{app_id}/push/campaigns/{campaign_id}\n  method: delete\n  operationId: DeletePushCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/{app_id}/push/campaigns/{campaign_id}\n  method: put\n  operationId: editPushCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/{app_id}/push/campaigns/{campaign_id}/archive\n\
  \  method: put\n  operationId: ArchivePushCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/{app_id}/audiences\n  method: post\n  operationId: createAudiences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/{app_id}/audiences\n  method: get\n  operationId: ListAudiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/apps/{app_id}/audiences/{audience_id}/segmentation\n\
  \  method: post\n  operationId: AudienceSegmentation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/{app_id}/audiences/{audience_id}\n  method: get\n  operationId: GetAudienceSegmentationCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/apps/{app_id}/audiences/{audience_id}\n  method: patch\n  operationId: editAudiences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/{app_id}/audiences/{audience_id}\n\
  \  method: delete\n  operationId: DeleteAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_id}/apps/{app_id}/campaigns\n  method: get\n  operationId: ListCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_id}/apps/{app_id}/campaigns/search\n  method: get\n  operationId: SearchCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localytics/refs/heads/main/agentic-access/localytics-agentic-access.yml
summary_line: 13 operations · 8 acting
tags:
- Company
- Martech
- Mobile Analytics
- Push Notifications
- Customer Engagement
- Marketing Automation
- APIs
---
