---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 22
api_specs:
- filename: openapi.json
  format: json
  label: NTHU Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://api.nthusa.tw/openapi.json
consequence_counts:
  read: 22
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nthu Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'National Tsing Hua University exposes 23 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: National Tsing Hua University
provider_slug: nthu
slug: nthu-agentic-access
source_filename: nthu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nthu-data-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 22\n    acting: 1\n  by_consequence:\n    read: 22\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /announcements/\n  method: get\n  operationId: getAnnouncements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /announcements/sources\n  method: get\n  operationId: getAnnouncementsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /announcements/lists/departments\n\
  \  method: get\n  operationId: listAnnouncementDepartments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buses/routes\n  method: get\n  operationId: getBusRouteData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buses/info/stops\n  method: get\n  operationId: getBusStopsInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buses/schedules\n  method: get\n  operationId: getBusSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buses/stops/{stop_name}\n  method: get\n  operationId: getStopBusInformationByStop\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/\n  method: get\n  operationId: getAllCourses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/search\n  method: get\n  operationId: searchCoursesByFieldAndValue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/search\n  method: post\n  operationId: searchCoursesByCondition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /courses/lists/{list_name}\n  method: get\n  operationId: listCoursesByType\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /departments/\n  method: get\n  operationId: getAllDepartments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /departments/search\n  method: get\n  operationId: searchDepartmentsAndPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dining/\n  method: get\n  operationId: getDiningData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dining/open\n  method: get\n  operationId: getOpenRestaurants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /energy/electricity_usage\n  method: get\n  operationId: getRealtimeElectricityUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /libraries/space\n  method: get\n  operationId: getLibrarySpaceAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /libraries/lost_and_found\n  method: get\n  operationId: getLibraryLostAndFoundItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /libraries/rss/{rss_type}\n  method: get\n  operationId: getLibraryRssData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/\n  method: get\n  operationId: getAllLocations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/search\n  method: get\n  operationId: fuzzySearchLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/\n  method: get\n  operationId: getAllNewsletters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter_name}\n  method: get\n  operationId: getNewsletterByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/agentic-access/nthu-agentic-access.yml
summary_line: 23 operations · 1 acting
tags:
- Education
- Higher Education
- University
- Taiwan
- Open Data
- Campus
---
