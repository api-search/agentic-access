---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 28
api_specs:
- filename: tum-locations-api-openapi.yml
  format: yaml
  label: NavigaTUM
  slug: navigatum
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tum/refs/heads/main/openapi/tum-locations-api-openapi.yml
- filename: tum-menu-api-openapi.yml
  format: yaml
  label: eat-api — Munich Student Canteen Menus
  slug: eat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tum/refs/heads/main/openapi/tum-menu-api-openapi.yml
- filename: tum-campus-api-openapi.yml
  format: yaml
  label: Technical University of Munich Campus API
  slug: tum-campus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tum/refs/heads/main/openapi/tum-campus-api-openapi.yml
consequence_counts:
  physical: 1
  read: 28
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tum Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/feedback/feedback
operation_count: 38
overview: 'Technical University of Munich exposes 38 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 9 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Technical University of Munich
provider_slug: tum
slug: tum-agentic-access
source_filename: tum-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/tum-calendar-api-openapi.yml, openapi/tum-campus-api-openapi.yml, openapi/tum-feedback-api-openapi.yml,\n  openapi/tum-locations-api-openapi.yml, openapi/tum-maps-api-openapi.yml, openapi/tum-menu-api-openapi.yml,\n  openapi/tum-openapi-json-api-openapi.yml, openapi/tum-static-api-openapi.yml, openapi/tum-status-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 38\n  by_action_class:\n    connected: 28\n    acting: 10\n  by_consequence:\n    read: 28\n    write: 9\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/calendar\n  method: post\n  operationId: calendar_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /canteen/allCanteens\n  method: get\n  operationId: Campus_ListCanteens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /canteen/headCount/{canteenId}\n  method: get\n  operationId: Campus_GetCanteenHeadCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /canteen/rating/allRatingTags\n  method: get\n  operationId: Campus_ListAvailableCanteenTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /canteen/rating/get\n  method: post\n  operationId: Campus_ListCanteenRatings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /canteen/rating/new\n  method: post\n  operationId: Campus_CreateCanteenRating\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /device\n  method: post\n  operationId: Campus_CreateDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /device/{deviceId}\n  method: delete\n  operationId: Campus_DeleteDevice\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dish/rating/allDishTags\n  method: get\n  operationId: Campus_ListNameTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dish/rating/allRatingTags\n  method: get\n  operationId: Campus_ListAvailableDishTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dish/rating/get\n  method: post\n  operationId: Campus_GetDishRatings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /dish/rating/new\n  method: post\n  operationId: Campus_CreateDishRating\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dishes\n  method: get\n  operationId: Campus_ListDishes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feedback\n  method: post\n  operationId: Campus_CreateFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /movies/{lastId}\n  method: get\n\
  \  operationId: Campus_ListMovies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news\n  method: get\n  operationId: Campus_ListNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news/alerts\n  method: get\n  operationId: Campus_ListNewsAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news/sources\n  method: get\n  operationId: Campus_ListNewsSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /student_clubs\n  method: get\n  operationId: Campus_ListStudentClub\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /updatenote/{version}\n  method: get\n  operationId: Campus_GetUpdateNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/feedback/feedback\n  method: post\n  operationId: send_feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/feedback/get_token\n  method: post\n  operationId: get_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/feedback/propose_edits\n  method: post\n  operationId: propose_edits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/locations/{id}\n  method: get\n  operationId: get_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/locations/{id}/nearby\n  method: get\n  operationId: nearby_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/locations/{id}/preview\n  method: get\n  operationId: maps_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/locations/{id}/qr-code\n  method: get\n  operationId: qr_code_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: get\n  operationId: search_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/maps/route\n  method: get\n  operationId: route_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{canteen_id}/{year}/{week}.json\n  method: get\n  operationId: getByCanteenIdByYear{week}Json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{canteen_id}/combined/combined.json\n\
  \  method: get\n  operationId: getByCanteenIdCombinedCombinedJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /all.json\n  method: get\n  operationId: getAllJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /all_ref.json\n  method: get\n  operationId: getAllRefJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/openapi.json\n  method: get\n  operationId: openapi_doc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enums/canteens.json\n  method: get\n  operationId: getEnumsCanteensJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enums/languages.json\n  method: get\n  operationId: getEnumsLanguagesJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enums/labels.json\n  method: get\n  operationId: getEnumsLabelsJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/status\n  method: get\n  operationId: health_status_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tum/refs/heads/main/agentic-access/tum-agentic-access.yml
summary_line: 38 operations · 10 acting
tags:
- University
- Higher Education
- Education
- Germany
- Technical University
- Universities of Excellence
- Campus
- Course Catalog
- Identity Federation
- Research Repository
- Open Source
- Student Information System
---
