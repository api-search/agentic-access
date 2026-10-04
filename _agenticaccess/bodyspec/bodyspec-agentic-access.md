---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 35
api_specs:
- filename: bodyspec-api-status-api-openapi.yml
  format: yaml
  label: BodySpec API Status API
  slug: bodyspec-api-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-api-status-api-openapi.yml
- filename: bodyspec-appointments-api-openapi.yml
  format: yaml
  label: BodySpec Appointments API
  slug: bodyspec-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-appointments-api-openapi.yml
- filename: bodyspec-availability-api-openapi.yml
  format: yaml
  label: BodySpec Availability API
  slug: bodyspec-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-availability-api-openapi.yml
- filename: bodyspec-bodyspec-api-api-openapi.yml
  format: yaml
  label: BodySpec BodySpec API
  slug: bodyspec-bodyspec-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-bodyspec-api-api-openapi.yml
- filename: bodyspec-locations-api-openapi.yml
  format: yaml
  label: BodySpec Locations API
  slug: bodyspec-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-locations-api-openapi.yml
- filename: bodyspec-partner-appointments-api-openapi.yml
  format: yaml
  label: BodySpec Partner Appointments API
  slug: bodyspec-partner-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-appointments-api-openapi.yml
- filename: bodyspec-partner-intake-api-openapi.yml
  format: yaml
  label: BodySpec Partner Intake API
  slug: bodyspec-partner-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-intake-api-openapi.yml
- filename: bodyspec-partner-orders-api-openapi.yml
  format: yaml
  label: BodySpec Partner Orders API
  slug: bodyspec-partner-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-orders-api-openapi.yml
- filename: bodyspec-partner-results-api-openapi.yml
  format: yaml
  label: BodySpec Partner Results API
  slug: bodyspec-partner-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-results-api-openapi.yml
- filename: bodyspec-partner-users-api-openapi.yml
  format: yaml
  label: BodySpec Partner Users API
  slug: bodyspec-partner-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-users-api-openapi.yml
- filename: bodyspec-partner-webhooks-api-openapi.yml
  format: yaml
  label: BodySpec Partner Webhooks API
  slug: bodyspec-partner-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-partner-webhooks-api-openapi.yml
- filename: bodyspec-reservations-api-openapi.yml
  format: yaml
  label: BodySpec Reservations API
  slug: bodyspec-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-reservations-api-openapi.yml
- filename: bodyspec-results-api-openapi.yml
  format: yaml
  label: BodySpec Results API
  slug: bodyspec-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-results-api-openapi.yml
- filename: bodyspec-services-api-openapi.yml
  format: yaml
  label: BodySpec Services API
  slug: bodyspec-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-services-api-openapi.yml
- filename: bodyspec-users-api-openapi.yml
  format: yaml
  label: BodySpec Users API
  slug: bodyspec-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/openapi/bodyspec-users-api-openapi.yml
