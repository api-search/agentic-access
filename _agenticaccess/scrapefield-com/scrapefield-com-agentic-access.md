---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 51
api_specs:
- filename: scrapefield-com-account-api-openapi.yml
  format: yaml
  label: scrapefield-com Account API
  slug: scrapefield-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scrapefield-com/openapi/scrapefield-com-account-api-openapi.yml
- filename: scrapefield-com-catalogue-api-openapi.yml
  format: yaml
  label: scrapefield-com Catalogue API
  slug: scrapefield-com-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scrapefield-com/openapi/scrapefield-com-catalogue-api-openapi.yml
- filename: scrapefield-com-google-maps-api-openapi.yml
  format: yaml
  label: scrapefield-com Google Maps API
  slug: scrapefield-com-google-maps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scrapefield-com/openapi/scrapefield-com-google-maps-api-openapi.yml
- filename: scrapefield-com-instagram-api-openapi.yml
  format: yaml
  label: scrapefield-com Instagram API
  slug: scrapefield-com-instagram-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scrapefield-com/openapi/scrapefield-com-instagram-api-openapi.yml
- filename: scrapefield-com-tiktok-api-openapi.yml
  format: yaml
  label: scrapefield-com Tik Tok API
  slug: scrapefield-com-tiktok-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scrapefield-com/openapi/scrapefield-com-tiktok-api-openapi.yml
- filename: scrapefield-com-x-api-openapi.yml
  format: yaml
  label: scrapefield-com X API
  slug: scrapefield-com-x-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scrapefield-com/openapi/scrapefield-com-x-api-openapi.yml
- filename: scrapefield-com-linked-in-api-openapi.yml
  format: yaml
  label: scrapefield-com Linked In API
  slug: scrapefield-com-linked-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scrapefield-com/openapi/scrapefield-com-linked-in-api-openapi.yml
consequence_counts:
  read: 51
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Scrapefield Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 52
overview: 'scrapefield-com exposes 52 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 51 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: scrapefield-com
provider_slug: scrapefield-com
slug: scrapefield-com-agentic-access
source_filename: scrapefield-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/scrapefield-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 51\n    acting: 1\n  by_consequence:\n    read: 51\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /google-maps/places\n  method: get\n  operationId: search_places\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /google-maps/place\n  method: get\n  operationId: get_place\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /google-maps/reviews\n\
  \  method: get\n  operationId: get_place_reviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /google-maps/photos\n  method: get\n  operationId: get_place_photos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /google-maps/posts\n  method: get\n  operationId: get_place_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/profile\n  method: get\n  operationId: get_linkedin_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/company\n  method: get\n  operationId: get_linkedin_company\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/employee-stats\n  method: get\n  operationId: get_linkedin_employee_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/employees\n  method: get\n  operationId: get_linkedin_company_people\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/people\n  method: get\n  operationId: search_linkedin_people\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/services\n  method: get\n  operationId: search_linkedin_services\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /linkedin/companies\n  method: get\n  operationId: search_linkedin_companies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/posts\n  method: get\n  operationId: get_linkedin_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/post\n  method: get\n  operationId: get_linkedin_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/comments\n  method: get\n  operationId: get_linkedin_post_comments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/reactions\n  method: get\n  operationId: get_linkedin_post_reactions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/activity\n  method: get\n  operationId: get_linkedin_activity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/jobs\n  method: get\n  operationId: search_linkedin_jobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/job\n  method: get\n  operationId: get_linkedin_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/ads\n  method: get\n  operationId: search_linkedin_ads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /linkedin/ad\n  method: get\n  operationId: get_linkedin_ad\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/group\n  method: get\n  operationId: get_linkedin_group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linkedin/groups\n  method: get\n  operationId: search_linkedin_groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/profile\n  method: get\n  operationId: get_instagram_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/posts\n  method: get\n  operationId: get_instagram_posts\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/post\n  method: get\n  operationId: get_instagram_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/comments\n  method: get\n  operationId: get_instagram_comments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/hashtag\n  method: get\n  operationId: get_instagram_hashtag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instagram/search\n  method: get\n  operationId: search_instagram_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/profile\n  method: get\n  operationId: get_tiktok_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/followers\n  method: get\n  operationId: get_tiktok_followers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/videos\n  method: get\n  operationId: get_tiktok_videos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/video\n  method: get\n  operationId: get_tiktok_video\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/comments\n  method: get\n  operationId: get_tiktok_comments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/search\n  method: get\n  operationId: search_tiktok\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/trending\n  method: get\n  operationId: get_tiktok_trending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tiktok/ads\n  method: get\n  operationId: search_tiktok_ads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x/profile\n  method: get\n  operationId: get_x_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /x/posts\n  method: get\n  operationId: get_x_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x/post\n  method: get\n  operationId: get_x_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x/replies\n  method: get\n  operationId: get_x_replies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x/retweeters\n  method: get\n  operationId: get_x_retweeters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x/followers\n  method: get\n  operationId: get_x_followers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x/search\n  method: get\n  operationId: search_x\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x/community\n  method: get\n  operationId: get_x_community\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: listUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /endpoints\n  method: get\n  operationId: listEndpoints\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /errors\n  method: get\n  operationId: listErrors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signup\n  method: post\n  operationId: startSignup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /signup\n  method: get\n  operationId: pollSignup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/scrapefield-com/agentic-access/scrapefield-com-agentic-access.yml
summary_line: 52 operations · 1 acting
tags:
- Data
- Web Scraping
- Social Media
- Automation
---
