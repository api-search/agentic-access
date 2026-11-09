---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 15
api_specs:
- filename: idphoto-ai-id-photo-api-v1-api-openapi.yml
  format: yaml
  label: idphoto-ai ID Photo API V1 API
  slug: idphoto-ai-id-photo-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/idphoto-ai/openapi/idphoto-ai-id-photo-api-v1-api-openapi.yml
- filename: idphoto-ai-id-photo-api-v2-api-openapi.yml
  format: yaml
  label: idphoto-ai ID Photo API V2 API
  slug: idphoto-ai-id-photo-api-v2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/idphoto-ai/openapi/idphoto-ai-id-photo-api-v2-api-openapi.yml
- filename: idphoto-ai-misc-api-openapi.yml
  format: yaml
  label: idphoto-ai Misc API
  slug: idphoto-ai-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/idphoto-ai/openapi/idphoto-ai-misc-api-openapi.yml
consequence_counts:
  read: 15
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Idphoto Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 34
overview: 'idphoto-ai exposes 34 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 19 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: idphoto-ai
provider_slug: idphoto-ai
slug: idphoto-ai-agentic-access
source_filename: idphoto-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/idphoto-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 15\n    acting: 19\n  by_consequence:\n    read: 15\n    write: 19\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/getSignedUrl\n  method: post\n  operationId: get_signed_url_v1_getSignedUrl_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/getIdPhotoWatermark/{tempAuthKey}\n  method: post\n  operationId: make_id_photo_watermark_with_key_v1_getIdPhotoWatermark__tempAuthKey__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/getFullPhotoNoBg\n  method: post\n  operationId: get_full_photo_no_bg_v1_getFullPhotoNoBg_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/getIdPhotoNoWatermark\n  method: post\n  operationId: getIdPhotoNoWatermark_v1_getIdPhotoNoWatermark_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/remake\n  method: post\n  operationId: remake_v1_remake_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/health\n  method: get\n  operationId: do_health_check_v2_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/make-id-photo\n  method: post\n  operationId: make_id_photo_v2_make_id_photo_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/makeIdPhoto\n  method: post\n  operationId: make_id_photo_v2_makeIdPhoto_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/makeIdPhotoWatermark\n  method: post\n  operationId: make_id_photo_watermark_v2_makeIdPhotoWatermark_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/getIdPhotoNoWatermark\n  method: post\n  operationId: get_id_photo_no_watermark_v2_getIdPhotoNoWatermark_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/getSignedUrl\n  method: post\n  operationId: get_signed_url_v2_getSignedUrl_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/getIdPhotoWatermark/{tempAuthKey}\n  method:\
  \ post\n  operationId: make_id_photo_watermark_with_key_v2_getIdPhotoWatermark__tempAuthKey__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/remake\n  method: post\n  operationId: remake_v2_remake_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/getFullPhotoNoBg\n  method: post\n  operationId: get_full_photo_no_bg_v2_getFullPhotoNoBg_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/invalidateSpecCache\n\
  \  method: get\n  operationId: invalidate_spec_cache_v2_invalidateSpecCache_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/verifyIdPhoto\n  method: post\n  operationId: verify_id_photo_spec_v2_verifyIdPhoto_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/validateIdPhoto\n  method: post\n  operationId: validate_id_photo_spec_v2_validateIdPhoto_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/getIdPhotoSpec\n\
  \  method: post\n  operationId: get_id_photo_spec_v2_getIdPhotoSpec_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/listIdPhotoSpecCode\n  method: post\n  operationId: list_id_photo_spec_code_v2_listIdPhotoSpecCode_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/makeAiPassportPhoto\n  method: post\n  operationId: make_ai_passport_photo_v2_makeAiPassportPhoto_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/removeBackgroundInternal\n  method: post\n  operationId: remove_background_internal_by_ali_segment_v2_removeBackgroundInternal_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/removeBackground\n  method: post\n  operationId: remove_background_v2_removeBackground_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/removeBackgroundFast\n  method: post\n  operationId: remove_background_fast_v2_removeBackgroundFast_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /v2/photoEnhance\n  method: post\n  operationId: photo_enhance_v2_photoEnhance_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/removeShadow\n  method: post\n  operationId: remove_shadow_v2_removeShadow_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/fixShoulder\n  method: post\n  operationId: fix_shoulder_v2_fixShoulder_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/aiEdit\n  method: post\n  operationId: ai_edit_v2_aiEdit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/updateIdPhotoUserMetadata\n  method: post\n  operationId: update_id_photo_user_metadata_v2_updateIdPhotoUserMetadata_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/queryAccountStatus\n  method: post\n  operationId: query_account_status_v2_queryAccountStatus_post\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/faceMatch\n  method: post\n  operationId: face_match_v2_faceMatch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /misc/health\n  method: get\n  operationId: do_health_check_misc_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /misc/versionSsss\n  method: get\n  operationId: version_check_misc_versionSsss_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /misc/region\n\
  \  method: get\n  operationId: region_check_misc_region_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /misc/dailyUsage\n  method: post\n  operationId: query_daily_usage_misc_dailyUsage_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/idphoto-ai/agentic-access/idphoto-ai-agentic-access.yml
summary_line: 34 operations · 19 acting
tags:
- Artificial Intelligence
- Photos
- Identity
- Passport
- Visa
- Image Processing
---