consequence_counts:
  physical: 2
  read: 35
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bodyspec Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/partners/{partner_id}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v1/partners/{partner_id}/orders/{order_id}
operation_count: 45
overview: 'BodySpec exposes 45 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read, 8 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BodySpec
provider_slug: bodyspec
slug: bodyspec-agentic-access
source_filename: bodyspec-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: generated\nsource: openapi/bodyspec-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 45\n  by_action_class:\n    connected: 35\n    acting: 10\n  by_consequence:\n    read: 35\n    write: 8\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/info\n  method: get\n  operationId: api_info_api_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - email\n    - openid\n    - profile\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    scope:\n    - email\n    - openid\n    - profile\n- path: /api/v1/users/me\n  method: get\n  operationId: _get_user_api_v1_users_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/me\n  method: patch\n  operationId: _update_user_api_v1_users_me_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/users/me/appts\n  method: get\n  operationId: _list_appts_api_v1_users_me_appts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/me/appts/{appt_id}\n  method: get\n\
  \  operationId: _get_appt_api_v1_users_me_appts__appt_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/me/results/\n  method: get\n  operationId: _get_results_api_v1_users_me_results__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/me/results/{result_id}\n  method: get\n  operationId: _get_result_detail_api_v1_users_me_results__result_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/me/results/{result_id}/dexa/scan-info\n  method: get\n  operationId: _get_dexa_scan_info_api_v1_users_me_results__result_id__dexa_scan_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/me/results/{result_id}/dexa/composition\n  method: get\n  operationId: _get_dexa_composition_api_v1_users_me_results__result_id__dexa_composition_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/me/results/{result_id}/dexa/bone-density\n  method: get\n  operationId: _get_dexa_bone_density_api_v1_users_me_results__result_id__dexa_bone_density_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/me/results/{result_id}/dexa/percentiles\n  method: get\n  operationId: _get_dexa_percentiles_api_v1_users_me_results__result_id__dexa_percentiles_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/users/me/results/{result_id}/dexa/visceral-fat\n  method: get\n  operationId: _get_dexa_visceral_fat_api_v1_users_me_results__result_id__dexa_visceral_fat_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/me/results/{result_id}/dexa/rmr\n  method: get\n  operationId: _get_dexa_rmr_api_v1_users_me_results__result_id__dexa_rmr_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/locations/{location_id}/availability\n  method: get\n  operationId: _get_availability_api_v1_locations__location_id__availability_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - email\n    - openid\n    - profile\n- path: /api/v1/locations/availability\n\
  \  method: get\n  operationId: _get_multi_availability_api_v1_locations_availability_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - email\n    - openid\n    - profile\n- path: /api/v1/locations\n  method: get\n  operationId: _list_locations_api_v1_locations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - email\n    - openid\n    - profile\n- path: /api/v1/locations/{location_id}\n  method: get\n  operationId: _get_location_api_v1_locations__location_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - email\n    - openid\n    - profile\n- path: /api/v1/services\n  method: get\n  operationId: _list_services_api_v1_services_get\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - email\n    - openid\n    - profile\n- path: /api/v1/services/{service_id}\n  method: get\n  operationId: _get_service_api_v1_services__service_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - email\n    - openid\n    - profile\n- path: /api/v1/partners/{partner_id}/reservations\n  method: get\n  operationId: _list_partner_reservations_api_v1_partners__partner_id__reservations_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/reservations\n  method: post\n  operationId: _create_reservation_api_v1_partners__partner_id__reservations_post\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/partners/{partner_id}/reservations/{appt_id}\n  method: get\n  operationId: _get_partner_reservation_api_v1_partners__partner_id__reservations__appt_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/reservations/{appt_id}\n  method: delete\n  operationId: _cancel_reservation_api_v1_partners__partner_id__reservations__appt_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1/partners/{partner_id}/users\n  method: get\n  operationId: _list_partner_users_api_v1_partners__partner_id__users_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/users/{user_id}/appts\n  method: get\n  operationId: _list_partner_user_appointments_api_v1_partners__partner_id__users__user_id__appts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/users/{user_id}/results\n  method: get\n  operationId: _list_partner_user_results_api_v1_partners__partner_id__users__user_id__results_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/users/{user_id}/results/{result_id}\n\
  \  method: get\n  operationId: _get_partner_user_result_detail_api_v1_partners__partner_id__users__user_id__results__result_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/users/{user_id}/results/{result_id}/export\n  method: post\n  operationId: _create_partner_user_result_export_api_v1_partners__partner_id__users__user_id__results__result_id__export_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/partners/{partner_id}/users/{user_id}/results/{result_id}/dexa/composition\n  method: get\n  operationId: _get_partner_dexa_composition_api_v1_partners__partner_id__users__user_id__results__result_id__dexa_composition_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/users/{user_id}/results/{result_id}/dexa/bone-density\n  method: get\n  operationId: _get_partner_dexa_bone_density_api_v1_partners__partner_id__users__user_id__results__result_id__dexa_bone_density_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/users/{user_id}/results/{result_id}/dexa/percentiles\n  method: get\n  operationId: _get_partner_dexa_percentiles_api_v1_partners__partner_id__users__user_id__results__result_id__dexa_percentiles_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/users/{user_id}/results/{result_id}/dexa/visceral-fat\n\
  \  method: get\n  operationId: _get_partner_dexa_visceral_fat_api_v1_partners__partner_id__users__user_id__results__result_id__dexa_visceral_fat_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/users/{user_id}/results/{result_id}/dexa/rmr\n  method: get\n  operationId: _get_partner_dexa_rmr_api_v1_partners__partner_id__users__user_id__results__result_id__dexa_rmr_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/users/{user_id}/results/{result_id}/dexa/scan-info\n  method: get\n  operationId: _get_partner_dexa_scan_info_api_v1_partners__partner_id__users__user_id__results__result_id__dexa_scan_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/users/{user_id}/intake\n  method: post\n  operationId: _create_intake_api_v1_partners__partner_id__users__user_id__intake_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/partners/{partner_id}/orders\n  method: post\n  operationId: _create_order_api_v1_partners__partner_id__orders_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/partners/{partner_id}/orders\n  method:\
  \ get\n  operationId: _list_orders_api_v1_partners__partner_id__orders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/orders/{order_id}\n  method: get\n  operationId: _get_order_api_v1_partners__partner_id__orders__order_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/orders/{order_id}\n  method: patch\n  operationId: _update_order_api_v1_partners__partner_id__orders__order_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/partners/{partner_id}/webhooks\n  method: get\n  operationId: list_webhooks_api_v1_partners__partner_id__webhooks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/partners/{partner_id}/webhooks\n  method: post\n  operationId: create_webhook_api_v1_partners__partner_id__webhooks_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/partners/{partner_id}/webhooks/{webhook_id}\n  method: get\n  operationId: get_webhook_api_v1_partners__partner_id__webhooks__webhook_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/partners/{partner_id}/webhooks/{webhook_id}\n  method: patch\n  operationId: update_webhook_api_v1_partners__partner_id__webhooks__webhook_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/partners/{partner_id}/webhooks/{webhook_id}\n  method: delete\n  operationId: delete_webhook_api_v1_partners__partner_id__webhooks__webhook_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bodyspec/refs/heads/main/agentic-access/bodyspec-agentic-access.yml
summary_line: 45 operations · 10 acting
tags:
- Company
- Health
- Fitness
- API
- Data
---
