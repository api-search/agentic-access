---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 26
api_specs:
- filename: tender-agents-com-agent-discovery-api-openapi.yml
  format: yaml
  label: tender-agents-com Agent Discovery API
  slug: tender-agents-com-agent-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-agent-discovery-api-openapi.yml
- filename: tender-agents-com-erp-export-api-openapi.yml
  format: yaml
  label: tender-agents-com ERP Export API
  slug: tender-agents-com-erp-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-erp-export-api-openapi.yml
- filename: tender-agents-com-gaeb-api-openapi.yml
  format: yaml
  label: tender-agents-com Gaeb API
  slug: tender-agents-com-gaeb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-gaeb-api-openapi.yml
- filename: tender-agents-com-keys-api-openapi.yml
  format: yaml
  label: tender-agents-com Keys API
  slug: tender-agents-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-keys-api-openapi.yml
- filename: tender-agents-com-mcp-api-openapi.yml
  format: yaml
  label: tender-agents-com MCP API
  slug: tender-agents-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-mcp-api-openapi.yml
- filename: tender-agents-com-oauth-api-openapi.yml
  format: yaml
  label: tender-agents-com OAuth API
  slug: tender-agents-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-oauth-api-openapi.yml
- filename: tender-agents-com-profiles-api-openapi.yml
  format: yaml
  label: tender-agents-com Profiles API
  slug: tender-agents-com-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-profiles-api-openapi.yml
- filename: tender-agents-com-signup-api-openapi.yml
  format: yaml
  label: tender-agents-com Signup API
  slug: tender-agents-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-signup-api-openapi.yml
- filename: tender-agents-com-source-status-api-openapi.yml
  format: yaml
  label: tender-agents-com Source Status API
  slug: tender-agents-com-source-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-source-status-api-openapi.yml
- filename: tender-agents-com-tenders-api-openapi.yml
  format: yaml
  label: tender-agents-com Tenders API
  slug: tender-agents-com-tenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-tenders-api-openapi.yml
- filename: tender-agents-com-tenders-public-api-openapi.yml
  format: yaml
  label: tender-agents-com Tenders Public API
  slug: tender-agents-com-tenders-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-tenders-public-api-openapi.yml
- filename: tender-agents-com-webhooks-api-openapi.yml
  format: yaml
  label: tender-agents-com Webhooks API
  slug: tender-agents-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-webhooks-api-openapi.yml
