---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 14
api_specs:
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Club Members API
  slug: virtuagym-club-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Club Employees API
  slug: virtuagym-club-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Memberships API
  slug: virtuagym-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Billing API
  slug: virtuagym-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Visits API
  slug: virtuagym-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Events API
  slug: virtuagym-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
- filename: virtuagym-openapi.yml
  format: yaml
  label: Virtuagym Coaching Workouts API
  slug: virtuagym-coaching-workouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/openapi/virtuagym-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Virtuagym Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/club/{club_id}/invoices
operation_count: 27
overview: 'Virtuagym exposes 27 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 12 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Virtuagym
provider_slug: virtuagym
slug: virtuagym-agentic-access
source_filename: virtuagym-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/virtuagym-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 14\n    acting: 13\n  by_consequence:\n    read: 14\n    write: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/club/{club_id}/member\n  method: get\n  operationId: listClubMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/member\n  method: put\n  operationId: createClubMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/club/{club_id}/member/{member_id}\n  method: get\n  operationId: getClubMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/member/{member_id}\n  method: put\n  operationId: updateClubMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/club/{club_id}/member/create_or_update\n  method: put\n  operationId: createOrUpdateClubMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/club/{club_id}/member/activate_user\n  method: post\n  operationId: activateClubMemberUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/club/{club_id}/employee\n  method: get\n  operationId: listClubEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/employee\n  method: put\n  operationId: createClubEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/club/{club_id}/employee/{employee_id}\n  method: get\n  operationId: getClubEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/employee/{employee_id}\n  method: put\n  operationId: updateClubEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/club/{club_id}/membership/definition\n  method: get\n  operationId: listMembershipDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/membership/instance\n\
  \  method: get\n  operationId: listMembershipInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/credit\n  method: get\n  operationId: listMemberCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/credit\n  method: put\n  operationId: assignMemberCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/club/{club_id}/invoices\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/club/{club_id}/invoices/{invoice_id}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/visits\n  method: get\n  operationId: listVisits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/visits\n  method: post\n  operationId: createVisit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/club/{club_id}/visits/{visit_id}\n  method: get\n  operationId: getVisit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/events/{event_id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/eventparticipants\n  method: get\n  operationId: listEventParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/eventparticipants\n\
  \  method: post\n  operationId: createEventParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/club/{club_id}/eventparticipants\n  method: put\n  operationId: updateEventParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/club/{club_id}/eventparticipants/{event_participant_id}\n  method: get\n  operationId: getEventParticipant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/club/{club_id}/eventparticipants/{event_participant_id}\n\
  \  method: delete\n  operationId: deleteEventParticipant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/club/{club_id}/member/workouts\n  method: post\n  operationId: assignMemberWorkout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtuagym/refs/heads/main/agentic-access/virtuagym-agentic-access.yml
summary_line: 27 operations · 13 acting
tags:
- Fitness
- Health Club Management
- Gym Management
- Coaching
- Membership Management
- Fitness Software
- Wellness
- Scheduling
- SaaS
---
