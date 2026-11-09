---
acting_count: 30
action_class_counts:
  acting: 30
  connected: 28
api_specs:
- filename: finedata-ai-api-keys-api-openapi.yml
  format: yaml
  label: finedata-ai API Keys API
  slug: finedata-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-api-keys-api-openapi.yml
- filename: finedata-ai-async-scraping-api-openapi.yml
  format: yaml
  label: finedata-ai Async Scraping API
  slug: finedata-ai-async-scraping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-async-scraping-api-openapi.yml
- filename: finedata-ai-google-serp-api-openapi.yml
  format: yaml
  label: finedata-ai Google SERP API
  slug: finedata-ai-google-serp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-google-serp-api-openapi.yml
- filename: finedata-ai-oauth-api-openapi.yml
  format: yaml
  label: finedata-ai OAuth API
  slug: finedata-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-oauth-api-openapi.yml
- filename: finedata-ai-plans-api-openapi.yml
  format: yaml
  label: finedata-ai Plans API
  slug: finedata-ai-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-plans-api-openapi.yml
- filename: finedata-ai-proxy-profiles-byop-api-openapi.yml
  format: yaml
  label: finedata-ai Proxy Profiles (BYOP) API
  slug: finedata-ai-proxy-profiles-byop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-proxy-profiles-byop-api-openapi.yml
- filename: finedata-ai-user-api-openapi.yml
  format: yaml
  label: finedata-ai User API
  slug: finedata-ai-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-user-api-openapi.yml
- filename: finedata-ai-user-statistics-api-openapi.yml
  format: yaml
  label: finedata-ai User Statistics API
  slug: finedata-ai-user-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-user-statistics-api-openapi.yml
- filename: finedata-ai-web-scraping-api-openapi.yml
  format: yaml
  label: finedata-ai Web Scraping API
  slug: finedata-ai-web-scraping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finedata-ai/openapi/finedata-ai-web-scraping-api-openapi.yml
