---
acting_count: 30
action_class_counts:
  acting: 30
  connected: 23
api_specs:
- filename: sudomock-com-account-api-openapi.yml
  format: yaml
  label: sudomock-com Account API
  slug: sudomock-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-account-api-openapi.yml
- filename: sudomock-com-background-removal-api-openapi.yml
  format: yaml
  label: sudomock-com Background removal API
  slug: sudomock-com-background-removal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-background-removal-api-openapi.yml
- filename: sudomock-com-fonts-api-openapi.yml
  format: yaml
  label: sudomock-com Fonts API
  slug: sudomock-com-fonts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-fonts-api-openapi.yml
- filename: sudomock-com-jobs-api-openapi.yml
  format: yaml
  label: sudomock-com Jobs API
  slug: sudomock-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-jobs-api-openapi.yml
- filename: sudomock-com-photo-mockups-api-openapi.yml
  format: yaml
  label: sudomock-com Photo mockups API
  slug: sudomock-com-photo-mockups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-photo-mockups-api-openapi.yml
- filename: sudomock-com-psd-mockups-api-openapi.yml
  format: yaml
  label: sudomock-com PSD mockups API
  slug: sudomock-com-psd-mockups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-psd-mockups-api-openapi.yml
- filename: sudomock-com-studio-api-openapi.yml
  format: yaml
  label: sudomock-com Studio API
  slug: sudomock-com-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-studio-api-openapi.yml
- filename: sudomock-com-video-mockups-api-openapi.yml
  format: yaml
  label: sudomock-com Video mockups API
  slug: sudomock-com-video-mockups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-video-mockups-api-openapi.yml
- filename: sudomock-com-webhook-deliveries-api-openapi.yml
  format: yaml
  label: sudomock-com Webhook deliveries API
  slug: sudomock-com-webhook-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-webhook-deliveries-api-openapi.yml
- filename: sudomock-com-webhook-endpoints-api-openapi.yml
  format: yaml
  label: sudomock-com Webhook endpoints API
  slug: sudomock-com-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-webhook-endpoints-api-openapi.yml
