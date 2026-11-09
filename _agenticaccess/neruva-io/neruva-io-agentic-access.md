---
acting_count: 108
action_class_counts:
  acting: 108
  connected: 65
api_specs:
- filename: neruva-io-agent-cognitive-api-openapi.yml
  format: yaml
  label: neruva-io Agent Cognitive API
  slug: neruva-io-agent-cognitive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neruva-io/openapi/neruva-io-agent-cognitive-api-openapi.yml
- filename: neruva-io-agent-federated-api-openapi.yml
  format: yaml
  label: neruva-io Agent Federated API
  slug: neruva-io-agent-federated-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neruva-io/openapi/neruva-io-agent-federated-api-openapi.yml
- filename: neruva-io-audit-api-openapi.yml
  format: yaml
  label: neruva-io Audit API
  slug: neruva-io-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neruva-io/openapi/neruva-io-audit-api-openapi.yml
- filename: neruva-io-commons-api-openapi.yml
  format: yaml
  label: neruva-io Commons API
  slug: neruva-io-commons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neruva-io/openapi/neruva-io-commons-api-openapi.yml
- filename: neruva-io-hd-native-api-openapi.yml
  format: yaml
  label: neruva-io Hd Native API
  slug: neruva-io-hd-native-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neruva-io/openapi/neruva-io-hd-native-api-openapi.yml
- filename: neruva-io-health-api-openapi.yml
  format: yaml
  label: neruva-io Health API
  slug: neruva-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neruva-io/openapi/neruva-io-health-api-openapi.yml
- filename: neruva-io-indexes-api-openapi.yml
  format: yaml
  label: neruva-io Indexes API
  slug: neruva-io-indexes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neruva-io/openapi/neruva-io-indexes-api-openapi.yml
- filename: neruva-io-me-api-openapi.yml
  format: yaml
  label: neruva-io Me API
  slug: neruva-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neruva-io/openapi/neruva-io-me-api-openapi.yml
- filename: neruva-io-memory-api-openapi.yml
  format: yaml
  label: neruva-io Memory API
  slug: neruva-io-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neruva-io/openapi/neruva-io-memory-api-openapi.yml
- filename: neruva-io-neruva-api-openapi.yml
  format: yaml
  label: neruva-io Neruva API
  slug: neruva-io-neruva-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neruva-io/openapi/neruva-io-neruva-api-openapi.yml
- filename: neruva-io-pii-api-openapi.yml
  format: yaml
  label: neruva-io Pii API
  slug: neruva-io-pii-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neruva-io/openapi/neruva-io-pii-api-openapi.yml
- filename: neruva-io-records-api-openapi.yml
  format: yaml
  label: neruva-io Records API
  slug: neruva-io-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neruva-io/openapi/neruva-io-records-api-openapi.yml