consequence_counts:
  read: 28
  safety-critical: 4
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Finedata Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/api-keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/api-keys/{key_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /oauth/revoke
operation_count: 58
overview: 'finedata-ai exposes 58 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 26 write, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: finedata-ai
provider_slug: finedata-ai
slug: finedata-ai-agentic-access
source_filename: finedata-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/finedata-ai.json, openapi/finedata-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 58\n  by_action_class:\n    acting: 30\n    connected: 28\n  by_consequence:\n    write: 26\n    read: 28\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /api/v1/scrape\n  method: post\n  operationId: scrape_endpoint_api_v1_scrape_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/async/scrape\n  method: post\n  operationId:\
  \ create_async_job_api_v1_async_scrape_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/async/jobs/{job_id}\n  method: get\n  operationId: get_job_status_api_v1_async_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/async/jobs/{job_id}\n  method: delete\n  operationId: cancel_job_api_v1_async_jobs__job_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/async/jobs\n\
  \  method: get\n  operationId: list_jobs_api_v1_async_jobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/async/stats\n  method: get\n  operationId: get_job_stats_api_v1_async_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/async/batch\n  method: post\n  operationId: create_batch_job_api_v1_async_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/async/batch/{batch_id}\n  method: get\n  operationId: get_batch_status_api_v1_async_batch__batch_id__get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/api-keys\n  method: post\n  operationId: create_api_key_api_v1_api_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/api-keys\n  method: get\n  operationId: list_api_keys_api_v1_api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/api-keys/{key_id}\n  method: delete\n  operationId: revoke_api_key_api_v1_api_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/me\n  method: get\n  operationId: get_current_user_info_api_v1_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  operationId: get_usage_api_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/plans\n  method: get\n  operationId: get_plans_api_v1_plans_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/proxy-profiles\n  method: post\n  operationId: create_profile_api_v1_proxy_profiles_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/proxy-profiles\n  method: get\n  operationId: list_profiles_api_v1_proxy_profiles_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/proxy-profiles/{profile_id}\n  method: get\n  operationId: get_profile_api_v1_proxy_profiles__profile_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/proxy-profiles/{profile_id}\n  method: put\n  operationId: update_profile_api_v1_proxy_profiles__profile_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/proxy-profiles/{profile_id}\n  method: delete\n  operationId: delete_profile_api_v1_proxy_profiles__profile_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/proxy-profiles/{profile_id}/test\n  method: post\n  operationId: test_profile_api_v1_proxy_profiles__profile_id__test_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/serp\n  method:\
  \ post\n  operationId: serp_endpoint_api_v1_serp_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/user/stats\n  method: get\n  operationId: get_user_stats_api_v1_user_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: authorization_server_metadata__well_known_oauth_authorization_server_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/jwks.json\n  method: get\n  operationId: jwks__well_known_jwks_json_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/register\n  method: post\n  operationId: register_client_oauth_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/authorize\n  method: get\n  operationId: authorize_oauth_authorize_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/consent/approve\n  method: post\n  operationId: consent_approve_oauth_consent_approve_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: token_oauth_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/revoke\n  method: post\n  operationId: revoke_token_oauth_revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/scrape\n  method: post\n  operationId: scrape_endpoint_api_v1_scrape_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/async/scrape\n  method: post\n  operationId: create_async_job_api_v1_async_scrape_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/async/jobs/{job_id}\n  method: get\n  operationId: get_job_status_api_v1_async_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/async/jobs/{job_id}\n  method: delete\n  operationId: cancel_job_api_v1_async_jobs__job_id__delete\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/async/jobs\n  method: get\n  operationId: list_jobs_api_v1_async_jobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/async/stats\n  method: get\n  operationId: get_job_stats_api_v1_async_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/async/batch\n  method: post\n  operationId: create_batch_job_api_v1_async_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/async/batch/{batch_id}\n  method: get\n  operationId: get_batch_status_api_v1_async_batch__batch_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/api-keys\n  method: post\n  operationId: create_api_key_api_v1_api_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/api-keys\n  method: get\n  operationId: list_api_keys_api_v1_api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/api-keys/{key_id}\n\
  \  method: delete\n  operationId: revoke_api_key_api_v1_api_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/me\n  method: get\n  operationId: get_current_user_info_api_v1_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  operationId: get_usage_api_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/plans\n  method: get\n  operationId: get_plans_api_v1_plans_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/proxy-profiles\n  method: post\n  operationId: create_profile_api_v1_proxy_profiles_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/proxy-profiles\n  method: get\n  operationId: list_profiles_api_v1_proxy_profiles_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/proxy-profiles/{profile_id}\n  method: get\n  operationId: get_profile_api_v1_proxy_profiles__profile_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/proxy-profiles/{profile_id}\n\
  \  method: put\n  operationId: update_profile_api_v1_proxy_profiles__profile_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/proxy-profiles/{profile_id}\n  method: delete\n  operationId: delete_profile_api_v1_proxy_profiles__profile_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/proxy-profiles/{profile_id}/test\n  method: post\n  operationId: test_profile_api_v1_proxy_profiles__profile_id__test_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/serp\n  method: post\n  operationId: serp_endpoint_api_v1_serp_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/user/stats\n  method: get\n  operationId: get_user_stats_api_v1_user_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: authorization_server_metadata__well_known_oauth_authorization_server_get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/jwks.json\n  method: get\n  operationId: jwks__well_known_jwks_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/register\n  method: post\n  operationId: register_client_oauth_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/authorize\n  method: get\n  operationId: authorize_oauth_authorize_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/consent/approve\n  method: post\n  operationId:\
  \ consent_approve_oauth_consent_approve_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: token_oauth_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/revoke\n  method: post\n  operationId: revoke_token_oauth_revoke_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/finedata-ai/agentic-access/finedata-ai-agentic-access.yml
summary_line: 58 operations · 30 acting · 4 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- Web Scraping
- Data Extraction
- MCP
- LLM
---
