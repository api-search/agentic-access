---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: facebook-lead-ads-openapi.yml
  format: yaml
  label: Meta Marketing API - Lead Ads
  slug: graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-openapi.yml
consequence_counts:
  read: 6
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Facebook Lead Ads Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Facebook Lead Ads exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Facebook Lead Ads
provider_slug: facebook-lead-ads
slug: facebook-lead-ads-agentic-access
source_filename: facebook-lead-ads-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/facebook-lead-ads-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 6\n    acting: 3\n  by_consequence:\n    read: 6\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /{page-id}/leadgen_forms\n  method: get\n  operationId: listLeadGenForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - leads_retrieval\n    - pages_manage_ads\n    - pages_show_list\n- path: /{page-id}/leadgen_forms\n  method: post\n  operationId: createLeadGenForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - leads_retrieval\n    - pages_manage_ads\n    - pages_show_list\n- path: /{form-id}\n  method: get\n  operationId: getLeadGenForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - leads_retrieval\n    - pages_manage_ads\n    - pages_show_list\n- path: /{form-id}/leads\n  method: get\n  operationId: listLeadsForForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - leads_retrieval\n    - pages_manage_ads\n    - pages_show_list\n- path: /{lead-id}\n  method: get\n  operationId: getLead\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - leads_retrieval\n    - pages_manage_ads\n    - pages_show_list\n- path: /{ad-id}/leads\n  method: get\n  operationId: listLeadsForAd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - leads_retrieval\n    - pages_manage_ads\n    - pages_show_list\n- path: /{form-id}/bulk_leads\n  method: get\n  operationId: bulkDownloadLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - leads_retrieval\n    - pages_manage_ads\n    - pages_show_list\n- path: /{app-id}/subscriptions\n  method: post\n  operationId: subscribeAppWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - leads_retrieval\n    - pages_manage_ads\n    - pages_show_list\n- path: /{page-id}/subscribed_apps\n  method: post\n  operationId: pageSubscribedApps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - leads_retrieval\n    - pages_manage_ads\n    - pages_show_list\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/agentic-access/facebook-lead-ads-agentic-access.yml
summary_line: 9 operations · 3 acting
tags:
- Advertising
- Lead Generation
- Lead Ads
- Marketing API
- Facebook
- Instagram
- Meta
- Webhooks
---