consequence_counts:
  read: 26
  safety-critical: 1
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Tender Agents Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/me/keys/{key_id}
operation_count: 45
overview: 'tender-agents-com exposes 45 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 18 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tender-agents-com
provider_slug: tender-agents-com
slug: tender-agents-com-agentic-access
source_filename: tender-agents-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/tender-agents-com-agentleads-openapi.json, openapi/tender-agents-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 45\n  by_action_class:\n    connected: 26\n    acting: 19\n  by_consequence:\n    read: 26\n    write: 18\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/health\n  method: get\n  operationId: health_api_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/source-status\n  method: get\n  operationId: source_status_api_v1_source_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/cpv\n  method: get\n  operationId: cpv_list_api_v1_cpv_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/countries\n  method: get\n  operationId: public_countries_api_v1_public_countries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/tenders/document-watches\n  method: post\n  operationId: watch_public_tender_documents_api_v1_public_tenders_document_watches_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/public/tenders\n\
  \  method: get\n  operationId: public_tenders_api_v1_public_tenders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tenders\n  method: get\n  operationId: list_tenders_api_v1_tenders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenders:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tenders/search\n  method: get\n  operationId: fts_search_api_v1_tenders_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenders:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tenders/{tender_id}\n  method: get\n  operationId: get_tender_by_id_api_v1_tenders__tender_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenders:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stats\n  method: get\n  operationId: stats_api_v1_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenders:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/company-profiles\n  method: post\n  operationId: create_public_company_profile_api_v1_public_company_profiles_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/company-profiles/{profile_id}\n  method: get\n  operationId: get_company_profile_api_v1_company_profiles__profile_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - profiles:read\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/company-profiles/{profile_id}/export\n  method: get\n  operationId: export_public_company_profile_api_v1_public_company_profiles__profile_id__export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/company-profiles/{profile_id}\n  method: delete\n  operationId: delete_public_company_profile_api_v1_public_company_profiles__profile_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/public/company-profiles/{profile_id}/matches\n  method: get\n  operationId: public_company_profile_matches_api_v1_public_company_profiles__profile_id__matches_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pilot/{profile_id}/{access_token}/matches\n  method: get\n  operationId: protected_pilot_matches_api_v1_pilot__profile_id___access_token__matches_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pilot/{profile_id}/{access_token}/tenders/{tender_id}\n  method: put\n  operationId: update_pilot_tender_state_api_v1_pilot__profile_id___access_token__tenders__tender_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pilot/{profile_id}/{access_token}/digest\n  method: post\n  operationId: run_pilot_digest_api_v1_pilot__profile_id___access_token__digest_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pilot/{profile_id}/{access_token}/gaeb/analyze\n  method: post\n  operationId: analyze_gaeb_upload_api_v1_pilot__profile_id___access_token__gaeb_analyze_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pilot/{profile_id}/{access_token}/gaeb/export\n  method: post\n  operationId: export_gaeb_upload_api_v1_pilot__profile_id___access_token__gaeb_export_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pilot/{profile_id}/{access_token}/tenders/{tender_id}/export\n  method: get\n  operationId: export_tender_api_v1_pilot__profile_id___access_token__tenders__tender_id__export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pilot/{profile_id}/{access_token}/tenders/{tender_id}/erp-webhook\n  method: post\n  operationId: deliver_tender_to_erp_webhook_api_v1_pilot__profile_id___access_token__tenders__tender_id__erp_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/me/keys\n  method: get\n  operationId: list_api_keys_api_v1_me_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/keys\n  method: post\n  operationId: create_api_key_api_v1_me_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/keys/{key_id}\n  method: delete\n  operationId: revoke_api_key_api_v1_me_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n \
  \     human-in-the-loop: required\n    audit: required\n- path: /api/v1/me/webhooks\n  method: get\n  operationId: list_webhooks_api_v1_me_webhooks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me/webhooks\n  method: post\n  operationId: create_webhook_api_v1_me_webhooks_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me/webhooks/{webhook_id}\n  method: delete\n  operationId: delete_webhook_api_v1_me_webhooks__webhook_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signup\n  method: post\n  operationId: signup_api_v1_signup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/standard\n  method: get\n  operationId: agent_standard_api_standard_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/glama.json\n  method: get\n  operationId: glama_connector_claim__well_known_glama_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: agent_card__well_known_agent_card_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: llms_txt_llms_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /server.json\n  method: get\n  operationId: mcp_server_json_server_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/a2a\n  method: post\n  operationId: a2a_jsonrpc_api_a2a_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/mcp/server-card.json\n  method: get\n  operationId: mcp_server_card__well_known_mcp_server_card_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcp_endpoint_mcp_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - fulltext:read\n    - tenders:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/open-data\n  method: post\n  operationId: mcp_open_data_endpoint_mcp_open_data_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/token\n  method: post\n  operationId: token_oauth_token_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: authorization_server_metadata__well_known_oauth_authorization_server_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: protected_resource_metadata__well_known_oauth_protected_resource_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tenders-public\n  method: get\n  operationId: searchTenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/source-status\n  method: get\n  operationId: sourceStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/signup\n  method: post\n  operationId: signupFree\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/tender-agents-com/agentic-access/tender-agents-com-agentic-access.yml
summary_line: 45 operations · 19 acting · 1 human-in-the-loop
tags:
- EU
- Procurement
- Tenders
- Artificial Intelligence
- Public Data
---