consequence_counts:
  physical: 1
  read: 23
  write: 29
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sudomock Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/webhook-endpoints/{endpoint_id}/test
operation_count: 53
overview: 'sudomock-com exposes 53 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read, 29 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: sudomock-com
provider_slug: sudomock-com
slug: sudomock-com-agentic-access
source_filename: sudomock-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/sudomock-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    acting: 30\n    connected: 23\n  by_consequence:\n    write: 29\n    read: 23\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/psd/upload\n  method: post\n  operationId: upload_psd_api_v1_psd_upload_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/renders\n  method: post\n  operationId: render_mockup_api_v1_renders_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/remove-background\n  method: post\n  operationId: remove_background_api_v1_remove_background_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/renders/video\n  method: post\n  operationId: render_video_api_v1_renders_video_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/jobs\n  method: get\n  operationId: list_jobs_api_v1_jobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jobs/{job_id}\n  method: get\n  operationId: get_job_api_v1_jobs__job_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/plans\n  method: get\n  operationId: get_plans_api_v1_packages_plans_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-endpoints\n  method: post\n  operationId: create_webhook_endpoint_api_v1_webhook_endpoints_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhook-endpoints\n  method: get\n  operationId: list_webhook_endpoints_api_v1_webhook_endpoints_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-endpoints/events\n  method: get\n  operationId: list_events_api_v1_webhook_endpoints_events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-endpoints/overview\n  method: get\n  operationId: webhook_overview_api_v1_webhook_endpoints_overview_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-endpoints/{endpoint_id}\n\
  \  method: get\n  operationId: get_webhook_endpoint_api_v1_webhook_endpoints__endpoint_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-endpoints/{endpoint_id}\n  method: patch\n  operationId: update_webhook_endpoint_api_v1_webhook_endpoints__endpoint_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhook-endpoints/{endpoint_id}\n  method: delete\n  operationId: delete_webhook_endpoint_api_v1_webhook_endpoints__endpoint_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhook-endpoints/{endpoint_id}/rotate-secret\n  method: post\n  operationId: rotate_webhook_secret_api_v1_webhook_endpoints__endpoint_id__rotate_secret_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhook-endpoints/{endpoint_id}/test\n  method: post\n  operationId: send_test_event_api_v1_webhook_endpoints__endpoint_id__test_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/webhook-endpoints/{endpoint_id}/deliveries\n  method: get\n  operationId: list_deliveries_api_v1_webhook_endpoints__endpoint_id__deliveries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-endpoints/{endpoint_id}/deliveries/{delivery_id}\n  method: get\n  operationId: get_delivery_detail_api_v1_webhook_endpoints__endpoint_id__deliveries__delivery_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-endpoints/{endpoint_id}/deliveries/{delivery_id}/replay\n  method: post\n  operationId: replay_delivery_api_v1_webhook_endpoints__endpoint_id__deliveries__delivery_id__replay_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhook-endpoints/{endpoint_id}/deliveries/replay-failed\n  method: post\n  operationId: replay_failed_deliveries_api_v1_webhook_endpoints__endpoint_id__deliveries_replay_failed_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/psd-mockups\n  method: get\n  operationId: list_mockups_api_v1_psd_mockups_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/psd-mockups/{uuid}\n  method: get\n  operationId: get_mockup_detail_api_v1_psd_mockups__uuid__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/psd-mockups/{uuid}\n  method: patch\n  operationId: update_mockup_api_v1_psd_mockups__uuid__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/psd-mockups/{uuid}/layers\n  method: get\n  operationId: get_mockup_layers_api_v1_psd_mockups__uuid__layers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/psd-mockups/{mockup_uuid}\n  method: delete\n  operationId: delete_mockup_api_v1_psd_mockups__mockup_uuid__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/mockups\n  method: get\n  operationId: list_mockups_api_v1_mockups_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/mockups/{uuid}\n  method: get\n  operationId: get_mockup_detail_api_v1_mockups__uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/mockups/{uuid}\n  method: patch\n  operationId: update_mockup_api_v1_mockups__uuid__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/mockups/{uuid}/layers\n  method: get\n  operationId: get_mockup_layers_api_v1_mockups__uuid__layers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/mockups/{mockup_uuid}\n  method: delete\n  operationId: delete_mockup_api_v1_mockups__mockup_uuid__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fonts\n  method: get\n  operationId: list_fonts_api_v1_fonts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fonts\n  method: post\n  operationId:\
  \ upload_font_api_v1_fonts_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fonts/{uuid}\n  method: get\n  operationId: get_font_api_v1_fonts__uuid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fonts/{uuid}\n  method: delete\n  operationId: delete_font_api_v1_fonts__uuid__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/me\n  method: get\n  operationId: get_current_user_info_api_v1_me_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/photo-mockups\n  method: post\n  operationId: create_public_2d_mockup_api_v1_photo_mockups_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/photo-mockups\n  method: get\n  operationId: list_2d_mockups_api_v1_photo_mockups_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/photo-mockups/{mockup_id}/print-areas\n  method: put\n  operationId: replace_public_2d_print_areas_api_v1_photo_mockups__mockup_id__print_areas_put\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/photo-mockups/{mockup_id}\n  method: get\n  operationId: get_2d_mockup_public_api_v1_photo_mockups__mockup_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/photo-mockups/{mockup_id}\n  method: patch\n  operationId: update_2d_mockup_api_v1_photo_mockups__mockup_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/photo-mockups/{mockup_id}\n  method: delete\n  operationId: delete_2d_mockup_api_v1_photo_mockups__mockup_id__delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/photo-mockups/{mockup_id}/render\n  method: post\n  operationId: render_2d_mockup_public_api_v1_photo_mockups__mockup_id__render_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sudoai/2d-mockups\n  method: post\n  operationId: create_public_2d_mockup_api_v1_sudoai_2d_mockups_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sudoai/2d-mockups\n  method: get\n  operationId: list_2d_mockups_api_v1_sudoai_2d_mockups_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sudoai/2d-mockups/{mockup_id}/print-areas\n  method: put\n  operationId: replace_public_2d_print_areas_api_v1_sudoai_2d_mockups__mockup_id__print_areas_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sudoai/2d-mockups/{mockup_id}\n  method: get\n  operationId: get_2d_mockup_public_api_v1_sudoai_2d_mockups__mockup_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sudoai/2d-mockups/{mockup_id}\n  method: patch\n  operationId: update_2d_mockup_api_v1_sudoai_2d_mockups__mockup_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sudoai/2d-mockups/{mockup_id}\n  method: delete\n  operationId: delete_2d_mockup_api_v1_sudoai_2d_mockups__mockup_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sudoai/2d-mockups/{mockup_id}/render\n  method: post\n  operationId:\
  \ render_2d_mockup_public_api_v1_sudoai_2d_mockups__mockup_id__render_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/studio/create-session\n  method: post\n  operationId: create_studio_session_api_v1_studio_create_session_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/studio/config\n  method: get\n  operationId: get_studio_config_api_v1_studio_config_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/studio/config\n  method: put\n  operationId: update_studio_config_api_v1_studio_config_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/studio/actions/consume\n  method: post\n  operationId: consume_action_api_v1_studio_actions_consume_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/sudomock-com/agentic-access/sudomock-com-agentic-access.yml
summary_line: 53 operations · 30 acting
tags:
- Mockup
- PSD
- E-Commerce
- Automation
---
