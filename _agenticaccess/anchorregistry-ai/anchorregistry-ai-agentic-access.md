---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 10
api_specs:
- filename: anchorregistry-ai-account-api-openapi.yml
  format: yaml
  label: AnchorRegistry Account API
  slug: anchorregistry-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchorregistry-ai/openapi/anchorregistry-ai-account-api-openapi.yml
- filename: anchorregistry-ai-discovery-api-openapi.yml
  format: yaml
  label: AnchorRegistry Discovery API
  slug: anchorregistry-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchorregistry-ai/openapi/anchorregistry-ai-discovery-api-openapi.yml
- filename: anchorregistry-ai-register-api-openapi.yml
  format: yaml
  label: AnchorRegistry Register API
  slug: anchorregistry-ai-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchorregistry-ai/openapi/anchorregistry-ai-register-api-openapi.yml
- filename: anchorregistry-ai-system-api-openapi.yml
  format: yaml
  label: AnchorRegistry System API
  slug: anchorregistry-ai-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchorregistry-ai/openapi/anchorregistry-ai-system-api-openapi.yml
- filename: anchorregistry-ai-verify-api-openapi.yml
  format: yaml
  label: AnchorRegistry Verify API
  slug: anchorregistry-ai-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anchorregistry-ai/openapi/anchorregistry-ai-verify-api-openapi.yml
consequence_counts:
  read: 10
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Anchorregistry Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'AnchorRegistry exposes 21 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AnchorRegistry
provider_slug: anchorregistry-ai
slug: anchorregistry-ai-agentic-access
source_filename: anchorregistry-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/anchorregistry-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 10\n    acting: 11\n  by_consequence:\n    read: 10\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: status_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/nonce\n  method: get\n\
  \  operationId: nonce_status_status_nonce_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registration/reserve\n  method: post\n  operationId: reserve_ar_ids_registration_reserve_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registration/status/{session_id}\n  method: get\n  operationId: get_registration_status_registration_status__session_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registration/seal\n  method: post\n  operationId: seal_tree_registration_seal_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registration/retraction\n  method: post\n  operationId: retract_anchor_registration_retraction_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registration/review\n  method: post\n  operationId: register_review_registration_review_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registration/void\n\
  \  method: post\n  operationId: register_void_registration_void_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registration/affirmed\n  method: post\n  operationId: register_affirmed_registration_affirmed_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /registration/pending\n  method: post\n  operationId: create_pending_registration_registration_pending_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/stripe\n  method: post\n  operationId: stripe_webhook_webhook_stripe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /register/account\n  method: post\n  operationId: register_account_register_account_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /register/account/topup\n  method: post\n  operationId: topup_account_register_account_topup_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /register/x402\n  method: post\n  operationId: register_with_account_register_x402_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{anchor_key}/balance\n  method: get\n  operationId: get_account_balance_account__anchor_key__balance_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{anchor_key}/tree\n  method: get\n  operationId: get_account_tree_account__anchor_key__tree_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/hash/{manifest_hash}\n  method: get\n  operationId: verify_by_manifest_hash_verify_hash__manifest_hash__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/{ar_id}\n  method: get\n  operationId: verify_by_ar_id_verify__ar_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tree/{ar_id}\n  method: get\n  operationId: get_tree_tree__ar_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/x402\n  method: get\n  operationId: x402_discovery__well_known_x402_get\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/anchorregistry-ai/agentic-access/anchorregistry-ai-agentic-access.yml
summary_line: 21 operations · 11 acting
tags:
- Provenance
- Onchain
- Artificial Intelligence
- Data
- Artifacts
---
