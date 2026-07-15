---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Donations API
  slug: fundraiseup-donations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Recurring Plans API
  slug: fundraiseup-recurring-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Supporters API
  slug: fundraiseup-supporters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Events API
  slug: fundraiseup-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
- filename: fundraiseup-openapi.yml
  format: yaml
  label: Fundraise Up Donor Portal Access Links API
  slug: fundraiseup-donor-portal-access-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/openapi/fundraiseup-openapi.yml
consequence_counts:
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fundraiseup Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Fundraise Up exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fundraise Up
provider_slug: fundraiseup
slug: fundraiseup-agentic-access
source_filename: fundraiseup-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fundraiseup-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 8\n    acting: 6\n  by_consequence:\n    read: 8\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /donations\n  method: get\n  operationId: listDonations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /donations\n  method: post\n  operationId: createDonation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /donations/{id}\n  method: get\n  operationId: getDonation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /donations/{id}\n  method: post\n  operationId: updateDonation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recurring_plans\n  method: get\n  operationId: listRecurringPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurring_plans\n  method: post\n  operationId: createRecurringPlan\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recurring_plans/{id}\n  method: get\n  operationId: getRecurringPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recurring_plans/{id}\n  method: post\n  operationId: updateRecurringPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /supporters\n  method: get\n  operationId: listSupporters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /supporters/{id}\n  method: get\n  operationId: getSupporter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /donor_portal/access_links/supporters/{id}\n  method: post\n  operationId: createSupporterAccessLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /donor_portal/access_links/recurring_plans/{id}\n  method: post\n  operationId: createRecurringPlanAccessLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundraiseup/refs/heads/main/agentic-access/fundraiseup-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- Fundraising
- Donations
- Nonprofit
- Payments
- Recurring Giving
- Donor Management
---
