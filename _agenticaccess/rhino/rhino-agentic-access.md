---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 4
api_specs:
- filename: rhino-authentication-api-openapi.yml
  format: yaml
  label: Rhino Authentication API
  slug: rhino-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhino/refs/heads/main/openapi/rhino-authentication-api-openapi.yml
- filename: rhino-partnerapi-v2-test-resident-api-openapi.yml
  format: yaml
  label: Rhino Partner Api::V2::Test::Resident API
  slug: rhino-partnerapi-v2-test-resident-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhino/refs/heads/main/openapi/rhino-partnerapi-v2-test-resident-api-openapi.yml
- filename: rhino-partnerapi-v2-test-sayrhinouser-api-openapi.yml
  format: yaml
  label: Rhino Partner Api::V2::Test::Sayrhino User API
  slug: rhino-partnerapi-v2-test-sayrhinouser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhino/refs/heads/main/openapi/rhino-partnerapi-v2-test-sayrhinouser-api-openapi.yml
- filename: rhino-prospects-api-openapi.yml
  format: yaml
  label: Rhino Prospects API
  slug: rhino-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhino/refs/heads/main/openapi/rhino-prospects-api-openapi.yml
- filename: rhino-webhooks-api-openapi.yml
  format: yaml
  label: Rhino Webhooks API
  slug: rhino-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhino/refs/heads/main/openapi/rhino-webhooks-api-openapi.yml
consequence_counts:
  read: 4
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rhino Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Rhino exposes 12 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Rhino
provider_slug: rhino
slug: rhino-agentic-access
source_filename: rhino-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: generated\nsource: openapi/rhino-partner-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 8\n    connected: 4\n  by_consequence:\n    write: 8\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /partners/{owner_slug}/prospects\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/{owner_slug}/prospects/{source}/{source_prospect_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partners/{owner_slug}/test/residents/{source}/{source_prospect_id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/{owner_slug}/test/sayrhino_users\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/{owner_slug}/webhooks/endpoints\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /partners/{owner_slug}/webhooks/endpoints\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/{owner_slug}/webhooks/endpoints/{endpoint_id}/deliveries\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partners/{owner_slug}/webhooks/endpoints/{endpoint_id}/deliveries/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partners/{owner_slug}/webhooks/endpoints/{endpoint_id}/deliveries/{id}/retry\n  method: post\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/{owner_slug}/webhooks/endpoints/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partners/{owner_slug}/webhooks/endpoints/{id}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /token\n  method: post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhino/refs/heads/main/agentic-access/rhino-agentic-access.yml
summary_line: 12 operations · 8 acting
tags:
- Insurance
- Insurtech
- Real-Estate
- Property Management
- Rentals
- Security Deposits
- Renters Insurance
- Webhook
- Partner API
---
