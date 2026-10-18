---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 27
api_specs:
- filename: perk-cost-centers-api-openapi.yml
  format: yaml
  label: Perk Cost centers API
  slug: perk-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-cost-centers-api-openapi.yml
- filename: perk-custom-fields-api-openapi.yml
  format: yaml
  label: Perk Custom fields API
  slug: perk-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-custom-fields-api-openapi.yml
- filename: perk-bookings-api-openapi.yml
  format: yaml
  label: Perk Bookings API
  slug: perk-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-bookings-api-openapi.yml
- filename: perk-companies-api-openapi.yml
  format: yaml
  label: Perk Companies API
  slug: perk-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-companies-api-openapi.yml
- filename: perk-invoices-api-openapi.yml
  format: yaml
  label: Perk Invoices API
  slug: perk-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-invoices-api-openapi.yml
- filename: perk-profiles-api-openapi.yml
  format: yaml
  label: Perk Profiles API
  slug: perk-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-profiles-api-openapi.yml
- filename: perk-schemas-api-openapi.yml
  format: yaml
  label: Perk Schemas API
  slug: perk-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-schemas-api-openapi.yml
- filename: perk-suppliers-api-openapi.yml
  format: yaml
  label: Perk Suppliers API
  slug: perk-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-suppliers-api-openapi.yml
- filename: perk-trips-api-openapi.yml
  format: yaml
  label: Perk Trips API
  slug: perk-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-trips-api-openapi.yml
- filename: perk-users-api-openapi.yml
  format: yaml
  label: Perk Users API
  slug: perk-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-users-api-openapi.yml
- filename: perk-webhooks-api-openapi.yml
  format: yaml
  label: Perk Webhooks API
  slug: perk-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-webhooks-api-openapi.yml
- filename: perk-resource-types-api-openapi.yml
  format: yaml
  label: Perk Resource Types API
  slug: perk-resource-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-resource-types-api-openapi.yml
- filename: perk-service-provider-config-api-openapi.yml
  format: yaml
  label: Perk Service Provider Config API
  slug: perk-service-provider-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/openapi/perk-service-provider-config-api-openapi.yml
consequence_counts:
  read: 27
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Perk Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 42
overview: 'Perk exposes 42 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Perk
provider_slug: perk
slug: perk-agentic-access
source_filename: perk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/perk-cost-centers-api-openapi.yml, openapi/perk-custom-fields-api-openapi.yml,\n  openapi/perk-custom-fields-openapi.yml, openapi/perk-scim-server-openapi.yml, openapi/perk-travelperk-api-v1-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    connected: 27\n    acting: 15\n  by_consequence:\n    read: 27\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /cost_centers\n  method: get\n  operationId: list-cost-centers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost_centers\n  method: post\n  operationId: create-cost-center\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cost_centers/bulk_update\n  method: patch\n  operationId: bulk-update-cost-centers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cost_centers/{id}\n  method: get\n  operationId: get-cost-center\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cost_centers/{id}\n  method: patch\n  operationId: update-cost-center\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cost_centers/{id}/access\n  method: put\n  operationId: set-cost-center-access\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cost_centers/{id}/users\n  method: put\n  operationId: set-cost-center-users\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom-fields/{custom_field_id}/select-options\n\
  \  method: get\n  operationId: list-custom-field-select-options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /custom-fields/{custom_field_id}/select-options\n  method: post\n  operationId: create-custom-field-select-options\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom-fields/{custom_field_id}/select-options/{option_id}/{archive_action}\n  method: post\n  operationId: archive-custom-field-select-option\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /ResourceTypes\n  method: get\n  operationId: list-resource-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Schemas\n  method: get\n  operationId: list-all-schemas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Schemas/urn:ietf:params:scim:schemas:core:2.0:User\n  method: get\n  operationId: get-user-schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Schemas/urn:ietf:params:scim:schemas:extension:enterprise:2.0:User\n  method: get\n  operationId: retrieve-an-enterprise-user\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /Schemas/urn:ietf:params:scim:schemas:extension:perkcustomfields:2.0:User\n  method: get\n  operationId: get_schemas-urn-ietf-params-scim-schemas-extension-perkcustomfields-2-0-user\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Schemas/urn:ietf:params:scim:schemas:extension:travelperk:2.0:User\n  method: get\n  operationId: custom-user-schema-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ServiceProviderConfig\n  method: get\n  operationId: service-provider-configuration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Users\n  method: post\n  operationId: create-a-new-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Users\n  method: get\n  operationId: list-all-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Users/{id}\n  method: patch\n  operationId: update-a-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Users/{id}\n  method: put\n  operationId: replace-a-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Users/{id}\n  method: get\n  operationId: retrieve-a-user-1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Users/{id}\n  method: delete\n  operationId: deactivate-a-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookings\n  method: get\n  operationId: list-all-bookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies\n  method: get\n  operationId: list-invoice-profiles-1\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: get\n  operationId: list-invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/lines\n  method: get\n  operationId: list-invoice-lines-1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{serial_number}\n  method: get\n  operationId: get-invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices/{serial_number}/pdf\n  method: get\n  operationId: download-pdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profiles\n \
  \ method: get\n  operationId: list-invoice-profiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suppliers\n  method: get\n  operationId: list-all-suppliers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips\n  method: get\n  operationId: list-all-trips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips/{id}\n  method: get\n  operationId: retrieve-a-trip-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trips/{trip_id}/custom-fields\n  method: get\n  operationId: retrieve-custom-fields\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: list-all-users-1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: subscribe-to-event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: list-webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/events\n  method: get\n  operationId: list-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: patch\n  operationId: update-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: get\n  operationId: get-subscription-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: delete\n  operationId: delete-webhook-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /webhooks/{id}/test\n  method: post\n  operationId: test-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/agentic-access/perk-agentic-access.yml
summary_line: 42 operations · 15 acting
tags:
- Company
- Corporate Travel
- Expense Management
- Spend Management
- Travel
- Invoices
- Fintech
- Software-as-a-Service
---
