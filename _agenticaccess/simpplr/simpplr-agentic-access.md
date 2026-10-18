---
acting_count: 29
action_class_counts:
  acting: 29
  connected: 45
api_specs:
- filename: simpplr-alerts-api-openapi.yml
  format: yaml
  label: Simpplr Alerts API
  slug: simpplr-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-alerts-api-openapi.yml
- filename: simpplr-analytics-api-openapi.yml
  format: yaml
  label: Simpplr Analytics API
  slug: simpplr-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-analytics-api-openapi.yml
- filename: simpplr-audience-api-openapi.yml
  format: yaml
  label: Simpplr Audience API
  slug: simpplr-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-audience-api-openapi.yml
- filename: simpplr-blogs-api-openapi.yml
  format: yaml
  label: Simpplr Blogs API
  slug: simpplr-blogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-blogs-api-openapi.yml
- filename: simpplr-carousels-api-openapi.yml
  format: yaml
  label: Simpplr Carousels API
  slug: simpplr-carousels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-carousels-api-openapi.yml
- filename: simpplr-contents-api-openapi.yml
  format: yaml
  label: Simpplr Contents API
  slug: simpplr-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-contents-api-openapi.yml
- filename: simpplr-notifications-api-openapi.yml
  format: yaml
  label: Simpplr Notifications API
  slug: simpplr-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-notifications-api-openapi.yml
- filename: simpplr-people-api-openapi.yml
  format: yaml
  label: Simpplr People API
  slug: simpplr-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-people-api-openapi.yml
- filename: simpplr-search-api-openapi.yml
  format: yaml
  label: Simpplr Search API
  slug: simpplr-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-search-api-openapi.yml
- filename: simpplr-simpplr-api-gw-search-people-by-id-api-openapi.yml
  format: yaml
  label: Simpplr Simpplr Api Gw Search People By Id API
  slug: simpplr-simpplr-api-gw-search-people-by-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-simpplr-api-gw-search-people-by-id-api-openapi.yml
- filename: simpplr-sites-api-openapi.yml
  format: yaml
  label: Simpplr Sites API
  slug: simpplr-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/openapi/simpplr-sites-api-openapi.yml
