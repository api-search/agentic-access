---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 29
api_specs:
- filename: edgrapi-activist-api-openapi.yml
  format: yaml
  label: Paper and Beyond Activist API
  slug: edgrapi-activist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-activist-api-openapi.yml
- filename: edgrapi-events-api-openapi.yml
  format: yaml
  label: Paper and Beyond Events API
  slug: edgrapi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-events-api-openapi.yml
- filename: edgrapi-filings-api-openapi.yml
  format: yaml
  label: Paper and Beyond Filings API
  slug: edgrapi-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-filings-api-openapi.yml
- filename: edgrapi-fundamentals-api-openapi.yml
  format: yaml
  label: Paper and Beyond Fundamentals API
  slug: edgrapi-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-fundamentals-api-openapi.yml
- filename: edgrapi-government-api-openapi.yml
  format: yaml
  label: Paper and Beyond Government API
  slug: edgrapi-government-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-government-api-openapi.yml
- filename: edgrapi-holdings-api-openapi.yml
  format: yaml
  label: Paper and Beyond Holdings API
  slug: edgrapi-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-holdings-api-openapi.yml
- filename: edgrapi-insider-api-openapi.yml
  format: yaml
  label: Paper and Beyond Insider API
  slug: edgrapi-insider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-insider-api-openapi.yml
- filename: edgrapi-meta-api-openapi.yml
  format: yaml
  label: Paper and Beyond Meta API
  slug: edgrapi-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-meta-api-openapi.yml
- filename: edgrapi-reference-api-openapi.yml
  format: yaml
  label: Paper and Beyond Reference API
  slug: edgrapi-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-reference-api-openapi.yml
- filename: edgrapi-search-api-openapi.yml
  format: yaml
  label: Paper and Beyond Search API
  slug: edgrapi-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-search-api-openapi.yml
- filename: edgrapi-webhooks-api-openapi.yml
  format: yaml
  label: Paper and Beyond Webhooks API
  slug: edgrapi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-webhooks-api-openapi.yml
- filename: edgrapi-xbrl-api-openapi.yml
  format: yaml
  label: Paper and Beyond Xbrl API
  slug: edgrapi-xbrl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/openapi/edgrapi-xbrl-api-openapi.yml
consequence_counts:
  physical: 1
  read: 29
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Edgrapi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/webhooks/{wid}/test
operation_count: 33
overview: 'Paper and Beyond exposes 33 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paper and Beyond
provider_slug: edgrapi
slug: edgrapi-agentic-access
source_filename: edgrapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: generated\nsource: openapi/edgrapi-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    acting: 4\n    connected: 29\n  by_consequence:\n    write: 3\n    read: 29\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/keys\n  method: post\n  operationId: create_free_key_v1_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/{ticker}\n  method: get\n  operationId: company_v1_company__ticker__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fundamentals/{ticker}\n  method: get\n  operationId: fundamentals_v1_fundamentals__ticker__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ratios/{ticker}\n  method: get\n  operationId: ratios_v1_ratios__ticker__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/filings/{ticker}\n  method: get\n  operationId: filings_v1_filings__ticker__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sections/{ticker}\n  method: get\n  operationId: filing_sections_v1_sections__ticker__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/download\n  method: get\n  operationId: download_filing_v1_download_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/insider/{ticker}\n  method: get\n  operationId: insider_trades_v1_insider__ticker__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/form144/{ticker}\n  method: get\n  operationId: form144_v1_form144__ticker__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/holdings/{identifier}\n  method: get\n  operationId: institutional_holdings_v1_holdings__identifier__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/activist/{identifier}\n  method: get\n  operationId: activist_stakes_v1_activist__identifier__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/restatements\n  method: get\n  operationId: events_restatements_v1_events_restatements_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/auditor-changes\n  method: get\n  operationId: events_auditor_changes_v1_events_auditor_changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events/{ticker}\n  method: get\n  operationId: material_events_v1_events__ticker__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resolve\n  method: get\n  operationId: resolve_entity_v1_resolve_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search/fulltext\n  method: get\n  operationId: search_fulltext_v1_search_fulltext_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/xbrl/by-accession/{accession}\n  method: get\n  operationId: xbrl_by_accession_v1_xbrl_by_accession__accession__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/xbrl/{ident}\n  method: get\n  operationId: xbrl_v1_xbrl__ident__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/shares/{ticker}\n  method: get\n  operationId: shares_v1_shares__ticker__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/formd/latest\n  method: get\n  operationId: formd_latest_v1_formd_latest_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/formd/{ident}\n  method: get\n  operationId: formd_issuer_v1_formd__ident__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/opportunities\n  method: get\n  operationId: opportunities_v1_opportunities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/awards\n  method: get\n  operationId: awards_v1_awards_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/grants\n  method: get\n  operationId: grants_v1_grants_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/congress\n  method: get\n  operationId: congress_feed_v1_congress_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/congress/{ticker}\n  method: get\n  operationId: congress_ticker_v1_congress__ticker__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subsidiaries/{ident}\n  method: get\n  operationId: company_subsidiaries_v1_subsidiaries__ident__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: get\n  operationId: webhook_list_v1_webhooks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: webhook_create_v1_webhooks_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /v1/webhooks/{wid}\n  method: delete\n  operationId: webhook_delete_v1_webhooks__wid__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{wid}/test\n  method: post\n  operationId: webhook_test_v1_webhooks__wid__test_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{wid}/deliveries\n  method: get\n  operationId: webhook_deliveries_v1_webhooks__wid__deliveries_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edgrapi/refs/heads/main/agentic-access/edgrapi-agentic-access.yml
summary_line: 33 operations · 4 acting
tags:
- Company
- Data
- Government
- Artificial Intelligence
---
