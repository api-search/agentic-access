---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 14
api_specs:
- filename: geocitation-openapi.json
  format: json
  label: GEOCitation Audit API
  slug: geocitation-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/openapi/geocitation-openapi.json
consequence_counts:
  read: 14
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Geocitation Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'GEOCitation exposes 17 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GEOCitation
provider_slug: geocitation
slug: geocitation-agentic-access
source_filename: geocitation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: generated\nsource: openapi/geocitation-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 3\n    connected: 14\n  by_consequence:\n    write: 3\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/audits\n  method: post\n  operationId: create_audit_v1_audits_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audits\n  method: get\n  operationId: list_audits_v1_audits_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audits/{audit_id}/stream\n  method: get\n  operationId: stream_audit_v1_audits__audit_id__stream_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audits/{audit_id}/status\n  method: get\n  operationId: get_audit_status_v1_audits__audit_id__status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audits/{audit_id}/events\n  method: get\n  operationId: list_audit_events_v1_audits__audit_id__events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audits/{audit_id}/retry-doc/{doc_slot}\n  method: post\n  operationId: retry_doc_node_v1_audits__audit_id__retry_doc__doc_slot__post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/audits/{audit_id}\n  method: get\n  operationId: get_audit_v1_audits__audit_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audits/{audit_id}/documents/{doc_type}\n  method: get\n  operationId: get_document_v1_audits__audit_id__documents__doc_type__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audits/{audit_id}/manifest\n  method: get\n  operationId: get_manifest_v1_audits__audit_id__manifest_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: read_usage_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meta/kpi-catalog\n  method: get\n  operationId: get_kpi_catalog_v1_meta_kpi_catalog_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meta/icp-priority/{icp_key}\n  method: get\n  operationId: get_icp_priority_v1_meta_icp_priority__icp_key__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/meta/branding\n  method: get\n  operationId: get_branding_v1_meta_branding_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/opt-out\n  method: post\n  operationId: create_opt_out_v1_opt_out_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/opt-out\n  method: get\n  operationId: list_opt_outs_v1_opt_out_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/detailed\n  method: get\n  operationId: health_detailed_health_detailed_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geocitation/refs/heads/main/agentic-access/geocitation-agentic-access.yml
summary_line: 17 operations · 3 acting
tags:
- SEO
- GEO
- AEO
- AI Search Visibility
- Content Intelligence
- Competitive Intelligence
- Marketing
- MarTech
- White-label
- Agency Tooling
- Web Data & Analytics
---
