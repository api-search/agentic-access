---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 22
api_specs:
- filename: abacore-net-abacore-workspace-api-openapi.yml
  format: yaml
  label: Abacore Abacore Workspace API
  slug: abacore-net-abacore-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-abacore-workspace-api-openapi.yml
- filename: abacore-net-ai-api-openapi.yml
  format: yaml
  label: Abacore AI API
  slug: abacore-net-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-ai-api-openapi.yml
- filename: abacore-net-cabinet-api-openapi.yml
  format: yaml
  label: Abacore Cabinet API
  slug: abacore-net-cabinet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-cabinet-api-openapi.yml
- filename: abacore-net-discovery-api-openapi.yml
  format: yaml
  label: Abacore Discovery API
  slug: abacore-net-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-discovery-api-openapi.yml
- filename: abacore-net-healthz-api-openapi.yml
  format: yaml
  label: Abacore Healthz API
  slug: abacore-net-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-healthz-api-openapi.yml
- filename: abacore-net-livez-api-openapi.yml
  format: yaml
  label: Abacore Livez API
  slug: abacore-net-livez-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-livez-api-openapi.yml
- filename: abacore-net-llms-txt-api-openapi.yml
  format: yaml
  label: Abacore Llms.txt API
  slug: abacore-net-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-llms-txt-api-openapi.yml
- filename: abacore-net-meta-api-openapi.yml
  format: yaml
  label: Abacore Meta API
  slug: abacore-net-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-meta-api-openapi.yml
- filename: abacore-net-opportunities-api-openapi.yml
  format: yaml
  label: Abacore Opportunities API
  slug: abacore-net-opportunities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-opportunities-api-openapi.yml
- filename: abacore-net-register-api-openapi.yml
  format: yaml
  label: Abacore Register API
  slug: abacore-net-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-register-api-openapi.yml
- filename: abacore-net-request-api-openapi.yml
  format: yaml
  label: Abacore Request API
  slug: abacore-net-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-request-api-openapi.yml
- filename: abacore-net-resources-api-openapi.yml
  format: yaml
  label: Abacore Resources API
  slug: abacore-net-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-resources-api-openapi.yml
- filename: abacore-net-school-api-openapi.yml
  format: yaml
  label: Abacore School API
  slug: abacore-net-school-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-school-api-openapi.yml
- filename: abacore-net-sitemap-xml-api-openapi.yml
  format: yaml
  label: Abacore Sitemap.xml API
  slug: abacore-net-sitemap-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-sitemap-xml-api-openapi.yml
- filename: abacore-net-well-known-api-openapi.yml
  format: yaml
  label: Abacore .well Known API
  slug: abacore-net-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-well-known-api-openapi.yml
- filename: abacore-net-workspace-api-openapi.yml
  format: yaml
  label: Abacore Workspace API
  slug: abacore-net-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abacore-net/openapi/abacore-net-workspace-api-openapi.yml
consequence_counts:
  read: 22
  safety-critical: 2
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Abacore Net Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cabinet/opportunity/{opportunity_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /cabinet/work/stop
operation_count: 43
overview: 'Abacore exposes 43 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 19 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Abacore
provider_slug: abacore-net
slug: abacore-net-agentic-access
source_filename: abacore-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/workspace-abacore-net-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    connected: 22\n    acting: 21\n  by_consequence:\n    read: 22\n    write: 19\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /livez\n  method: get\n  operationId: livez_livez_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: get\n  operationId: healthz_healthz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /\n  method: get\n  operationId: home__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities\n  method: get\n  operationId: opportunities_opportunities_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{public_id}\n  method: get\n  operationId: detail_opportunities__public_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace/opportunities/{public_id}\n  method: get\n  operationId: workspace_detail_alias_workspace_opportunities__public_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/meta\n  method: get\n \
  \ operationId: api_meta_api_v1_meta_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/resources\n  method: get\n  operationId: api_resources_api_v1_resources_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/resources/{public_id}\n  method: get\n  operationId: api_resource_detail_api_v1_resources__public_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/discovery\n  method: get\n  operationId: api_discovery_api_v1_discovery_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ai/discovery\n  method: get\n  operationId: api_ai_discovery_api_v1_ai_discovery_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/abacore-workspace.json\n  method: get\n  operationId: well_known_workspace__well_known_abacore_workspace_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: llms_txt_llms_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sitemap.xml\n  method: get\n  operationId: sitemap_sitemap_xml_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{public_id}/apply\n  method: get\n  operationId: apply_form_opportunities__public_id__apply_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{public_id}/apply\n  method: post\n  operationId: apply_submit_opportunities__public_id__apply_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /register\n  method: get\n  operationId: register_form_register_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /register\n  method: post\n  operationId: register_submit_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /school\n  method: get\n  operationId: school_school_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /school/apply\n  method: get\n  operationId: school_apply_school_apply_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /school/apply\n  method: post\n  operationId: school_submit_school_apply_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /request\n  method: get\n  operationId: request_form_request_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /request\n  method: post\n  operationId: request_submit_request_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cabinet/telegram/start\n  method: post\n  operationId: cabinet_telegram_start_cabinet_telegram_start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cabinet/telegram/status\n  method: post\n  operationId: cabinet_telegram_status_cabinet_telegram_status_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cabinet/login\n  method: post\n  operationId: cabinet_login_cabinet_login_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cabinet/logout\n  method: post\n  operationId: cabinet_logout_cabinet_logout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /cabinet\n  method: get\n  operationId: cabinet_cabinet_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cabinet/credentials\n  method: post\n  operationId: superadmin_credentials_cabinet_credentials_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cabinet/opportunity/{opportunity_id}/start\n  method: post\n  operationId: interaction_start_cabinet_opportunity__opportunity_id__start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /cabinet/opportunity/{opportunity_id}/stop\n  method: post\n  operationId: interaction_stop_cabinet_opportunity__opportunity_id__stop_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cabinet/opportunity/{opportunity_id}/stage\n  method: post\n  operationId: interaction_stage_cabinet_opportunity__opportunity_id__stage_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cabinet/opportunity/{opportunity_id}/note\n  method: post\n  operationId: work_note_cabinet_opportunity__opportunity_id__note_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cabinet/work/start\n  method: post\n  operationId: work_start_cabinet_work_start_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cabinet/work/heartbeat\n  method: post\n  operationId: work_heartbeat_cabinet_work_heartbeat_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /cabinet/work/stop\n  method: post\n  operationId: work_stop_cabinet_work_stop_post\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /cabinet/users\n  method: get\n  operationId: users_cabinet_users_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cabinet/users/create\n  method: post\n  operationId: user_create_cabinet_users_create_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /cabinet/users/{account_id}\n  method: get\n  operationId: user_detail_cabinet_users__account_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cabinet/users/{account_id}/policy\n  method: post\n  operationId: user_policy_cabinet_users__account_id__policy_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cabinet/users/{account_id}/password\n  method: post\n  operationId: user_password_cabinet_users__account_id__password_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cabinet/users/{account_id}/role\n  method: post\n  operationId: user_role_cabinet_users__account_id__role_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cabinet/users/{account_id}/status\n  method: post\n  operationId: user_status_cabinet_users__account_id__status_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/abacore-net/agentic-access/abacore-net-agentic-access.yml
summary_line: 43 operations · 21 acting · 2 human-in-the-loop
tags:
- Artificial Intelligence
- Cybersecurity
- Blockchain
- IoT
- Data Center
---
