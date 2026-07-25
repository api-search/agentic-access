---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 16
api_specs:
- filename: kevel-ads-api-openapi.yml
  format: yaml
  label: Kevel Ads API
  slug: kevel-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-ads-api-openapi.yml
- filename: kevel-advertisers-api-openapi.yml
  format: yaml
  label: Kevel Advertisers API
  slug: kevel-advertisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-advertisers-api-openapi.yml
- filename: kevel-campaigns-api-openapi.yml
  format: yaml
  label: Kevel Campaigns API
  slug: kevel-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-campaigns-api-openapi.yml
- filename: kevel-channels-api-openapi.yml
  format: yaml
  label: Kevel Channels API
  slug: kevel-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-channels-api-openapi.yml
- filename: kevel-creatives-api-openapi.yml
  format: yaml
  label: Kevel Creatives API
  slug: kevel-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-creatives-api-openapi.yml
- filename: kevel-decision-api-openapi.yml
  format: yaml
  label: Kevel Decision API
  slug: kevel-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-decision-api-openapi.yml
- filename: kevel-flights-api-openapi.yml
  format: yaml
  label: Kevel Flights API
  slug: kevel-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-flights-api-openapi.yml
- filename: kevel-reporting-api-openapi.yml
  format: yaml
  label: Kevel Reporting API
  slug: kevel-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-reporting-api-openapi.yml
- filename: kevel-sites-api-openapi.yml
  format: yaml
  label: Kevel Sites API
  slug: kevel-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-sites-api-openapi.yml
- filename: kevel-zones-api-openapi.yml
  format: yaml
  label: Kevel Zones API
  slug: kevel-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-zones-api-openapi.yml
consequence_counts:
  read: 16
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kevel Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 33
overview: 'Kevel exposes 33 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kevel
provider_slug: kevel
slug: kevel-agentic-access
source_filename: kevel-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kevel-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    acting: 17\n    connected: 16\n  by_consequence:\n    write: 17\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2\n  method: post\n  operationId: makeDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /advertiser\n  method: get\n  operationId: listAdvertisers\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /advertiser\n  method: post\n  operationId: createAdvertiser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /advertiser/{id}\n  method: get\n  operationId: getAdvertiser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /advertiser/{id}\n  method: put\n  operationId: updateAdvertiser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /advertiser/{id}\n  method: delete\n  operationId: deleteAdvertiser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaign\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaign\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaign/{id}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaign/{id}\n  method: put\n  operationId: updateCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /flight\n  method: get\n  operationId: listFlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flight\n  method: post\n  operationId: createFlight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /flight/{id}\n  method: get\n  operationId: getFlight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /flight/{id}\n  method: put\n  operationId: updateFlight\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ad\n  method: get\n  operationId: listAds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ad\n  method: post\n  operationId: createAd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ad/{id}\n  method: get\n  operationId: getAd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ad/{id}\n  method: put\n  operationId: updateAd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creative\n  method: get\n  operationId: listCreatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creative\n  method: post\n  operationId: createCreative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creative/{id}\n  method: get\n  operationId: getCreative\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /creative/{id}\n  method: put\n  operationId: updateCreative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /site\n  method: get\n  operationId: listSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site\n  method: post\n  operationId: createSite\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /site/{id}\n  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /site/{id}\n  method: put\n  operationId: updateSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /zone\n  method: get\n  operationId: listZones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /zone/{id}\n  method: get\n  operationId: getZone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zone/{id}\n  method: put\n  operationId: updateZone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channel\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channel\n  method: post\n  operationId: createChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /report/queue\n  method: post\n  operationId: queueReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /report/{reportId}\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/agentic-access/kevel-agentic-access.yml
summary_line: 33 operations · 17 acting
tags:
- Ad Serving
- Advertising
- API-First
- Audience
- Monetization
- Reporting
---
