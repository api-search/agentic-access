---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 4
api_specs:
- filename: dynamic-yield-api-only-api-openapi.yml
  format: yaml
  label: Dynamic Yield API only API
  slug: dynamic-yield-api-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-api-only-api-openapi.yml
- filename: dynamic-yield-experience-apis-api-openapi.yml
  format: yaml
  label: Dynamic Yield Experience APIs API
  slug: dynamic-yield-experience-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-experience-apis-api-openapi.yml
- filename: dynamic-yield-product-data-api-openapi.yml
  format: yaml
  label: Dynamic Yield Product Data API
  slug: dynamic-yield-product-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-product-data-api-openapi.yml
- filename: dynamic-yield-profile-anywhere-api-openapi.yml
  format: yaml
  label: Dynamic Yield Profile Anywhere API
  slug: dynamic-yield-profile-anywhere-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-profile-anywhere-api-openapi.yml
- filename: dynamic-yield-user-data-api-api-openapi.yml
  format: yaml
  label: Dynamic Yield User Data API
  slug: dynamic-yield-user-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/openapi/dynamic-yield-user-data-api-api-openapi.yml
consequence_counts:
  read: 4
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dynamic Yield Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Dynamic Yield exposes 23 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dynamic Yield
provider_slug: dynamic-yield
slug: dynamic-yield-agentic-access
source_filename: dynamic-yield-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/dynamic-yield-experience-api-openapi.yml, openapi/dynamic-yield-experience-apis-for-api-sections-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 19\n    connected: 4\n  by_consequence:\n    write: 19\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /collect/user/engagement\n  method: post\n  operationId: trackEngagement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/user/event\n\
  \  method: post\n  operationId: trackEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/user/pageview\n  method: post\n  operationId: trackPageviews\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/add-ons\n  method: post\n  operationId: updateAddOnsFeed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /feeds/branch/outage/bulk\n  method: post\n  operationId: reportOutages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/branch/{id}/inventory\n  method: post\n  operationId: updateBranchFeed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/{feedId}/bulk\n  method: post\n  operationId: updateProductFeed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feeds/{feedId}/transaction/{transactionId}\n  method: get\n  operationId: trackTransactionStatusWholeTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/{feedId}/transaction/{transactionId}/item/{itemId}\n  method: get\n  operationId: trackTransactionStatusSpecificItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serve/user/agent\n  method: post\n  operationId: shoppingMuse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /serve/user/browse\n\
  \  method: post\n  operationId: browse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /serve/user/choose\n  method: post\n  operationId: chooseVariations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /serve/user/search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serve/user/suggest\n  method: post\n  operationId: suggest\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userdata/channels/{channel}/opt-in\n  method: post\n  operationId: updateReconnectOptIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userdata/channels/{channel}/opt-out\n  method: post\n  operationId: updateReconnectOptOut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userdata/events\n\
  \  method: post\n  operationId: externalEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userdata/{feedKey}/bulk\n  method: post\n  operationId: userDataApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /userprofile\n  method: get\n  operationId: profileAnywhere\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collect/user/engagement (API only)\n  method: post\n  operationId: reporting-engagement-2\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/user/event (API only)\n  method: post\n  operationId: reporting-events-api-only\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/user/pageview (API only)\n  method: post\n  operationId: reporting-pageviews-api-only\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /serve/user/choose (API only)\n  method: post\n  operationId: choosing-variations-api-only\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamic-yield/refs/heads/main/agentic-access/dynamic-yield-agentic-access.yml
summary_line: 23 operations · 19 acting
tags:
- Company
- Cloud
- Personalization
- Experience Optimization
- Recommendations
- A/B Testing
- Search
- E-Commerce
- Retail
- Machine Learning
- MACH
- Mastercard
---
