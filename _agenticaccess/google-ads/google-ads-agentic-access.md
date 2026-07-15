---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 2
api_specs:
- filename: google-ads-api-openapi.yml
  format: yaml
  label: Google Ads API
  slug: google-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-api-openapi.yml
consequence_counts:
  read: 2
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Ads Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Google Ads exposes 10 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Ads
provider_slug: google-ads
slug: google-ads-agentic-access
source_filename: google-ads-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-ads-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 8\n    connected: 2\n  by_consequence:\n    write: 8\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v18/customers/{customerId}/googleAds:search\n  method: post\n  operationId: searchGoogleAds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v18/customers/{customerId}/googleAds:searchStream\n  method: post\n  operationId:\
  \ searchStreamGoogleAds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v18/customers/{customerId}/campaigns:mutate\n  method: post\n  operationId: mutateCampaigns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v18/customers/{customerId}/adGroups:mutate\n  method: post\n  operationId: mutateAdGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v18/customers/{customerId}/adGroupAds:mutate\n  method: post\n  operationId: mutateAdGroupAds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v18/customers/{customerId}/adGroupCriteria:mutate\n  method: post\n  operationId: mutateAdGroupCriteria\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v18/customers/{customerId}/campaignBudgets:mutate\n  method: post\n  operationId: mutateCampaignBudgets\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v18/customers/{customerId}/biddingStrategies:mutate\n  method: post\n  operationId: mutateBiddingStrategies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v18/customers/{customerId}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v18/customers:listAccessibleCustomers\n  method: get\n  operationId: listAccessibleCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/agentic-access/google-ads-agentic-access.yml
summary_line: 10 operations · 8 acting
tags:
- Advertising
- Campaign Management
- Digital Advertising
- Google
- Marketing
- PPC
---
