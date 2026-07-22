---
acting_count: 59
action_class_counts:
  acting: 59
  connected: 58
api_specs:
- filename: oxen-hub-api-openapi-original.json
  format: json
  label: Oxen Hub AI & Fine-Tuning API
  slug: oxen-hub-ai-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-hub-api-openapi-original.json
- filename: oxen-server-openapi-original.json
  format: json
  label: Oxen Data Version Control Server API
  slug: oxen-data-version-control-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-server-openapi-original.json
consequence_counts:
  physical: 1
  read: 58
  safety-critical: 22
  write: 36
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 22
kind: agentic-access
layout: agentic-access
method: generated
name: Oxen Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/ai/audio/generate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/ai/chat/completions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/ai/images/edit
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/ai/images/generate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/ai/models/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/ai/models/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/ai/models/{id}/activate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/ai/models/{id}/deactivate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/ai/models/{id}/favorite
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/ai/models/{id}/favorite
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/ai/queue
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/ai/queue/{generation_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/ai/videos/generate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/repos/{namespace}/{repo_name}/evaluations/*resource_path
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/repos/{namespace}/{repo_name}/fine_tunes
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}/actions/run
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}/actions/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}/checkpoints/{step}/deploy
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}/tokenize
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}/train_status/{new_status}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/repos/{namespace}/{repo_name}/transfer
operation_count: 117
overview: 'Oxen exposes 117 API operations that an AI agent could call, of which 59 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 58 read, 36 write, 1 physical, and 22 safety-critical.


  22 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Oxen
provider_slug: oxen
slug: oxen-agentic-access
source_filename: oxen-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/oxen-hub-api-openapi-original.json, openapi/oxen-server-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 117\n  by_action_class:\n    acting: 59\n    connected: 58\n  by_consequence:\n    safety-critical: 22\n    read: 58\n    write: 36\n    physical: 1\n  human_in_the_loop_required: 22\noperations:\n- path: /api/ai/audio/generate\n  method: post\n  operationId: OxenApiWeb.Controllers.ModelController.generate_audio\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api/ai/chat/completions\n  method: post\n  operationId: OxenApiWeb.Controllers.ModelController.get_model_response\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/ai/generations\n  method: get\n  operationId: OxenApiWeb.Controllers.GenerationsController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai/generations/{generation_id}\n  method: get\n  operationId: OxenApiWeb.Controllers.GenerationsController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/ai/images/edit\n  method: post\n  operationId: OxenApiWeb.Controllers.ModelController.edit_image\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/ai/images/generate\n  method: post\n  operationId: OxenApiWeb.Controllers.ModelController.generate_image\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/ai/models\n  method: get\n  operationId: OxenApiWeb.Controllers.ModelsController.index\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai/models/favorites\n  method: get\n  operationId: OxenApiWeb.Controllers.ModelsController.list_favorites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai/models/featured\n  method: get\n  operationId: OxenApiWeb.Controllers.ModelsController.list_featured\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai/models/search\n  method: get\n  operationId: OxenApiWeb.Controllers.ModelsController.search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai/models/{id}\n  method: delete\n  operationId: OxenApiWeb.Controllers.ModelsController.delete_custom_model\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/ai/models/{id}\n  method: get\n  operationId: OxenApiWeb.Controllers.ModelsController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai/models/{id}\n  method: put\n  operationId: OxenApiWeb.Controllers.ModelsController.update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/ai/models/{id}/activate\n\
  \  method: post\n  operationId: OxenApiWeb.Controllers.ModelsController.wake\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/ai/models/{id}/deactivate\n  method: post\n  operationId: OxenApiWeb.Controllers.ModelsController.deactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/ai/models/{id}/favorite\n  method: delete\n  operationId: OxenApiWeb.Controllers.ModelsController.delete_favorite\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/ai/models/{id}/favorite\n  method: post\n  operationId: OxenApiWeb.Controllers.ModelsController.create_favorite\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/ai/queue\n  method: get\n  operationId: OxenApiWeb.Controllers.QueueController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai/queue\n  method: post\n  operationId:\
  \ OxenApiWeb.Controllers.QueueController.create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/ai/queue/{generation_id}\n  method: delete\n  operationId: OxenApiWeb.Controllers.QueueController.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/ai/queue/{generation_id}\n  method: get\n  operationId: OxenApiWeb.Controllers.QueueController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai/videos/generate\n  method: post\n  operationId: OxenApiWeb.Controllers.ModelController.generate_video\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/orgs/{name}/fine_tunes\n  method: get\n  operationId: OxenApiWeb.Controllers.FineTuneController.list_for_org\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/evaluations/*resource_path\n  method: post\n  operationId: OxenApiWeb.Controllers.EvaluationController.create_evaluation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/evaluations/{evaluation_id}\n  method: get\n  operationId: OxenApiWeb.Controllers.EvaluationController.get_evaluation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/fine_tunes\n  method: get\n  operationId: OxenApiWeb.Controllers.FineTuneController.index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/fine_tunes\n  method: post\n  operationId: OxenApiWeb.Controllers.FineTuneController.create\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}\n  method: delete\n  operationId: OxenApiWeb.Controllers.FineTuneController.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}\n  method: get\n  operationId: OxenApiWeb.Controllers.FineTuneController.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}\n  method: patch\n  operationId: OxenApiWeb.Controllers.FineTuneController.update\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}/actions/run\n  method: post\n  operationId: OxenApiWeb.Controllers.FineTuneController.run\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}/actions/stop\n\
  \  method: post\n  operationId: OxenApiWeb.Controllers.FineTuneController.stop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}/checkpoints\n  method: get\n  operationId: OxenApiWeb.Controllers.FineTuneController.checkpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}/checkpoints/{step}/deploy\n  method: post\n  operationId: OxenApiWeb.Controllers.FineTuneController.create_checkpoint_deployment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}/logs\n  method: get\n  operationId: OxenApiWeb.Controllers.FineTuneController.logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}/tokenize\n  method: post\n  operationId: OxenApiWeb.Controllers.FineTuneController.tokenize\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}/train_status\n\
  \  method: get\n  operationId: OxenApiWeb.Controllers.FineTuneController.get_train_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/fine_tunes/{id}/train_status/{new_status}\n  method: put\n  operationId: OxenApiWeb.Controllers.FineTuneController.update_train_status\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/user/fine_tunes\n  method: get\n  operationId: OxenApiWeb.Controllers.FineTuneController.list_accessible\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/users/{username}/fine_tunes\n  method: get\n  operationId: OxenApiWeb.Controllers.FineTuneController.list_for_user\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/branches/{branch_name}/merge\n  method: post\n  operationId: maybe_create_merge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/commits/upload\n  method: post\n  operationId: upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/compare/data_frames/{compare_id}/diff\n  method: get\n  operationId: get_derived_df\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/commits_db\n  method: get\n  operationId: download_commits_db\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/export/download/{resource}\n  method: get\n  operationId: download_zip\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/commits/upload_chunk\n  method: post\n  operationId: upload_chunk\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/compare/{base_head}/dir/{dir}/entries\n  method: get\n  operationId: dir_entries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/stats\n  method: get\n  operationId: stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/compare/{base_head}/file/{resource}\n  method: get\n  operationId: file\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/branches/{branch_name}\n\
  \  method: delete\n  operationId: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/branches/{branch_name}\n  method: get\n  operationId: show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/branches/{branch_name}\n  method: put\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/workspaces/clear\n\
  \  method: delete\n  operationId: clear\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/versions/batch-download\n  method: post\n  operationId: batch_download\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/data_frames/{resource}\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/compare/data_frames\n\
  \  method: post\n  operationId: create_df_diff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/commits/{commit_id}/complete\n  method: post\n  operationId: complete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/workspaces/{workspace_id}/merge/{branch}\n  method: get\n  operationId: mergeability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/workspaces/{workspace_id}/merge/{branch}\n\
  \  method: post\n  operationId: commit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/commits/mark_commits_as_synced\n  method: post\n  operationId: mark_commits_as_synced\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/commits/root\n  method: get\n  operationId: root_commit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}\n\
  \  method: get\n  operationId: index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/compare/{base_head}/tree\n  method: get\n  operationId: dir_tree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/compare/data_frames/{compare_id}\n  method: delete\n  operationId: delete_df_diff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/compare/data_frames/{compare_id}\n  method: get\n  operationId: get_df_diff\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/compare/data_frames/{compare_id}\n  method: put\n  operationId: update_df_diff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/commits/{commit_id}\n  method: get\n  operationId: show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/versions/{resource}\n  method: get\n  operationId: download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/repos/{namespace}/{repo_name}/workspaces/{workspace_id}\n  method: delete\n  operationId: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/workspaces/{workspace_id}\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/commits/{commit_or_branch}/commit_entries_db\n  method: get\n  operationId: download_commit_entries_db\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/import/{resource}\n  method:\
  \ post\n  operationId: import\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/commits\n  method: get\n  operationId: index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/commits\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/data_frames/from_directory/{resource}\n  method:\
  \ post\n  operationId: from_directory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/commits/history/{resource}\n  method: get\n  operationId: history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/namespaces/{namespace}\n  method: get\n  operationId: show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/versions/{version_id}/metadata\n  method: get\n  operationId: metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/workspaces/{workspace_id}/files/batch/{directory}\n  method: post\n  operationId: add_version_files\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/import/upload/{resource}\n  method: post\n  operationId: upload_zip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/workspaces/{workspace_id}/files/{path}\n  method: get\n  operationId: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/workspaces/{workspace_id}/files/{path}\n  method: post\n  operationId: add\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/commits/missing\n  method: get\n  operationId: list_missing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/metadata/{resource}\n  method: get\n  operationId: file\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/repos/{namespace}/{repo_name}/metadata/{resource}\n  method: put\n  operationId: update_metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/workspaces/{workspace_id}/changes/{path}\n  method: delete\n  operationId: unstage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/merge/{base_head}\n  method: get\n  operationId: show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/merge/{base_head}\n  method: post\n  operationId: merge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/commits/missing_files\n  method: get\n  operationId: list_missing_files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/file/{resource}\n  method: delete\n  operationId: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/file/{resource}\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/repos/{namespace}/{repo_name}/file/{resource}\n  method: patch\n  operationId: mv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/file/{resource}\n  method: put\n  operationId: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/workspaces/{workspace_id}/changes\n  method: delete\n  operationId: unstage_many\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/data_frames/{resource}/index\n  method: post\n  operationId: index\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/versions\n  method: post\n  operationId: batch_upload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/commits/{commit_id}/upload_tree\n  method: post\n  operationId: upload_tree\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/repos/{namespace}/{repo_name}/commits/all\n  method: get\n  operationId: list_all\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optiona\n\n# --- truncated at 32 KB (37 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/agentic-access/oxen-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/agentic-access/oxen-agentic-access.yml
summary_line: 117 operations · 59 acting · 22 human-in-the-loop
tags:
- Company
- Data Version Control
- Machine Learning
- Artificial Intelligence
- Fine-Tuning
- Inference
- Datasets
- MLOps
- Large Language Models
- Model Deployment
- Developer Tools
- Version Control
---
