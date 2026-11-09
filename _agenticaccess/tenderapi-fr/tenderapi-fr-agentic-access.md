---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 12
api_specs:
- filename: tenderapi-fr-auth-api-openapi.yml
  format: yaml
  label: tenderapi-fr Auth API
  slug: tenderapi-fr-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderapi-fr/openapi/tenderapi-fr-auth-api-openapi.yml
- filename: tenderapi-fr-awards-api-openapi.yml
  format: yaml
  label: tenderapi-fr Awards API
  slug: tenderapi-fr-awards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderapi-fr/openapi/tenderapi-fr-awards-api-openapi.yml
- filename: tenderapi-fr-billing-api-openapi.yml
  format: yaml
  label: tenderapi-fr Billing API
  slug: tenderapi-fr-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderapi-fr/openapi/tenderapi-fr-billing-api-openapi.yml
- filename: tenderapi-fr-health-api-openapi.yml
  format: yaml
  label: tenderapi-fr Health API
  slug: tenderapi-fr-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderapi-fr/openapi/tenderapi-fr-health-api-openapi.yml
- filename: tenderapi-fr-keys-api-openapi.yml
  format: yaml
  label: tenderapi-fr Keys API
  slug: tenderapi-fr-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderapi-fr/openapi/tenderapi-fr-keys-api-openapi.yml
- filename: tenderapi-fr-profiles-api-openapi.yml
  format: yaml
  label: tenderapi-fr Profiles API
  slug: tenderapi-fr-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderapi-fr/openapi/tenderapi-fr-profiles-api-openapi.yml
- filename: tenderapi-fr-renewals-api-openapi.yml
  format: yaml
  label: tenderapi-fr Renewals API
  slug: tenderapi-fr-renewals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderapi-fr/openapi/tenderapi-fr-renewals-api-openapi.yml
- filename: tenderapi-fr-tenders-api-openapi.yml
  format: yaml
  label: tenderapi-fr Tenders API
  slug: tenderapi-fr-tenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderapi-fr/openapi/tenderapi-fr-tenders-api-openapi.yml
consequence_counts:
  physical: 2
  read: 12
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tenderapi Fr Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/start
operation_count: 23
overview: 'tenderapi-fr exposes 23 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 9 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tenderapi-fr
provider_slug: tenderapi-fr
slug: tenderapi-fr-agentic-access
source_filename: tenderapi-fr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/tenderapi-fr-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 12\n    acting: 11\n  by_consequence:\n    read: 12\n    write: 9\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /tenders\n  method: get\n  operationId: search_tenders_tenders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenders/{tender_id}\n  method: get\n  operationId: get_tender_tenders__tender_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /awards\n  method: get\n  operationId: search_awards_awards_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /awards/winner-intel\n  method: get\n  operationId: winner_intelligence_awards_winner_intel_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /awards/{award_id}\n  method: get\n  operationId: get_award_awards__award_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /renewals\n  method: get\n  operationId: search_renewals_renewals_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles\n  method: post\n  operationId:\
  \ create_profile_profiles_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles\n  method: get\n  operationId: list_profiles_profiles_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/preview/locked\n  method: post\n  operationId: preview_locked_profiles_preview_locked_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/preview\n  method: post\n  operationId: preview_profile_profiles_preview_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profile_id}\n  method: get\n  operationId: get_profile_profiles__profile_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{profile_id}\n  method: put\n  operationId: update_profile_profiles__profile_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profile_id}\n  method: delete\n  operationId: delete_profile_profiles__profile_id__delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profiles/{profile_id}/set-active\n  method: post\n  operationId: set_profile_active_profiles__profile_id__set_active_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /keys/me\n  method: get\n  operationId: get_my_key_keys_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: get_me_me_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/start\n  method: post\n  operationId: start_checkout_billing_start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/checkout\n  method: post\n  operationId: create_checkout_billing_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/portal\n  method: post\n\
  \  operationId: customer_portal_billing_portal_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/login\n  method: post\n  operationId: login_auth_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/session\n  method: get\n  operationId: session_info_auth_session_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/logout\n  method: post\n  operationId: logout_auth_logout_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/tenderapi-fr/agentic-access/tenderapi-fr-agentic-access.yml
summary_line: 23 operations · 11 acting
tags:
- Company
- Procurement
- Public Data
- France
- Europe
---
