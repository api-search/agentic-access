---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: microsoft-linkedin-openapi.yml
  format: yaml
  label: LinkedIn Marketing API
  slug: marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/openapi/microsoft-linkedin-openapi.yml
consequence_counts:
  read: 9
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Linkedin Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Microsoft LinkedIn exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft LinkedIn
provider_slug: microsoft-linkedin
slug: microsoft-linkedin-agentic-access
source_filename: microsoft-linkedin-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-linkedin-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 9\n    acting: 8\n  by_consequence:\n    read: 9\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /rest/adAccounts\n  method: get\n  operationId: adAccounts_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rw_ads\n- path: /rest/adAccounts\n  method: post\n  operationId: adAccounts_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}\n  method: get\n  operationId: adAccounts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}\n  method: post\n  operationId: adAccounts_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}\n  method: delete\n  operationId: adAccounts_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}/adCampaignGroups\n  method: get\n  operationId: adCampaignGroups_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}/adCampaignGroups\n  method: post\n  operationId: adCampaignGroups_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}/adCampaignGroups/{campaignGroupID}\n  method: get\n\
  \  operationId: adCampaignGroups_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}/adCampaignGroups/{campaignGroupID}\n  method: post\n  operationId: adCampaignGroups_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}/adCampaigns\n  method: get\n  operationId: adCampaigns_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}/adCampaigns\n  method: post\n  operationId:\
  \ adCampaigns_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}/adCampaigns/{adCampaignID}\n  method: get\n  operationId: adCampaigns_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}/adCampaigns/{adCampaignID}\n  method: post\n  operationId: adCampaigns_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  \    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}/adCreatives\n  method: get\n  operationId: adCreatives_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}/adCreatives\n  method: post\n  operationId: adCreatives_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - rw_ads\n- path: /rest/adAccounts/{adAccountID}/adCreatives/{adCreativeID}\n  method: get\n  operationId: adCreatives_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rw_ads\n- path:\
  \ /rest/adAccountUsers\n  method: get\n  operationId: adAccountUsers_find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rw_ads\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-linkedin/refs/heads/main/agentic-access/microsoft-linkedin-agentic-access.yml
summary_line: 17 operations · 8 acting
tags:
- Marketing
- Microsoft
- Professional Networking
- Recruiting
- Social Network
---
