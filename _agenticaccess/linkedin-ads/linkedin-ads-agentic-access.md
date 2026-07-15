---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: linkedin-ads-openapi.yml
  format: yaml
  label: LinkedIn Marketing API
  slug: marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-openapi.yml
consequence_counts:
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Linkedin Ads Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'LinkedIn Marketing API exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LinkedIn Marketing API
provider_slug: linkedin-ads
slug: linkedin-ads-agentic-access
source_filename: linkedin-ads-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/linkedin-ads-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 4\n    connected: 5\n  by_consequence:\n    write: 4\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /adAccounts\n  method: post\n  operationId: createAdAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - rw_ads\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adAccounts/{adAccountId}\n  method: get\n  operationId: getAdAccount\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_ads\n    - rw_ads\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adAccounts/{adAccountId}/adCampaignGroups\n  method: post\n  operationId: createAdCampaignGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - rw_ads\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adAccounts/{adAccountId}/adCampaigns\n  method: post\n  operationId: createAdCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - rw_ads\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adAccounts/{adAccountId}/creatives\n\
  \  method: post\n  operationId: createCreative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - rw_ads\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adTargetingFacets\n  method: get\n  operationId: listAdTargetingFacets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_ads\n    - rw_ads\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adTargetingEntities\n  method: get\n  operationId: getAdTargetingEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_ads\n    - rw_ads\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audienceCounts\n  method: get\n  operationId: getAudienceCounts\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - r_ads\n    - rw_ads\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adBudgetPricing\n  method: get\n  operationId: getAdBudgetPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - r_ads\n    - rw_ads\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/agentic-access/linkedin-ads-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Advertising
- Marketing
- LinkedIn
- Lead Generation
- Audience Targeting
- Conversions API
- Social Marketing
---