consequence_counts:
  read: 65
  safety-critical: 13
  write: 95
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 13
kind: agentic-access
layout: agentic-access
method: generated
name: Neruva Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/agent/code/step
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/agent/computer/step
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/agent/computer/step_magistral
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/agent/plan_cache_lookup
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/agent/plan_cache_save
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/agent/reflect_prompt
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/agent/route_intent_prompt
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/commons/skills
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/commons/skills/{skill_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/commons/skills/{skill_id}/cert
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/commons/skills/{skill_id}/checker
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/commons/skills/{skill_id}/onecall
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/commons/skills/{skill_id}/purpose
operation_count: 173
overview: 'neruva-io exposes 173 API operations that an AI agent could call, of which 108 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 65 read, 95 write, and 13 safety-critical.


  13 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: neruva-io
provider_slug: neruva-io
slug: neruva-io-agentic-access
source_filename: neruva-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/neruva-io-internal-openapi.json, openapi/neruva-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 173\n  by_action_class:\n    connected: 65\n    acting: 108\n  by_consequence:\n    read: 65\n    write: 95\n    safety-critical: 13\n  human_in_the_loop_required: 13\noperations:\n- path: /users\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{id}\n  method: delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /export\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/settings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/settings\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/keys\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/kg/{name}/facts\n  method: post\n  operationId: add_facts_v1_hd_kg__name__facts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/kg/{name}/neighbors\n  method: post\n  operationId: kg_neighbors_v1_hd_kg__name__neighbors_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/kg/{name}/context\n  method: post\n  operationId: get_context_v1_hd_kg__name__context_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/kg/extraction_prompt\n  method: get\n  operationId: kg_extraction_prompt_v1_hd_kg_extraction_prompt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/kg/{name}/derive\n  method: post\n  operationId: derive_relation_v1_hd_kg__name__derive_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/kg/{name}/compose\n  method: post\n  operationId: compose_relation_v1_hd_kg__name__compose_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/kg/{name}/replace_fact\n  method: post\n  operationId: replace_fact_v1_hd_kg__name__replace_fact_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/kg/{name}/facts/delete\n  method: post\n  operationId: delete_facts_v1_hd_kg__name__facts_delete_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/kg/{name}/forget_entity\n  method: post\n  operationId: forget_entity_v1_hd_kg__name__forget_entity_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/kg/{name}/query\n  method: post\n  operationId: query_kg_v1_hd_kg__name__query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/kg/{name}/assign_features\n  method: post\n  operationId: assign_features_v1_hd_kg__name__assign_features_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/kg/{name}/quorum_audit\n  method: post\n  operationId: quorum_audit_v1_hd_kg__name__quorum_audit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/kg/{name}/compress\n  method: post\n  operationId: compress_to_tt_v1_hd_kg__name__compress_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/kg/{name}/query_topk\n  method: post\n  operationId: query_kg_topk_v1_hd_kg__name__query_topk_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/kg\n  method: get\n  operationId: list_kgs_v1_hd_kg_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/kg/backfill_subject_index\n  method: post\n  operationId: backfill_subject_index_v1_hd_kg_backfill_subject_index_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/kg/{name}/describe\n  method: get\n\
  \  operationId: describe_kg_v1_hd_kg__name__describe_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/kg/{name}/stats\n  method: get\n  operationId: kg_stats_v1_hd_kg__name__stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/kg/{name}/export\n  method: get\n  operationId: export_kg_v1_hd_kg__name__export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/kg/{name}/import\n  method: post\n  operationId: import_kg_v1_hd_kg__name__import_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/kg/{name}\n  method: delete\n  operationId: delete_kg_v1_hd_kg__name__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/analogy\n  method: post\n  operationId: analogy_v1_hd_analogy_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/cbr/{name}/create\n  method: post\n  operationId: cbr_create_v1_hd_cbr__name__create_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/cbr/{name}/episodes\n  method: post\n  operationId: cbr_add_episodes_v1_hd_cbr__name__episodes_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/cbr/{name}/query\n  method: post\n  operationId: cbr_query_v1_hd_cbr__name__query_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/cbr/{name}/stats\n  method:\
  \ get\n  operationId: cbr_stats_v1_hd_cbr__name__stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/cbr/{name}\n  method: delete\n  operationId: cbr_delete_v1_hd_cbr__name__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/cbr\n  method: get\n  operationId: list_cbrs_v1_hd_cbr_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/cbr/{name}/describe\n  method: get\n  operationId: describe_cbr_v1_hd_cbr__name__describe_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/blend/query\n  method: post\n  operationId: blend_query_v1_hd_blend_query_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/causal/{name}/worlds\n  method: post\n  operationId: add_worlds_v1_hd_causal__name__worlds_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/causal/{name}/query\n  method: post\n  operationId: query_causal_v1_hd_causal__name__query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/causal/{name}/export\n  method: get\n  operationId: export_scm_v1_hd_causal__name__export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/causal/{name}/import\n  method: post\n  operationId: import_scm_v1_hd_causal__name__import_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/causal/{name}\n  method: delete\n  operationId: delete_causal_v1_hd_causal__name__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/hd/causal\n  method: get\n  operationId: list_causals_v1_hd_causal_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hd/causal/{name}/describe\n  method: get\n  operationId: describe_causal_v1_hd_causal__name__describe_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/records/{namespace}\n  method: post\n  operationId: ingest_v1_records__namespace__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/records/{namespace}/query\n\
  \  method: post\n  operationId: query_v1_records__namespace__query_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/records/{namespace}/timeline\n  method: get\n  operationId: timeline_v1_records__namespace__timeline_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/records/{namespace}/forget\n  method: post\n  operationId: forget_v1_records__namespace__forget_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/records/{namespace}/compact\n  method: post\n  operationId: compact_v1_records__namespace__compact_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/records/{namespace}/stats\n  method: get\n  operationId: stats_v1_records__namespace__stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/records/{namespace}/export\n  method: get\n  operationId: export_neruva_v1_records__namespace__export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/records/{namespace}/import\n  method: post\n  operationId: import_neruva_v1_records__namespace__import_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/records/{namespace}/{record_id}\n  method: get\n  operationId: get_record_v1_records__namespace___record_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/records/{namespace}/{record_id}\n  method: delete\n  operationId: delete_record_v1_records__namespace___record_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/records/{namespace}/{record_id}/update\n  method: post\n  operationId: update_record_v1_records__namespace___record_id__update_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/records/{namespace}/{record_id}/replace_text\n  method: post\n  operationId: replace_record_text_v1_records__namespace___record_id__replace_text_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/records/{namespace}/{record_id}/bind_tag\n  method: post\n  operationId: bind_record_tag_v1_records__namespace___record_id__bind_tag_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/me/plan\n  method: get\n  operationId: me_plan_v1_me_plan_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/wallet\n  method: get\n  operationId: me_wallet_v1_me_wallet_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/usage\n  method: get\n  operationId: me_usage_v1_me_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/keys\n  method: get\n  operationId: me_keys_v1_me_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/me/op_log\n  method: get\n  operationId: me_op_log_v1_me_op_log_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/remember\n  method: post\n  operationId: agent_remember_v1_agent_remember_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/recall\n  method: post\n  operationId: agent_recall_v1_agent_recall_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/agent/snapshot\n  method: post\n  operationId: agent_snapshot_v1_agent_snapshot_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/restore\n  method: post\n  operationId: agent_restore_v1_agent_restore_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/context_put\n  method: post\n  operationId: agent_context_put_v1_agent_context_put_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/context_get\n  method: post\n  operationId: agent_context_get_v1_agent_context_get_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/check_consistency\n  method: post\n  operationId: agent_check_consistency_v1_agent_check_consistency_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/consensus_check\n  method: post\n  operationId: agent_consensus_check_v1_agent_consensus_check_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/associative_recall\n  method: post\n  operationId: agent_associative_recall_v1_agent_associative_recall_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/causal_query\n  method: post\n  operationId: agent_causal_query_v1_agent_causal_query_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/context\n  method: post\n  operationId: agent_context_v1_agent_context_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/context_typed\n  method: post\n  operationId: agent_context_typed_v1_agent_context_typed_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/plan_cache_lookup\n  method: post\n  operationId: _killed_agent_step_v1_agent_plan_cache_lookup_post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agent/plan_cache_save\n  method: post\n  operationId: _killed_agent_step_v1_agent_plan_cache_save_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agent/code/step\n  method: post\n  operationId: _killed_agent_step_v1_agent_code_step_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agent/computer/step_magistral\n  method: post\n  operationId: _killed_agent_step_v1_agent_computer_step_magistral_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agent/computer/step\n  method: post\n  operationId: _killed_agent_step_v1_agent_computer_step_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agent/route_intent_prompt\n\
  \  method: post\n  operationId: _killed_agent_step_v1_agent_route_intent_prompt_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agent/reflect_prompt\n  method: post\n  operationId: _killed_agent_step_v1_agent_reflect_prompt_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/agent/recall_full\n  method: post\n  operationId: agent_recall_full_v1_agent_recall_full_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/counterfactual_rollout\n  method: post\n  operationId: counterfactual_rollout_v1_agent_counterfactual_rollout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/model_belief_add\n  method: post\n  operationId: model_belief_add_v1_agent_model_belief_add_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/agent/model_belief\n  method: post\n  operationId: model_belief_v1_agent_model_belief_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/extract_schema\n  method: post\n  operationId: extract_schema_v1_agent_extract_schema_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/register_action\n  method: post\n  operationId: register_action_v1_agent_register_action_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/plan_efe\n  method: post\n  operationId: plan_efe_v1_agent_plan_efe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/continual_train\n  method: post\n  operationId: continual_train_v1_agent_continual_train_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/continual_predict\n  method: post\n  operationId: continual_predict_v1_agent_continual_predict_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/hierarchical_add\n  method: post\n  operationId: hierarchical_add_v1_agent_hierarchical_add_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/hierarchical_decode\n  method: post\n  operationId: hierarchical_decode_v1_agent_hierarchical_decode_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/induce_rule\n  method: post\n  operationId: induce_rule_v1_agent_induce_rule_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/persist_rule\n  method: post\n  operationId: persist_rule_v1_agent_persist_rule_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/recall_rule\n  method: post\n  operationId: recall_rule_v1_agent_recall_rule_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pii/rules\n  method: post\n  operationId: create_pii_rule_v1_pii_rules_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pii/rules\n  method: get\n  operationId: list_pii_rules_v1_pii_rules_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (55 KB total) ---\n# Full source: https://artifacts.apis.io/neruva-io/agentic-access/neruva-io-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/neruva-io/agentic-access/neruva-io-agentic-access.yml
summary_line: 173 operations · 108 acting · 13 human-in-the-loop
tags:
- Company
- Memory
- Artificial Intelligence
- Agents
- MCP
---
