---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 22
api_specs:
- filename: hopin-bank-questions-api-openapi.yml
  format: yaml
  label: RingCentral Events Bank Questions API
  slug: hopin-bank-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-bank-questions-api-openapi.yml
- filename: hopin-booths-api-openapi.yml
  format: yaml
  label: RingCentral Events Booths API
  slug: hopin-booths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-booths-api-openapi.yml
- filename: hopin-data-subscriptions-api-openapi.yml
  format: yaml
  label: RingCentral Events Data Subscriptions API
  slug: hopin-data-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-data-subscriptions-api-openapi.yml
- filename: hopin-events-api-openapi.yml
  format: yaml
  label: RingCentral Events Events API
  slug: hopin-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-events-api-openapi.yml
- filename: hopin-health-api-openapi.yml
  format: yaml
  label: RingCentral Events Health API
  slug: hopin-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-health-api-openapi.yml
- filename: hopin-magic-links-api-openapi.yml
  format: yaml
  label: RingCentral Events Magic Links API
  slug: hopin-magic-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-magic-links-api-openapi.yml
- filename: hopin-organizations-api-openapi.yml
  format: yaml
  label: RingCentral Events Organizations API
  slug: hopin-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-organizations-api-openapi.yml
- filename: hopin-registrations-api-openapi.yml
  format: yaml
  label: RingCentral Events Registrations API
  slug: hopin-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-registrations-api-openapi.yml
- filename: hopin-reports-api-openapi.yml
  format: yaml
  label: RingCentral Events Reports API
  slug: hopin-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-reports-api-openapi.yml
- filename: hopin-schedule-items-api-openapi.yml
  format: yaml
  label: RingCentral Events Schedule Items API
  slug: hopin-schedule-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-schedule-items-api-openapi.yml
- filename: hopin-sessions-api-openapi.yml
  format: yaml
  label: RingCentral Events Sessions API
  slug: hopin-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-sessions-api-openapi.yml
- filename: hopin-stages-api-openapi.yml
  format: yaml
  label: RingCentral Events Stages API
  slug: hopin-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-stages-api-openapi.yml
- filename: hopin-templates-api-openapi.yml
  format: yaml
  label: RingCentral Events Templates API
  slug: hopin-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-templates-api-openapi.yml
- filename: hopin-tickets-api-openapi.yml
  format: yaml
  label: RingCentral Events Tickets API
  slug: hopin-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/hopin-tickets-api-openapi.yml
consequence_counts:
  read: 22
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hopin Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 31
overview: 'RingCentral Events exposes 31 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RingCentral Events
provider_slug: hopin
slug: hopin-agentic-access
source_filename: hopin-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    connected: 22\n    acting: 9\n  by_consequence:\n    read: 22\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/health\n  method: get\n  operationId: Health_Check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations\n  method: get\n  operationId: Retrieve_the_list_of_Organizations_property_of_the_user\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{organizationId}\n  method: get\n  operationId: Retrieve_the_details_of_the_Organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tickets/{ticketId}/bankQuestions\n  method: get\n  operationId: Returns_the_list_of_bank_questions_for_given_ticket_type\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{organizationId}/events\n  method: get\n  operationId: Returns_the_list_of_the_Organization_s_Events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{organizationId}/events\n  method: post\n  operationId:\
  \ Creates_an_Event_for_an_Organization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/events/{eventId}\n  method: get\n  operationId: Retrieve_Event_Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{eventId}/duplications\n  method: post\n  operationId: Duplicates_an_existing_Event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/events/{eventId}/registrations\n  method: get\n  operationId: Retrieve_the_list_of_registrations_for_an_Event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{eventId}/registrations\n  method: post\n  operationId: Create_a_registration_for_event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/registrations/{registrationId}\n  method: patch\n  operationId: Update_registration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/registrations/{registrationId}\n  method: get\n  operationId: Retrieve_registration_details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{eventId}/booths\n  method: get\n  operationId: Retrieve_Booths_for_an_Event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{eventId}/reports\n  method: get\n  operationId: Get_Reports_List_for_an_Event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports/{reportId}/download\n  method: get\n  operationId: Download_Report\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports/{reportId}\n  method: get\n  operationId: Get_Report_Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{eventId}/reports/{reportType}\n  method: post\n  operationId: Create_Report_for_an_Event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/booths/{boothId}/tags\n  method: get\n  operationId: Returns_the_list_of_tags_for_a_Booth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/booths/{scheduleId}/tags\n  method: get\n  operationId: Returns_the_list_of_tags_for_a_ScheduleItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{eventId}/dataSubscriptions\n  method: post\n  operationId: Create_a_new_data_subscription_for_an_Event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/events/{eventId}/scheduleItems\n  method: get\n  operationId: Retrieve_the_list_of_schedule_items_for_an_Event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{eventId}/sessions\n  method: get\n  operationId: Retrieve_the_list_of_sessions_for_an_Event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{eventId}/stages\n  method: get\n  operationId: Retrieve_Stages_for_an_Event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tickets/{ticketId}/magicLinks\n  method: post\n  operationId: Creates_Magic_Link_for_a_Ticket_type\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/tickets/{ticketId}/magicLinks\n  method: get\n  operationId: Retrieve_Magic_Links_for_a_Ticket_type\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/magicLinks/{magicLinkId}\n  method: delete\n  operationId: Deletes_Magic_Link\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/magicLinks/{magicLinkId}\n  method: get\n  operationId: Retrieve_Magic_Link_Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{eventId}/tickets\n\
  \  method: get\n  operationId: Retrieve_Ticket_Types_for_an_Event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tickets/{ticketId}\n  method: get\n  operationId: Retrieve_Ticket_Type_Details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/templates/{templateID}/event\n  method: post\n  operationId: Creates_an_event_from_template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{organizationId}/templates\n  method: get\n  operationId: Returns_the_list_of_the_organization_s_templates\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/agentic-access/hopin-agentic-access.yml
summary_line: 31 operations · 9 acting
tags:
- Event
- Virtual Events
- Hybrid Events
- Webinars
- Event Management
- Registration
- Sessions
- Networking
---
