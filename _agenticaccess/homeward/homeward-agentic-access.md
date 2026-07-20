---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 1
api_specs:
- filename: homeward-offer-estimate-openapi.yml
  format: yaml
  label: Homeward Offer Estimate API
  slug: homeward-offer-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/homeward/refs/heads/main/openapi/homeward-offer-estimate-openapi.yml
consequence_counts:
  read: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Homeward Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Homeward exposes 5 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Homeward
provider_slug: homeward
slug: homeward-agentic-access
source_filename: homeward-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/homeward-offer-estimate-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 4\n    connected: 1\n  by_consequence:\n    write: 4\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/1.0.0/partner/offer-request/\n  method: post\n  operationId: createOfferRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1.0.0/estimate/sell/{preliminary_offer_id}/\n  method: get\n  operationId:\
  \ getOfferEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1.0.0/partner/offer-request/{offer_request_id}/agent/\n  method: patch\n  operationId: updateOfferRequestAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buybox/\n  method: post\n  operationId: checkBuyboxEligibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agents/finalize-lead/{lead_id}/\n  method: post\n  operationId: finalizeOfferRequest\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homeward/refs/heads/main/agentic-access/homeward-agentic-access.yml
summary_line: 5 operations · 4 acting
tags:
- Company
- Real Estate
- Home Finance
- Mortgage
- Proptech
- Cash Offer
- Title
- Lending
---
