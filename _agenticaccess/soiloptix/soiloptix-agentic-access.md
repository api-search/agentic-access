---
acting_count: 38
action_class_counts:
  acting: 38
  connected: 47
api_specs:
- filename: soiloptix-analyses-billable-api-openapi.yml
  format: yaml
  label: SoilOptix Analyses - Billable API
  slug: soiloptix-analyses-billable-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-analyses-billable-api-openapi.yml
- filename: soiloptix-analyses-read-api-openapi.yml
  format: yaml
  label: SoilOptix Analyses - Read API
  slug: soiloptix-analyses-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-analyses-read-api-openapi.yml
- filename: soiloptix-authentication-api-openapi.yml
  format: yaml
  label: SoilOptix Authentication API
  slug: soiloptix-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-authentication-api-openapi.yml
- filename: soiloptix-businesses-api-openapi.yml
  format: yaml
  label: SoilOptix Businesses API
  slug: soiloptix-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-businesses-api-openapi.yml
- filename: soiloptix-countries-api-openapi.yml
  format: yaml
  label: SoilOptix Countries API
  slug: soiloptix-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-countries-api-openapi.yml
- filename: soiloptix-farms-api-openapi.yml
  format: yaml
  label: SoilOptix Farms API
  slug: soiloptix-farms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-farms-api-openapi.yml
- filename: soiloptix-fields-api-openapi.yml
  format: yaml
  label: SoilOptix Fields API
  slug: soiloptix-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-fields-api-openapi.yml
- filename: soiloptix-my-account-api-openapi.yml
  format: yaml
  label: SoilOptix My Account API
  slug: soiloptix-my-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-my-account-api-openapi.yml
- filename: soiloptix-v3-boundaries-api-openapi.yml
  format: yaml
  label: SoilOptix v3 - Boundaries API
  slug: soiloptix-v3-boundaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-v3-boundaries-api-openapi.yml
- filename: soiloptix-v3-customers-api-openapi.yml
  format: yaml
  label: SoilOptix v3 - Customers API
  slug: soiloptix-v3-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-v3-customers-api-openapi.yml
- filename: soiloptix-v3-farms-api-openapi.yml
  format: yaml
  label: SoilOptix v3 - Farms API
  slug: soiloptix-v3-farms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-v3-farms-api-openapi.yml
- filename: soiloptix-v3-fields-api-openapi.yml
  format: yaml
  label: SoilOptix v3 - Fields API
  slug: soiloptix-v3-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-v3-fields-api-openapi.yml
- filename: soiloptix-v3-identity-api-openapi.yml
  format: yaml
  label: SoilOptix v3 - Identity API
  slug: soiloptix-v3-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-v3-identity-api-openapi.yml
- filename: soiloptix-v3-sets-api-openapi.yml
  format: yaml
  label: SoilOptix v3 - Sets API
  slug: soiloptix-v3-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soiloptix/openapi/soiloptix-v3-sets-api-openapi.yml
