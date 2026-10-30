---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 13
api_specs:
- filename: clayhr-agents-api-openapi.yml
  format: yaml
  label: ClayHR Agents API
  slug: clayhr-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clayhr/refs/heads/main/openapi/clayhr-agents-api-openapi.yml
- filename: clayhr-auth-api-openapi.yml
  format: yaml
  label: ClayHR Auth API
  slug: clayhr-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clayhr/refs/heads/main/openapi/clayhr-auth-api-openapi.yml
- filename: clayhr-documents-api-openapi.yml
  format: yaml
  label: ClayHR Documents API
  slug: clayhr-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clayhr/refs/heads/main/openapi/clayhr-documents-api-openapi.yml
- filename: clayhr-leads-api-openapi.yml
  format: yaml
  label: ClayHR Leads API
  slug: clayhr-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clayhr/refs/heads/main/openapi/clayhr-leads-api-openapi.yml
- filename: clayhr-system-api-openapi.yml
  format: yaml
  label: ClayHR System API
  slug: clayhr-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clayhr/refs/heads/main/openapi/clayhr-system-api-openapi.yml
- filename: clayhr-tickets-api-openapi.yml
  format: yaml
  label: ClayHR Tickets API
  slug: clayhr-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clayhr/refs/heads/main/openapi/clayhr-tickets-api-openapi.yml
- filename: clayhr-widget-api-openapi.yml
  format: yaml
  label: ClayHR Widget API
  slug: clayhr-widget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clayhr/refs/heads/main/openapi/clayhr-widget-api-openapi.yml
consequence_counts:
  read: 13
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clayhr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'ClayHR exposes 30 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ClayHR
provider_slug: clayhr
slug: clayhr-agentic-access
source_filename: clayhr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 13\n    acting: 17\n  by_consequence:\n    read: 13\n    write: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /api/auth/google/login\n  method: get\n  operationId: google_login_api_auth_google_login_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/google/callback\n  method: get\n  operationId: google_callback_api_auth_google_callback_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/auth/me\n  method: get\n  operationId: me_api_auth_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/logout\n  method: post\n  operationId: logout_api_auth_logout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/tools/catalog\n  method: get\n  operationId: tool_catalog_api_agents_tools_catalog_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: get\n  operationId: list_agents_api_agents_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents\n  method: post\n  operationId: create_agent_api_agents_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agent_id}\n  method: get\n  operationId: get_agent_api_agents__agent_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/{agent_id}\n  method: patch\n  operationId: update_agent_api_agents__agent_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agent_id}\n  method: delete\n  operationId: delete_agent_api_agents__agent_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agent_id}/widget\n  method: put\n  operationId: update_widget_api_agents__agent_id__widget_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agent_id}/tools\n  method: put\n  operationId: upsert_tool_api_agents__agent_id__tools_put\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agent_id}/domains\n  method: get\n  operationId: list_domains_api_agents__agent_id__domains_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/{agent_id}/domains\n  method: post\n  operationId: add_domain_api_agents__agent_id__domains_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agent_id}/domains/{domain_id}\n  method: delete\n  operationId: remove_domain_api_agents__agent_id__domains__domain_id__delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agent_id}/documents\n  method: get\n  operationId: list_documents_api_agents__agent_id__documents_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/{agent_id}/documents/file\n  method: post\n  operationId: upload_file_api_agents__agent_id__documents_file_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agent_id}/documents/website\n\
  \  method: post\n  operationId: add_website_api_agents__agent_id__documents_website_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agent_id}/documents/text\n  method: post\n  operationId: add_text_api_agents__agent_id__documents_text_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agent_id}/documents/{document_id}/reingest\n  method: post\n  operationId: reingest_api_agents__agent_id__documents__document_id__reingest_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agent_id}/documents/{document_id}\n  method: delete\n  operationId: delete_document_api_agents__agent_id__documents__document_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agent_id}/tickets\n  method: get\n  operationId: list_tickets_api_agents__agent_id__tickets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/{agent_id}/tickets/{ticket_id}\n  method: patch\n  operationId: update_ticket_api_agents__agent_id__tickets__ticket_id__patch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/{agent_id}/leads\n  method: get\n  operationId: list_leads_api_agents__agent_id__leads_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/{agent_id}/leads/{lead_id}\n  method: patch\n  operationId: update_lead_api_agents__agent_id__leads__lead_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/assets/{key}\n  method: get\n  operationId:\
  \ get_asset_api_assets__key__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/widget/bootstrap\n  method: get\n  operationId: widget_bootstrap_api_widget_bootstrap_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/chat\n  method: post\n  operationId: chat_api_chat_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/chat/close\n  method: post\n  operationId: close_conversation_api_chat_close_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clayhr/refs/heads/main/agentic-access/clayhr-agentic-access.yml
summary_line: 30 operations · 17 acting
tags:
- HR
- SaaS
- Cloud
- Human Capital Management
- Recruiting
- Company
---
