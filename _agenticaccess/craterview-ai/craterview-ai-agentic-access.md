---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 11
api_specs:
- filename: craterview-ai-account-api-openapi.yml
  format: yaml
  label: craterview-ai Account API
  slug: craterview-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craterview-ai/openapi/craterview-ai-account-api-openapi.yml
- filename: craterview-ai-gallery-api-openapi.yml
  format: yaml
  label: craterview-ai Gallery API
  slug: craterview-ai-gallery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craterview-ai/openapi/craterview-ai-gallery-api-openapi.yml
- filename: craterview-ai-jobs-api-openapi.yml
  format: yaml
  label: craterview-ai Jobs API
  slug: craterview-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craterview-ai/openapi/craterview-ai-jobs-api-openapi.yml
- filename: craterview-ai-keys-api-openapi.yml
  format: yaml
  label: craterview-ai Keys API
  slug: craterview-ai-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craterview-ai/openapi/craterview-ai-keys-api-openapi.yml
- filename: craterview-ai-models-api-openapi.yml
  format: yaml
  label: craterview-ai Models API
  slug: craterview-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craterview-ai/openapi/craterview-ai-models-api-openapi.yml
- filename: craterview-ai-usage-api-openapi.yml
  format: yaml
  label: craterview-ai Usage API
  slug: craterview-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craterview-ai/openapi/craterview-ai-usage-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  safety-critical: 2
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Craterview Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/keys/current
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/keys/{key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/gallery/{post_id}
operation_count: 24
overview: 'craterview-ai exposes 24 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 10 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: craterview-ai
provider_slug: craterview-ai
slug: craterview-ai-agentic-access
source_filename: craterview-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/craterview-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 11\n    acting: 13\n  by_consequence:\n    read: 11\n    write: 10\n    safety-critical: 2\n    physical: 1\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/models\n  method: get\n  operationId: list_models_v1_models_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/uploads\n  method: post\n  operationId: create_upload_v1_uploads_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads\n  method: get\n  operationId: read_upload_v1_uploads_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs\n  method: post\n  operationId: create_job_v1_jobs_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs\n  method: get\n  operationId: list_jobs_v1_jobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}\n  method: get\n \
  \ operationId: get_job_v1_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{job_id}/keep\n  method: post\n  operationId: keep_v1_jobs__job_id__keep_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{job_id}/keep\n  method: delete\n  operationId: forget_v1_jobs__job_id__keep_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs/{job_id}/media\n  method: delete\n  operationId:\
  \ delete_media_v1_jobs__job_id__media_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: get_usage_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: get\n  operationId: list_keys_v1_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: mint_key_v1_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/current\n  method: get\n  operationId: current_key_v1_keys_current_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/current\n  method: delete\n  operationId: revoke_current_key_v1_keys_current_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/keys/{key_id}\n  method: delete\n  operationId: revoke_key_v1_keys__key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/account\n  method: delete\n  operationId: close_account_v1_account_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/secret\n  method: get\n  operationId: get_webhook_secret_v1_webhooks_secret_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/secret/rotate\n  method: post\n  operationId: rotate_webhook_secret_v1_webhooks_secret_rotate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/product-updates\n  method: get\n  operationId: get_product_updates_v1_account_product_updates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account/product-updates\n  method: put\n  operationId: put_product_updates_v1_account_product_updates_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/gallery\n  method: post\n  operationId: submit_v1_gallery_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/gallery\n  method: get\n  operationId: gallery_v1_gallery_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gallery/submissions\n  method: get\n  operationId: mine_v1_gallery_submissions_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gallery/{post_id}\n  method: delete\n  operationId: withdraw_v1_gallery__post_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/craterview-ai/agentic-access/craterview-ai-agentic-access.yml
summary_line: 24 operations · 13 acting · 2 human-in-the-loop
tags:
- Image Processing
- Artificial Intelligence
- PhotoRestoration
- Upscaling
- Multimedia
---
