---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 29
api_specs:
- filename: ometria-contacts-api-openapi.yml
  format: yaml
  label: Ometria Contacts API
  slug: ometria-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-contacts-api-openapi.yml
- filename: ometria-custom-event-api-openapi.yml
  format: yaml
  label: Ometria Custom Event API
  slug: ometria-custom-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-custom-event-api-openapi.yml
- filename: ometria-custom-fields-api-openapi.yml
  format: yaml
  label: Ometria Custom Fields API
  slug: ometria-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-custom-fields-api-openapi.yml
- filename: ometria-field-forget-email-phone-erasure-api-openapi.yml
  format: yaml
  label: Ometria Field forget (email / phone erasure) API
  slug: ometria-field-forget-email-phone-erasure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-field-forget-email-phone-erasure-api-openapi.yml
- filename: ometria-gdpr-anonymisation-requests-api-openapi.yml
  format: yaml
  label: Ometria GDPR anonymisation requests API
  slug: ometria-gdpr-anonymisation-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-gdpr-anonymisation-requests-api-openapi.yml
- filename: ometria-lists-api-openapi.yml
  format: yaml
  label: Ometria Lists API
  slug: ometria-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-lists-api-openapi.yml
- filename: ometria-orders-api-openapi.yml
  format: yaml
  label: Ometria Orders API
  slug: ometria-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-orders-api-openapi.yml
- filename: ometria-products-api-openapi.yml
  format: yaml
  label: Ometria Products API
  slug: ometria-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-products-api-openapi.yml
- filename: ometria-profiles-api-openapi.yml
  format: yaml
  label: Ometria Profiles API
  slug: ometria-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-profiles-api-openapi.yml
- filename: ometria-push-api-openapi.yml
  format: yaml
  label: Ometria Push API
  slug: ometria-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-push-api-openapi.yml
- filename: ometria-transactional-email-api-openapi.yml
  format: yaml
  label: Ometria Transactional Email API
  slug: ometria-transactional-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-transactional-email-api-openapi.yml
- filename: ometria-translation-requests-api-openapi.yml
  format: yaml
  label: Ometria Translation Requests API
  slug: ometria-translation-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-translation-requests-api-openapi.yml
- filename: ometria-unsubscribes-api-openapi.yml
  format: yaml
  label: Ometria Unsubscribes API
  slug: ometria-unsubscribes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ometria/openapi/ometria-unsubscribes-api-openapi.yml
consequence_counts:
  physical: 1
  read: 29
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ometria Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transactional-email/send
operation_count: 39
overview: 'Ometria exposes 39 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 9 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ometria
provider_slug: ometria
slug: ometria-agentic-access
source_filename: ometria-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/ometria-data-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    connected: 29\n    acting: 10\n  by_consequence:\n    read: 29\n    write: 9\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /contacts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{collection}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{collection}/{contact_id}\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-events/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-events/{event_type}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-events/{event_type}/{event_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_fields\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom_fields\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom_fields\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom_fields/{category}/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-deletion-requests\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-deletion-requests\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-deletion-requests/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /field-forget\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /field-forget\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /field-forget/bulk\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /field-forget/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{list_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{list_id}/changes\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{list_id}/contacts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{list_id}/contacts_export\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merge-profile\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merge-profile\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /merge-profile/{job_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/{product_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles/{profile_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /push\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /push/_errors\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactional-email/send\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /translations/requests\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translations/requests/{request_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translations/requests/{request_id}/preview\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translations/submit\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unsubscribes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ometria/agentic-access/ometria-agentic-access.yml
summary_line: 39 operations · 10 acting
tags:
- Company
- Retail
- Customer Data Platform
- Artificial Intelligence
- Marketing
---
