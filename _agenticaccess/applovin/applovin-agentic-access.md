---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 16
api_specs:
- filename: applovin-max-revenue-reporting.yaml
  format: yaml
  label: AppLovin MAX Revenue Reporting API
  slug: applovin-max-revenue-reporting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-max-revenue-reporting.yaml
- filename: applovin-max-ad-unit-management.yaml
  format: yaml
  label: AppLovin MAX Ad Unit Management API
  slug: applovin-max-ad-unit-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-max-ad-unit-management.yaml
- filename: applovin-growth-reporting.yaml
  format: yaml
  label: AppLovin Growth (Axon / AppDiscovery) Reporting API
  slug: applovin-growth-reporting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-growth-reporting.yaml
- filename: applovin-growth-asset-reporting.yaml
  format: yaml
  label: AppLovin Growth Asset Reporting API
  slug: applovin-growth-asset-reporting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-growth-asset-reporting.yaml
- filename: applovin-axon-campaign-management.yaml
  format: yaml
  label: AppLovin Axon Campaign Management API
  slug: applovin-axon-campaign-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-axon-campaign-management.yaml
- filename: applovin-conversion-api-lead-gen.yaml
  format: yaml
  label: AppLovin Conversion API for Lead Generation
  slug: applovin-conversion-api-lead-gen
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-conversion-api-lead-gen.yaml
consequence_counts:
  read: 16
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Applovin Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'AppLovin exposes 30 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AppLovin
provider_slug: applovin
slug: applovin-agentic-access
source_filename: applovin-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/applovin-axon-campaign-management.yaml, openapi/applovin-conversion-api-lead-gen.yaml,\n  openapi/applovin-growth-asset-reporting.yaml, openapi/applovin-growth-reporting.yaml, openapi/applovin-max-ad-unit-management.yaml,\n  openapi/applovin-max-revenue-reporting.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 16\n    acting: 14\n  by_consequence:\n    read: 16\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /campaign/list\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /campaign/create\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaign/update\n  method: post\n  operationId: updateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creative_set/list\n  method: get\n  operationId: listCreativeSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creative_set/list_by_campaign_id\n  method: get\n  operationId: listCreativeSetsByCampaignId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creative_set/create\n  method: post\n  operationId: createCreativeSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creative_set/update\n  method: post\n  operationId: updateCreativeSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creative_set/clone\n  method: post\n  operationId: cloneCreativeSet\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset/list\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asset/upload\n  method: post\n  operationId: uploadAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asset/upload_result\n  method: get\n  operationId: getAssetUploadResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/event\n  method: post\n  operationId: postConversionEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assetReport\n  method: get\n  operationId: getAssetReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assetAnalyticsReport\n  method: get\n  operationId: getAssetAnalyticsReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report\n  method: get\n  operationId: getGrowthReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /ad_units\n  method: get\n  operationId: listAdUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ad_unit\n  method: post\n  operationId: createAdUnit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ad_unit/{ad_unit_id}\n  method: get\n  operationId: getAdUnit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ad_unit/{ad_unit_id}\n  method: post\n  operationId: updateAdUnit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ad_unit/{ad_unit_id}/{segment_id}\n  method: get\n  operationId: getAdUnitWaterfall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ad_unit/{ad_unit_id}/{segment_id}\n  method: post\n  operationId: updateAdUnitWaterfall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ad_unit_experiment/{ad_unit_id}\n  method: get\n  operationId: getAdUnitExperiment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ad_unit_experiment/{ad_unit_id}\n\
  \  method: post\n  operationId: upsertAdUnitExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ad_unit_experiment/{ad_unit_id}/{segment_id}\n  method: get\n  operationId: getAdUnitExperimentWaterfall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ad_unit_experiment/{ad_unit_id}/{segment_id}\n  method: post\n  operationId: updateAdUnitExperimentWaterfall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /test_devices\n\
  \  method: get\n  operationId: listTestDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /test_device\n  method: post\n  operationId: createTestDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /test_device/{test_device_id}\n  method: get\n  operationId: getTestDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /test_device/{test_device_id}\n  method: post\n  operationId: updateTestDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /maxReport\n  method: get\n  operationId: getMaxRevenueReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/agentic-access/applovin-agentic-access.yml
summary_line: 30 operations · 14 acting
tags:
- Advertising
- Mobile
- AdTech
- App Monetization
- Mediation
- User Acquisition
- Marketing Technology
- Conversion Tracking
---