consequence_counts:
  read: 45
  write: 29
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Simpplr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 74
overview: 'Simpplr exposes 74 API operations that an AI agent could call, of which 29 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 45 read and 29 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Simpplr
provider_slug: simpplr
slug: simpplr-agentic-access
source_filename: simpplr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/simpplr-api-gateway-openapi.yml, openapi/simpplr-api-gw-file-upload-openapi.yml,\n  openapi/simpplr-api-gw-search-people-by-id-openapi.yml, openapi/simpplr-staging-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 74\n  by_action_class:\n    acting: 29\n    connected: 45\n  by_consequence:\n    write: 29\n    read: 45\n  human_in_the_loop_required: 0\noperations:\n- path: /alerts\n  method: post\n  operationId: create-a-new-alert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /alerts\n  method: get\n  operationId: search-for-alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts/{alert-id}\n  method: put\n  operationId: update-an-alert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alerts/{alert-id}\n  method: delete\n  operationId: delete-an-alert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alerts/{alert-id}?expire=true\n  method: put\n  operationId:\
  \ expire-an-alert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analytics/adoption\n  method: get\n  operationId: app-adoption\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/adoption-average\n  method: get\n  operationId: app-adoption-average\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/app-adoption\n  method: get\n  operationId: app-adoption-1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/app-page-views\n\
  \  method: get\n  operationId: app-page-views\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/campaigns\n  method: get\n  operationId: campaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/content-engagement\n  method: get\n  operationId: content-engagement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/content-publications\n  method: get\n  operationId: content-publications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/content-referral-sources\n  method: get\n  operationId: content-referral-sources\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/content-views-by-type\n  method: get\n  operationId: content-views-by-type\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/content-views-list\n  method: get\n  operationId: content-views-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/knowledge-page-stats\n  method: get\n  operationId: knowledge-page-stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/low-activity-sites\n  method: get\n  operationId: low-activity-sites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/newsletter\n  method: get\n  operationId: news-letters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/people-count\n  method: get\n  operationId: people-count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/people-performance\n  method: get\n  operationId: people-performance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/profile-completeness\n  method: get\n  operationId: people-profile-completeness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /analytics/search-list\n  method: get\n  operationId: search-list-1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/searches\n  method: get\n  operationId: searches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/searches-performed\n  method: get\n  operationId: search-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/site-count\n  method: get\n  operationId: site-count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/site-popularity\n  method: get\n  operationId: site-popularity\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/site-publications\n  method: get\n  operationId: site-publications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/social-engagement\n  method: get\n  operationId: social-engagement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/social-engagement-list\n  method: get\n  operationId: social-engagement-list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /audience\n  method: post\n  operationId: add-audience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audience\n  method: put\n  operationId: update-audience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audience/{audience-id}\n  method: delete\n  operationId: delete-audience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /blogs\n  method: post\n  operationId: create-a-blog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /blogs/{content-id}\n  method: get\n  operationId: get-blog-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blogs/{content-id}\n  method: put\n  operationId: update-a-blog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /blogs/{content-id}\n  method: delete\n  operationId: delete-a-blog\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /carousels/{type}\n  method: get\n  operationId: get-carousel-data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contents\n  method: get\n  operationId: search-for-contents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contents/event/all\n  method: get\n  operationId: get-all-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contents/event/{content-id}\n  method: get\n  operationId: search-for-an-event-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /contents/mustread/active\n  method: get\n  operationId: get-must-read-content\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contents/page-categories\n  method: post\n  operationId: search-page-categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contents/page/{content-id}\n  method: get\n  operationId: search-for-a-page-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contents/site/{site-id}/content/{content-id}\n  method: delete\n  operationId: delete-a-page-by-id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contents/site/{site-id}/event\n  method: post\n  operationId: create-an-event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contents/site/{site-id}/event/{content-id}\n  method: put\n  operationId: update-an-event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contents/site/{site-id}/event/{content-id}\n  method: delete\n  operationId: delete-an-event-by-id\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contents/site/{site-id}/page/{content-id}\n  method: put\n  operationId: update-a-page\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contents/site/{site_id}/album\n  method: delete\n  operationId: delete-album-images-by-ids\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /notifications\n  method: post\n  operationId: create-a-notification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications\n  method: get\n  operationId: search-for-notifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/{notification-id}\n  method: put\n  operationId: update-a-notification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people\n  method: get\n  operationId:\
  \ search-for-people\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{people-id}\n  method: put\n  operationId: update-people\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: get\n  operationId: search-within-a-section\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/autocomplete\n  method: get\n  operationId: autocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/feed\n  method: get\n  operationId:\
  \ search-within-feed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites\n  method: post\n  operationId: create-a-site\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites\n  method: get\n  operationId: search-for-sites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/activate\n  method: put\n  operationId: update-site-as-active\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site-id}\n  method: get\n  operationId: get-site-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site-id}\n  method: put\n  operationId: update-a-site\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site-id}/follower/{follower-id}\n  method: post\n  operationId: add-a-follower-to-a-site\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /sites/{site-id}/follower/{follower-id}\n  method: delete\n  operationId: remove-a-follower-from-a-site\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site-id}/getFiles\n  method: get\n  operationId: search-for-site-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site-id}/member/{member-id}\n  method: post\n  operationId: add-a-member-to-a-site\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /sites/{site-id}/member/{member-id}\n  method: delete\n  operationId: remove-a-member-from-a-site\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contents/site/{site-id}/page\n  method: post\n  operationId: create-page\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /?\n  method: get\n  operationId: search-for-people-by-people-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analytics/views\n\
  \  method: get\n  operationId: app-adoption-2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contents/approval\n  method: get\n  operationId: fetch-all-content-for-approval\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contents/content/{content_id}/validate\n  method: post\n  operationId: validate-a-content\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contents/site/{site_id}/content/{content_id}/approval\n  method: post\n  operationId: content-approval\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contents/video\n  method: get\n  operationId: fetch-video-metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpplr/refs/heads/main/agentic-access/simpplr-agentic-access.yml
summary_line: 74 operations · 29 acting
tags:
- Company
- Employee Experience
- Intranet
- Employee Communications
- Digital Workplace
- Internal Communications
- Human Resources
- Collaboration
- Enterprise Software
- Salesforce
---
