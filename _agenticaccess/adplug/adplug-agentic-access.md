---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 20
api_specs:
- filename: adplug-health-api-openapi.yml
  format: yaml
  label: AdPlug Health API
  slug: adplug-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-health-api-openapi.yml
- filename: adplug-mcp-api-openapi.yml
  format: yaml
  label: AdPlug MCP API
  slug: adplug-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-mcp-api-openapi.yml
- filename: adplug-oauth-api-openapi.yml
  format: yaml
  label: AdPlug OAuth API
  slug: adplug-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-oauth-api-openapi.yml
- filename: adplug-oauth-legacy-compat-api-openapi.yml
  format: yaml
  label: AdPlug OAUTH Legacy Compat API
  slug: adplug-oauth-legacy-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-oauth-legacy-compat-api-openapi.yml
- filename: adplug-users-api-openapi.yml
  format: yaml
  label: AdPlug Users API
  slug: adplug-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-users-api-openapi.yml
- filename: adplug-webhooks-api-openapi.yml
  format: yaml
  label: AdPlug Webhooks API
  slug: adplug-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 20
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Adplug Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/users/{user_id}/checkout-opened
operation_count: 35
overview: 'AdPlug exposes 35 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 14 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AdPlug
provider_slug: adplug
slug: adplug-agentic-access
source_filename: adplug-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: generated\nsource: openapi/adplug.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 20\n    acting: 15\n  by_consequence:\n    read: 20\n    write: 14\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/google-ads/authorize\n  method: get\n  operationId: authorize_oauth_google_ads_authorize_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/google-ads/callback\n  method: get\n  operationId: callback_oauth_google_ads_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/linkedin-ads/authorize\n  method: get\n  operationId: authorize_oauth_linkedin_ads_authorize_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/linkedin-ads/callback\n  method: get\n  operationId: callback_oauth_linkedin_ads_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/microsoft-ads/authorize\n  method: get\n  operationId: authorize_oauth_microsoft_ads_authorize_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/microsoft-ads/callback\n  method: get\n  operationId: callback_oauth_microsoft_ads_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/meta-ads/authorize\n  method: get\n  operationId: authorize_oauth_meta_ads_authorize_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/meta-ads/callback\n  method: get\n  operationId: callback_oauth_meta_ads_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meta/data-deletion\n  method: post\n  operationId: data_deletion_meta_data_deletion_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/hubspot/authorize\n  method:\
  \ get\n  operationId: authorize_oauth_hubspot_authorize_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/hubspot/callback\n  method: get\n  operationId: callback_oauth_hubspot_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/google-search-console/authorize\n  method: get\n  operationId: authorize_oauth_google_search_console_authorize_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/google-search-console/callback\n  method: get\n  operationId: callback_oauth_google_search_console_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /webhooks/paddle-sandbox\n  method: post\n  operationId: paddle_webhook_sandbox_webhooks_paddle_sandbox_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/paddle-live\n  method: post\n  operationId: paddle_webhook_live_webhooks_paddle_live_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorize\n  method: get\n  operationId: authorize_passthrough_authorize_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /token\n  method: post\n  operationId: token_passthrough_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /register\n  method: post\n  operationId: register_passthrough_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/{mcp_token}/info\n  method: get\n  operationId:\
  \ mcp_info_mcp__mcp_token__info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/{user_id}/profile\n  method: get\n  operationId: get_user_profile_api_users__user_id__profile_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/{user_id}/connections\n  method: get\n  operationId: get_user_connections_api_users__user_id__connections_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/{user_id}/checkout-opened\n  method: post\n  operationId: checkout_opened_api_users__user_id__checkout_opened_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/{user_id}/usage\n  method: get\n  operationId: get_user_usage_api_users__user_id__usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/{user_id}/connections/{platform}\n  method: delete\n  operationId: delete_user_connection_api_users__user_id__connections__platform__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/{user_id}/hubspot-portals\n  method: get\n  operationId: get_hubspot_portals_api_users__user_id__hubspot_portals_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/{user_id}/hubspot-portals/{hub_id}\n  method: patch\n  operationId: rename_hubspot_portal_api_users__user_id__hubspot_portals__hub_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/{user_id}/hubspot-portals/{hub_id}\n  method: delete\n  operationId: delete_hubspot_portal_api_users__user_id__hubspot_portals__hub_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/users/{user_id}\n  method: delete\n  operationId: delete_user_account_api_users__user_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/{user_id}/rotate-mcp-token\n  method: post\n  operationId: rotate_mcp_token_api_users__user_id__rotate_mcp_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/{user_id}/paddle-sync-subscription\n  method: post\n  operationId: sync_paddle_subscription_api_users__user_id__paddle_sync_subscription_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/{user_id}/paddle-subscription\n  method: get\n  operationId: get_paddle_subscription_api_users__user_id__paddle_subscription_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/users/{user_id}/paddle-portal-session\n  method: post\n  operationId: create_paddle_portal_session_api_users__user_id__paddle_portal_session_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/{user_id}/paddle-change-plan\n\
  \  method: post\n  operationId: paddle_change_plan_api_users__user_id__paddle_change_plan_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/users/{user_id}/paddle-cancel-current-sub\n  method: post\n  operationId: paddle_cancel_current_sub_api_users__user_id__paddle_cancel_current_sub_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/agentic-access/adplug-agentic-access.yml
summary_line: 35 operations · 15 acting
tags:
- PPC
- AI Integration
- Agency Tools
- Search Console
---
