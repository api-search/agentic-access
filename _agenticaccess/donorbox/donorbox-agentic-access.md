---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Campaigns API
  slug: donorbox-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Donations API
  slug: donorbox-donations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Plans API
  slug: donorbox-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Donors API
  slug: donorbox-donors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Events API
  slug: donorbox-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Tickets API
  slug: donorbox-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
- filename: donorbox-openapi.yml
  format: yaml
  label: Donorbox Event Ticket Purchases API
  slug: donorbox-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/openapi/donorbox-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Donorbox Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Donorbox exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Donorbox
provider_slug: donorbox
slug: donorbox-agentic-access
source_filename: donorbox-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/donorbox-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /donations\n  method: get\n  operationId: listDonations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /donors\n  method: get\n  operationId: listDonors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tickets\n  method: get\n  operationId: listTickets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchases\n  method: get\n  operationId: listPurchases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/donorbox/refs/heads/main/agentic-access/donorbox-agentic-access.yml
summary_line: 7 operations
tags:
- Nonprofit
- Fundraising
- Donations
- Payments
- Recurring Giving
- Event Ticketing
---
