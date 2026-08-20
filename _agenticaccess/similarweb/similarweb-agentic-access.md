---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 19
api_specs:
- filename: similarweb-account-api-openapi.yml
  format: yaml
  label: SimilarWeb Account API
  slug: similarweb-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-account-api-openapi.yml
- filename: similarweb-app-intelligence-api-openapi.yml
  format: yaml
  label: SimilarWeb App Intelligence API
  slug: similarweb-app-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-app-intelligence-api-openapi.yml
- filename: similarweb-credits-api-openapi.yml
  format: yaml
  label: SimilarWeb Credits API
  slug: similarweb-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-credits-api-openapi.yml
- filename: similarweb-geography-api-openapi.yml
  format: yaml
  label: SimilarWeb Geography API
  slug: similarweb-geography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-geography-api-openapi.yml
- filename: similarweb-integrations-api-openapi.yml
  format: yaml
  label: SimilarWeb Integrations API
  slug: similarweb-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-integrations-api-openapi.yml
- filename: similarweb-keywords-api-openapi.yml
  format: yaml
  label: SimilarWeb Keywords API
  slug: similarweb-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-keywords-api-openapi.yml
- filename: similarweb-lead-enrichment-api-openapi.yml
  format: yaml
  label: SimilarWeb Lead Enrichment API
  slug: similarweb-lead-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-lead-enrichment-api-openapi.yml
- filename: similarweb-rankings-api-openapi.yml
  format: yaml
  label: SimilarWeb Rankings API
  slug: similarweb-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-rankings-api-openapi.yml
- filename: similarweb-reports-api-openapi.yml
  format: yaml
  label: SimilarWeb Reports API
  slug: similarweb-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-reports-api-openapi.yml
- filename: similarweb-similar-sites-api-openapi.yml
  format: yaml
  label: SimilarWeb Similar Sites API
  slug: similarweb-similar-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-similar-sites-api-openapi.yml
- filename: similarweb-traffic-and-engagement-api-openapi.yml
  format: yaml
  label: SimilarWeb Traffic and Engagement API
  slug: similarweb-traffic-and-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-traffic-and-engagement-api-openapi.yml
- filename: similarweb-traffic-sources-api-openapi.yml
  format: yaml
  label: SimilarWeb Traffic Sources API
  slug: similarweb-traffic-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-traffic-sources-api-openapi.yml
- filename: similarweb-webhooks-api-openapi.yml
  format: yaml
  label: SimilarWeb Webhooks API
  slug: similarweb-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-webhooks-api-openapi.yml
consequence_counts:
  read: 19
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Similarweb Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'SimilarWeb exposes 27 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SimilarWeb
provider_slug: similarweb
slug: similarweb-agentic-access
source_filename: similarweb-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/similarweb-batch-api-openapi.yml, openapi/similarweb-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 19\n    acting: 8\n  by_consequence:\n    read: 19\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/batch/credits\n  method: get\n  operationId: getBatchCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch/v4/request-report\n  method: post\n  operationId: requestReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/v4/request-status\n  method: get\n  operationId: getRequestStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch/v4/request-validate\n  method: post\n  operationId: validateRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/v4/report-history\n  method: get\n  operationId: getReportHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch/v4/retry-request\n\
  \  method: post\n  operationId: retryRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/v4/tables-describe\n  method: get\n  operationId: describeTables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch/v4/s3-integration\n  method: post\n  operationId: createS3Integration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/v4/gcs-integration\n  method: post\n  operationId: createGcsIntegration\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/v4/integrations\n  method: get\n  operationId: getAllIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch/v4/webhooks/subscribe\n  method: post\n  operationId: subscribeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/v4/webhooks/list\n  method: get\n  operationId: listWebhookSubscriptions\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch/v4/webhooks/unsubscribe\n  method: delete\n  operationId: unsubscribeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batch/v4/webhooks/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/batch/credits\n  method: get\n  operationId: getCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v1/website/{domain_name}/capabilities\n  method: get\n  operationId: checkCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/website/{domain_name}/traffic-and-engagement/visits\n  method: get\n  operationId: getVisitsDesktop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/website/{domain_name}/traffic-and-engagement/bounce-rate\n  method: get\n  operationId: getBounceRateDesktop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/website/{domain_name}/traffic-sources/overview-share\n  method: get\n  operationId: getTrafficSourcesOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/website/{domain_name}/geo/traffic-by-country\n  method: get\n  operationId: getGeographyDesktop\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/website/{domain_name}/global-rank/global-rank\n  method: get\n  operationId: getGlobalRank\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/website-analysis/keywords\n  method: get\n  operationId: getWebsiteKeywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/website/{domain_name}/lead-enrichment/all\n  method: get\n  operationId: getLeadEnrichment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/apps/google/downloads\n  method: get\n  operationId: getAppDownloadsAndroid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5/apps/apple/downloads\n  method: get\n  operationId: getAppDownloadsIos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/website/{domain_name}/similar-sites\n  method: get\n  operationId: getSimilarSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/rank-tracker/{campaign_id}/reports/overview-report/performanceOverTime\n  method: get\n  operationId: getRankTrackingCampaignOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/agentic-access/similarweb-agentic-access.yml
summary_line: 27 operations · 8 acting
tags:
- Digital Intelligence
- Web Analytics
- Traffic Analytics
- Competitive Intelligence
- Keyword Analytics
- Audience Demographics
- App Intelligence
- Market Research
- E-Commerce
- SEO
---
