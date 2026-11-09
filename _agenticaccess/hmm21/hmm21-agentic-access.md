---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: hmm21-arrival-notice-api-openapi.yml
  format: yaml
  label: HMM Arrival Notice API
  slug: hmm21-arrival-notice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-arrival-notice-api-openapi.yml
- filename: hmm21-bookings-api-openapi.yml
  format: yaml
  label: HMM Bookings API
  slug: hmm21-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-bookings-api-openapi.yml
- filename: hmm21-eblcompany-id-requests-api-openapi.yml
  format: yaml
  label: HMM Eblcompany Id Requests API
  slug: hmm21-eblcompany-id-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-eblcompany-id-requests-api-openapi.yml
- filename: hmm21-kr-nexawave-cert-file-api-openapi.yml
  format: yaml
  label: HMM KR NEXAWAVE CERT FILE API
  slug: hmm21-kr-nexawave-cert-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-kr-nexawave-cert-file-api-openapi.yml
- filename: hmm21-kr-nexawave-class-survey-api-openapi.yml
  format: yaml
  label: HMM KR NEXAWAVE CLASS SURVEY API
  slug: hmm21-kr-nexawave-class-survey-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-kr-nexawave-class-survey-api-openapi.yml
- filename: hmm21-kr-nexawave-cms-pms-api-openapi.yml
  format: yaml
  label: HMM KR NEXAWAVE CMS PMS API
  slug: hmm21-kr-nexawave-cms-pms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hmm21/openapi/hmm21-kr-nexawave-cms-pms-api-openapi.yml
consequence_counts:
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hmm21 Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'HMM exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HMM
provider_slug: hmm21
slug: hmm21-agentic-access
source_filename: hmm21-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/hmm21-arrival-notice-openapi.yml, openapi/hmm21-booking-openapi.yml, openapi/hmm21-certificate-file-openapi.yml,\n  openapi/hmm21-class-survey-status-openapi.yml, openapi/hmm21-cms-pms-status-openapi.yml, openapi/hmm21-ebl-company-id-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 5\n    acting: 4\n  by_consequence:\n    read: 5\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /arrival-notice\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings\n  method: post\n  operationId: create-bookings\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookings/{bookingReference}\n  method: get\n  operationId: get-bookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/{bookingReference}\n  method: put\n  operationId: update-bookings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookings/{bookingReference}\n  method: patch\n  operationId: cancel-booking\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{certno}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{imono}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{imono}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eblcompany-id-requests\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/hmm21/agentic-access/hmm21-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Company
- Shipping
- Logistics
- Container Shipping
- Maritime
- DCSA
- Supply Chain
---
