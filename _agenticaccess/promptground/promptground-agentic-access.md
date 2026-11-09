---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 15
api_specs:
- filename: promptground-api-v1-api-openapi.yml
  format: yaml
  label: PromptGround API v1 API
  slug: promptground-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-api-v1-api-openapi.yml
- filename: promptground-api-v2-api-openapi.yml
  format: yaml
  label: PromptGround API v2 API
  slug: promptground-api-v2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-api-v2-api-openapi.yml
- filename: promptground-invites-api-openapi.yml
  format: yaml
  label: PromptGround Invites API
  slug: promptground-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-invites-api-openapi.yml
- filename: promptground-models-api-openapi.yml
  format: yaml
  label: PromptGround Models API
  slug: promptground-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-models-api-openapi.yml
- filename: promptground-payments-api-openapi.yml
  format: yaml
  label: PromptGround Payments API
  slug: promptground-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-payments-api-openapi.yml
- filename: promptground-projects-api-openapi.yml
  format: yaml
  label: PromptGround Projects API
  slug: promptground-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-projects-api-openapi.yml
- filename: promptground-prompts-api-openapi.yml
  format: yaml
  label: PromptGround Prompts API
  slug: promptground-prompts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-prompts-api-openapi.yml
- filename: promptground-sessions-api-openapi.yml
  format: yaml
  label: PromptGround Sessions API
  slug: promptground-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-sessions-api-openapi.yml
- filename: promptground-settings-api-openapi.yml
  format: yaml
  label: PromptGround Settings API
  slug: promptground-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-settings-api-openapi.yml
consequence_counts:
  physical: 1
  read: 15
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Promptground Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/webhook
operation_count: 36
overview: 'PromptGround exposes 36 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 20 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PromptGround
provider_slug: promptground
slug: promptground-agentic-access
source_filename: promptground-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/promptground-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    connected: 15\n    acting: 21\n  by_consequence:\n    read: 15\n    write: 20\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /projects\n  method: get\n  operationId: get_projects_projects_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: post\n  operationId: create_project_projects_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}\n  method: get\n  operationId: get_project_projects__project_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}\n  method: post\n  operationId: update_project_projects__project_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}\n  method: delete\n  operationId: delete_project_projects__project_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/leave\n  method: post\n  operationId: leave_project_endpoint_projects__project_id__leave_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/remove_user/{user_id_to_remove}\n  method: delete\n  operationId: remove_user_from_project_projects__project_id__remove_user__user_id_to_remove__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /projects/{project_id}/prompts\n  method: get\n  operationId: get_prompts_projects__project_id__prompts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/prompts\n  method: post\n  operationId: create_prompt_projects__project_id__prompts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/prompts/runs\n  method: post\n  operationId: get_prompt_runs_projects__project_id__prompts_runs_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/prompts/fresh-runs\n\
  \  method: post\n  operationId: get_prompt_runs_projects__project_id__prompts_fresh_runs_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/prompts/runs/{run_id}\n  method: post\n  operationId: get_prompt_runs_projects__project_id__prompts_runs__run_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/prompts/{prompt_id}\n  method: get\n  operationId: get_prompt_details_projects__project_id__prompts__prompt_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/prompts/{prompt_id}\n\
  \  method: post\n  operationId: update_prompt_projects__project_id__prompts__prompt_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/prompts/{prompt_id}/delete\n  method: post\n  operationId: delete_prompt_projects__project_id__prompts__prompt_id__delete_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/prompts/{prompt_id}/versions/{prompt_version_id}/variables\n  method: get\n  operationId: get_version_variables_projects__project_id__prompts__prompt_id__versions__prompt_version_id__variables_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/prompts/{prompt_id}/run/{prompt_version_id}\n  method: post\n  operationId: post_run_prompt_projects__project_id__prompts__prompt_id__run__prompt_version_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/settings/team\n  method: get\n  operationId: get_team_projects__project_id__settings_team_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/settings\n  method: post\n  operationId: create_project_projects__project_id__settings_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/settings/api-keys\n  method: get\n  operationId: get_api_keys_projects__project_id__settings_api_keys_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{project_id}/settings/api-keys\n  method: post\n  operationId: create_api_key_projects__project_id__settings_api_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/settings/api-keys/{api_key_id}\n\
  \  method: post\n  operationId: update_api_key_name_projects__project_id__settings_api_keys__api_key_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{project_id}/settings/api-keys/{api_key_id}\n  method: delete\n  operationId: delete_api_key_projects__project_id__settings_api_keys__api_key_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invites/accept/{code}\n  method: post\n  operationId: accept_invite_invites_accept__code__post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invites/{project_id}\n  method: post\n  operationId: create_invite_invites__project_id__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/new\n  method: post\n  operationId: new_session_sessions_new_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/me\n  method: get\n  operationId:\
  \ new_sessions_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/pay/{interval}/{project_id}\n  method: get\n  operationId: redirect_to_payment_payments_pay__interval___project_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/tokens/pay/{project_id}\n  method: get\n  operationId: redirect_to_payment_for_tokens_payments_tokens_pay__project_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/credits/pay/{project_id}\n  method: get\n  operationId: redirect_to_payment_for_credits_payments_credits_pay__project_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /payments/webhook\n  method: post\n  operationId: stripe_webhook_payments_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/supported-models\n  method: get\n  operationId: get_supported_models_models_supported_models_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/models-with-pricing\n  method: get\n  operationId: get_models_with_pricing_models_models_with_pricing_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/prompt\n  method: post\n  operationId: prompt_v1_prompt_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/prompt/messages\n  method: post\n  operationId: messages_v2_prompt_messages_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/prompt/run\n  method: post\n  operationId: run_prompt_v2_prompt_run_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/promptground/agentic-access/promptground-agentic-access.yml
summary_line: 36 operations · 21 acting
tags:
- Artificial Intelligence
- Prompt Engineering
- Collaboration
- Analytics
- SDK
---
