---
acting_count: 35
action_class_counts:
  acting: 35
  connected: 22
api_specs:
- filename: tito-openapi.yml
  format: yaml
  label: Tito Events API
  slug: tito-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Releases API
  slug: tito-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Tickets API
  slug: tito-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Registrations API
  slug: tito-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Discount Codes API
  slug: tito-discount-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Activities API
  slug: tito-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Check-in Lists API
  slug: tito-check-in-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Refunds API
  slug: tito-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Webhook Endpoints API
  slug: tito-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
consequence_counts:
  read: 22
  write: 35
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tito Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 57
overview: 'Tito exposes 57 API operations that an AI agent could call, of which 35 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 35 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tito
provider_slug: tito
slug: tito-agentic-access
source_filename: tito-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tito-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 57\n  by_action_class:\n    connected: 22\n    acting: 35\n  by_consequence:\n    read: 22\n    write: 35\n  human_in_the_loop_required: 0\noperations:\n- path: /hello\n  method: get\n  operationId: hello\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/events\n  method: post\n  operationId:\
  \ createEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/events/past\n  method: get\n  operationId: listPastEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/events/archived\n  method: get\n  operationId: listArchivedEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}\n\
  \  method: patch\n  operationId: updateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}\n  method: delete\n  operationId: deleteEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/duplication\n  method: post\n  operationId: duplicateEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/duplication\n  method: get\n  operationId: getEventDuplicationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/releases\n  method: get\n  operationId: listReleases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/releases\n  method: post\n  operationId: createRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/releases/{release_slug}\n  method: get\n  operationId:\
  \ getRelease\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/releases/{release_slug}\n  method: patch\n  operationId: updateRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/releases/{release_slug}\n  method: delete\n  operationId: deleteRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/releases/{release_slug}/archival\n\
  \  method: post\n  operationId: archiveRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/releases/{release_slug}/archival\n  method: delete\n  operationId: unarchiveRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/releases/{release_slug}/duplication\n  method: post\n  operationId: duplicateRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/releases/{release_slug}/activation\n  method: patch\n  operationId: activateRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/releases/{release_slug}/deactivation\n  method: patch\n  operationId: deactivateRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/releases/{release_slug}/publication\n  method:\
  \ post\n  operationId: publishRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/releases/{release_slug}/publication\n  method: delete\n  operationId: unpublishRelease\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/tickets\n  method: get\n  operationId: listTickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/tickets\n\
  \  method: post\n  operationId: createTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/tickets/{ticket_slug}\n  method: get\n  operationId: getTicket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/tickets/{ticket_slug}\n  method: patch\n  operationId: updateTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/tickets/{ticket_slug}/reassignments\n\
  \  method: post\n  operationId: reassignTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/tickets/{ticket_slug}/void\n  method: post\n  operationId: voidTicket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/registrations\n  method: get\n  operationId: listRegistrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/registrations\n\
  \  method: post\n  operationId: createRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/registrations/{registration_slug}\n  method: get\n  operationId: getRegistration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/registrations/{registration_slug}\n  method: patch\n  operationId: updateRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /{account_slug}/{event_slug}/registrations/{registration_slug}/confirmations\n  method: post\n  operationId: markRegistrationPaid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/registrations/{registration_slug}/confirmations\n  method: delete\n  operationId: markRegistrationUnpaid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/discount_codes\n  method: get\n  operationId: listDiscountCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/discount_codes\n  method: post\n  operationId: createDiscountCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/discount_codes/{discount_code_id}\n  method: get\n  operationId: getDiscountCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/discount_codes/{discount_code_id}\n  method: patch\n  operationId: updateDiscountCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/discount_codes/{discount_code_id}\n  method: delete\n  operationId: deleteDiscountCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/activities\n  method: get\n  operationId: listActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/activities\n  method: post\n  operationId: createActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/activities/{activity_id}\n  method: get\n  operationId: getActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/activities/{activity_id}\n  method: patch\n  operationId: updateActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/activities/{activity_id}\n  method: delete\n  operationId: deleteActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/activities/{activity_id}/duplication\n  method: post\n  operationId: duplicateActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/checkin_lists\n  method: get\n  operationId: listCheckinLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/checkin_lists\n  method: post\n  operationId: createCheckinList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/checkin_lists/{checkin_list_slug}\n  method: get\n  operationId: getCheckinList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/checkin_lists/{checkin_list_slug}\n  method: patch\n  operationId: updateCheckinList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/checkin_lists/{checkin_list_slug}\n  method: delete\n  operationId: deleteCheckinList\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/refunds\n  method: get\n  operationId: listRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/refunds/{refund_id}\n  method: get\n  operationId: getRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/webhook_endpoints\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/webhook_endpoints\n\
  \  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/webhook_endpoints/{id}\n  method: get\n  operationId: getWebhookEndpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{account_slug}/{event_slug}/webhook_endpoints/{id}\n  method: patch\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{account_slug}/{event_slug}/webhook_endpoints/{id}\n\
  \  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/agentic-access/tito-agentic-access.yml
summary_line: 57 operations · 35 acting
tags:
- Event Ticketing
- Events
- Registration
- Ticketing
- Conferences
- Event Management
- Attendees
- Webhooks
- SaaS
---