consequence_counts:
  physical: 6
  read: 47
  safety-critical: 2
  write: 30
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Soiloptix Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/auth/resetForgottenPassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v4/auth/resetPassword
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v4/businesses/{business_id}/children/{child_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v4/businesses/{business_id}/children/{child_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v4/businesses/{business_id}/customers/{customer_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v4/businesses/{business_id}/customers/{customer_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v4/myaccount/businesses/{business_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v4/myaccount/businesses/{business_id}
operation_count: 85
overview: 'SoilOptix exposes 85 API operations that an AI agent could call, of which 38 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 47 read, 30 write, 6 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SoilOptix
provider_slug: soiloptix
slug: soiloptix-agentic-access
source_filename: soiloptix-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/soiloptix-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 85\n  by_action_class:\n    acting: 38\n    connected: 47\n  by_consequence:\n    write: 30\n    safety-critical: 2\n    read: 47\n    physical: 6\n  human_in_the_loop_required: 2\noperations:\n- path: /api/v4/auth/token\n  method: post\n  operationId: login_direct_flow_api_v4_auth_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/auth/refresh\n  method: post\n \
  \ operationId: refresh_api_v4_auth_refresh_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/auth/resetPassword\n  method: post\n  operationId: reset_password_api_v4_auth_resetPassword_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v4/auth/forgotPassword\n  method: get\n  operationId: forgot_password_api_v4_auth_forgotPassword_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /api/v4/auth/resetForgottenPassword\n  method: post\n  operationId: reset_forgotten_password_api_v4_auth_resetForgottenPassword_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v4/auth/registerUser\n  method: post\n  operationId: register_user_api_v4_auth_registerUser_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/myaccount\n  method: get\n  operationId: get_account_information_api_v4_myaccount_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/myaccount\n  method: patch\n  operationId: update_my_account_api_v4_myaccount_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/myaccount/businesses/\n  method: get\n  operationId: get_business_relationships_api_v4_myaccount_businesses__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/myaccount/businesses/{business_id}\n  method: patch\n  operationId: update_business_relationship_api_v4_myaccount_businesses__business_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/myaccount/businesses/{business_id}\n  method: delete\n  operationId: remove_business_relationship_api_v4_myaccount_businesses__business_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/myaccount/invites/\n  method: get\n  operationId: get_my_invites_api_v4_myaccount_invites__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /api/v4/myaccount/invites/{invite_id}\n  method: post\n  operationId: accept_invite_api_v4_myaccount_invites__invite_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/myaccount/invites/{invite_id}\n  method: delete\n  operationId: decline_invite_api_v4_myaccount_invites__invite_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/myaccount/notifications/\n  method: get\n  operationId: get_notifications_api_v4_myaccount_notifications__get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/myaccount/terms_and_conditions/\n  method: post\n  operationId: agree_to_terms_and_conditions_api_v4_myaccount_terms_and_conditions__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/businesses/\n  method: get\n  operationId: get_businesses_api_v4_businesses__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/businesses/\n  method: post\n  operationId: create_business_api_v4_businesses__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/businesses/{business_id}\n  method: get\n  operationId: get_business_api_v4_businesses__business_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/businesses/{business_id}\n  method: patch\n  operationId: update_business_api_v4_businesses__business_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/businesses/{business_id}\n  method: delete\n  operationId: delete_business_api_v4_businesses__business_id__delete\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/businesses/{business_id}/customers/{customer_id}\n  method: delete\n  operationId: remove_customer_business_relationship_api_v4_businesses__business_id__customers__customer_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/businesses/{business_id}/customers/{customer_id}\n  method: patch\n  operationId: modify_customer_business_relationship_api_v4_businesses__business_id__customers__customer_id__patch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/businesses/{business_id}/invites/\n  method: get\n  operationId: get_invites_api_v4_businesses__business_id__invites__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/businesses/{business_id}/invites/\n  method: post\n  operationId: create_invite_api_v4_businesses__business_id__invites__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v4/businesses/{business_id}/invites/{invite_id}\n  method: get\n  operationId: get_invite_api_v4_businesses__business_id__invites__invite_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/businesses/{business_id}/invites/{invite_id}\n  method: patch\n  operationId: update_invite_api_v4_businesses__business_id__invites__invite_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/businesses/{business_id}/invites/{invite_id}\n  method: delete\n  operationId: delete_invite_api_v4_businesses__business_id__invites__invite_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/businesses/{business_id}/children/{child_id}\n  method: put\n  operationId: add_child_business_relationship_by_id_api_v4_businesses__business_id__children__child_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/businesses/{business_id}/children/{child_id}\n  method: delete\n  operationId: remove_child_business_relationship_by_id_api_v4_businesses__business_id__children__child_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/farms/\n  method: get\n  operationId: get_farms_api_v4_farms__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/farms/\n  method: post\n  operationId: create_farm_api_v4_farms__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/farms/{farm_id}\n  method: get\n  operationId: get_farm_by_id_api_v4_farms__farm_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/farms/{farm_id}\n  method: patch\n  operationId: update_farm_api_v4_farms__farm_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/farms/{farm_id}\n  method: delete\n  operationId: delete_farm_api_v4_farms__farm_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/fields/\n  method: get\n  operationId: get_fields_api_v4_fields__get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/fields/\n  method: post\n  operationId: create_field_api_v4_fields__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/fields/{field_id}\n  method: get\n  operationId: get_field_api_v4_fields__field_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/fields/{field_id}\n  method: patch\n  operationId: update_field_api_v4_fields__field_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/fields/{field_id}\n  method: delete\n  operationId: delete_field_api_v4_fields__field_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/analyses/\n  method: get\n  operationId: get_analyses_api_v4_analyses__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/\n  method: post\n  operationId: create_analysis_api_v4_analyses__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/analyses/{analysis_id}\n  method: patch\n  operationId: update_analysis_api_v4_analyses__analysis_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/analyses/{analysis_id}\n  method: get\n  operationId: get_analysis_by_id_api_v4_analyses__analysis_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/models/\n  method: get\n  operationId: get_analysis_models_api_v4_analyses__analysis_id__models__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/models/{model_id}/geojson\n  method: get\n  operationId: get_analysis_model_regression_heatmap_api_v4_analyses__analysis_id__models__model_id__geojson_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/samplePoints\n  method: get\n  operationId: get_sample_point_locations_by_analysis_id_api_v4_analyses__analysis_id__samplePoints_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/files\n  method: get\n  operationId: list_all_files_in_analysis_api_v4_analyses__analysis_id__files_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/files/{subfolder}\n\
  \  method: get\n  operationId: list_files_in_analysis_api_v4_analyses__analysis_id__files__subfolder__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/files/{subfolder}/{filename}\n  method: get\n  operationId: download_analysis_file_api_v4_analyses__analysis_id__files__subfolder___filename__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/files/{subfolder}/{filename}\n  method: delete\n  operationId: delete_raw_upload_file_api_v4_analyses__analysis_id__files__subfolder___filename__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/analyses/{analysis_id}/boundary\n  method: post\n  operationId: save_boundary_wkt_api_v4_analyses__analysis_id__boundary_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/analyses/{analysis_id}/packages\n  method: patch\n  operationId: select_packages_api_v4_analyses__analysis_id__packages_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/analyses/{analysis_id}/submit\n  method: put\n  operationId: submit_analysis_api_v4_analyses__analysis_id__submit_put\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/analyses/{analysis_id}/files/upload/\n  method: post\n  operationId: tus_upload_docs_api_v4_analyses__analysis_id__files_upload__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/analyses/{analysis_id}/messages/\n  method: get\n  operationId: get_messages_api_v4_analyses__analysis_id__messages__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/messages/\n\
  \  method: post\n  operationId: create_message_api_v4_analyses__analysis_id__messages__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/analyses/{analysis_id}/messages/{message_id}/read\n  method: put\n  operationId: mark_as_read_api_v4_analyses__analysis_id__messages__message_id__read_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/analyses/{analysis_id}/exports/\n  method: get\n  operationId: get_analysis_exports_api_v4_analyses__analysis_id__exports__get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/exports/csv\n  method: get\n  operationId: get_regression_csv_api_v4_analyses__analysis_id__exports_csv_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/exports/shp\n  method: get\n  operationId: get_shp_export_api_v4_analyses__analysis_id__exports_shp_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/exports/pdf\n  method: get\n  operationId: get_pdf_export_api_v4_analyses__analysis_id__exports_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/exports/tif\n\
  \  method: get\n  operationId: get_tif_zip_export_api_v4_analyses__analysis_id__exports_tif_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/exports/lab\n  method: get\n  operationId: get_sample_points_export_api_v4_analyses__analysis_id__exports_lab_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/analyses/{analysis_id}/exports/bnd\n  method: get\n  operationId: export_boundary_by_id_api_v4_analyses__analysis_id__exports_bnd_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/countries/\n  method: get\n  operationId: get_countries_api_v4_countries__get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/login\n  method: post\n  operationId: login_direct_flow_api_v3_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/refresh\n  method: post\n  operationId: refresh_api_v3_refresh_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v3/boundaries/\n  method: get\n  operationId: get_boundaries_api_v3_boundaries__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/boundaries/{boundary_id}\n  method: get\n  operationId: get_boundary_by_id_api_v3_boundaries__boundary_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/customers/\n  method: get\n  operationId: get_customers_api_v3_customers__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/customers/{customer_id}\n  method: get\n  operationId: get_customer_by_id_api_v3_customers__customer_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/customers/{customer_id}/farms\n  method: get\n  operationId: get_farms_by_customer_id_api_v3_customers__customer_id__farms_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/farms/\n  method: get\n  operationId: get_farms_api_v3_farms__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/farms/{farm_id}\n  method: get\n  operationId: get_farm_by_id_api_v3_farms__farm_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/farms/{farm_id}/fields\n  method: get\n  operationId: get_fields_by_farm_id_api_v3_farms__farm_id__fields_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/fields/\n  method: get\n  operationId: get_fields_api_v3_fields__get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/fields/{field_id}\n  method: get\n  operationId: get_field_by_id_api_v3_fields__field_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/fields/{field_id}/sets\n  method: get\n  operationId: get_sets_by_field_id_api_v3_fields__field_id__sets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/sets/\n  method: get\n  operationId: get_sets_api_v3_sets__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/sets/{set_id}\n  method: get\n  operationId: get_set_by_id_api_v3_sets__set_id__get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/sets/{set_id}/points\n  method: get\n  operationId: get_points_by_set_id_api_v3_sets__set_id__points_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/sets/{set_id}/points/{column_index}\n  method: get\n  operationId: get_points_by_set_id_column_specific_api_v3_sets__set_id__points__column_index__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/sets/{set_id}/shapefile\n  method: get\n  operationId: get_shapefile_by_set_id_api_v3_sets__set_id__shapefile_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/sets/{set_id}/samples\n\
  \  method: get\n  operationId: get_samples_by_set_id_api_v3_sets__set_id__samples_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/soiloptix/agentic-access/soiloptix-agentic-access.yml
summary_line: 85 operations · 38 acting · 2 human-in-the-loop
tags:
- Agriculture
- Soil-Analysis
- Precision Agriculture
- Mapping
- Technology
---
