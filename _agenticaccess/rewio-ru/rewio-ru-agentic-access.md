---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 25
api_specs:
- filename: rewio-ru-analytics-api-openapi.yml
  format: yaml
  label: rewio-ru Analytics API
  slug: rewio-ru-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rewio-ru/openapi/rewio-ru-analytics-api-openapi.yml
- filename: rewio-ru-complaints-api-openapi.yml
  format: yaml
  label: rewio-ru Complaints API
  slug: rewio-ru-complaints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rewio-ru/openapi/rewio-ru-complaints-api-openapi.yml
- filename: rewio-ru-folders-api-openapi.yml
  format: yaml
  label: rewio-ru Folders API
  slug: rewio-ru-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rewio-ru/openapi/rewio-ru-folders-api-openapi.yml
- filename: rewio-ru-health-api-openapi.yml
  format: yaml
  label: rewio-ru Health API
  slug: rewio-ru-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rewio-ru/openapi/rewio-ru-health-api-openapi.yml
- filename: rewio-ru-hidden-pinned-api-openapi.yml
  format: yaml
  label: rewio-ru hidden & pinned API
  slug: rewio-ru-hidden-pinned-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rewio-ru/openapi/rewio-ru-hidden-pinned-api-openapi.yml
- filename: rewio-ru-links-api-openapi.yml
  format: yaml
  label: rewio-ru Links API
  slug: rewio-ru-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rewio-ru/openapi/rewio-ru-links-api-openapi.yml
- filename: rewio-ru-objects-api-openapi.yml
  format: yaml
  label: rewio-ru Objects API
  slug: rewio-ru-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rewio-ru/openapi/rewio-ru-objects-api-openapi.yml
- filename: rewio-ru-replies-api-openapi.yml
  format: yaml
  label: rewio-ru Replies API
  slug: rewio-ru-replies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rewio-ru/openapi/rewio-ru-replies-api-openapi.yml
- filename: rewio-ru-reviews-api-openapi.yml
  format: yaml
  label: rewio-ru Reviews API
  slug: rewio-ru-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rewio-ru/openapi/rewio-ru-reviews-api-openapi.yml
- filename: rewio-ru-sources-api-openapi.yml
  format: yaml
  label: rewio-ru Sources API
  slug: rewio-ru-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rewio-ru/openapi/rewio-ru-sources-api-openapi.yml
- filename: rewio-ru-support-api-openapi.yml
  format: yaml
  label: rewio-ru Support API
  slug: rewio-ru-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rewio-ru/openapi/rewio-ru-support-api-openapi.yml
- filename: rewio-ru-webhooks-api-openapi.yml
  format: yaml
  label: rewio-ru Webhooks API
  slug: rewio-ru-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rewio-ru/openapi/rewio-ru-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 25
  write: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rewio Ru Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/support/message
operation_count: 53
overview: 'rewio-ru exposes 53 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 27 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: rewio-ru
provider_slug: rewio-ru
slug: rewio-ru-agentic-access
source_filename: rewio-ru-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/rewio-ru-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    connected: 25\n    acting: 28\n  by_consequence:\n    read: 25\n    write: 27\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health/read\n  method: get\n  operationId: read_health_check_health_read_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v3/reviews/sync\n  method: get\n  operationId: sync_reviews_v3_v3_reviews_sync_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reviews\n  method: get\n  operationId: get_reviews_v3_v3_reviews_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reviews/{review_id}\n  method: get\n  operationId: get_review_v3_v3_reviews__review_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/ratings\n  method: get\n  operationId: get_ratings_v3_v3_ratings_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/ratings/history\n  method: get\n  operationId:\
  \ get_ratings_history_v3_v3_ratings_history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/objects\n  method: post\n  operationId: create_object_v3_v3_objects_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/objects\n  method: get\n  operationId: list_objects_v3_v3_objects_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/objects\n  method: put\n  operationId: switch_objects_v3_v3_objects_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/objects/refresh\n  method: get\n  operationId: list_object_refresh_v3_v3_objects_refresh_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/objects/{object_id}\n  method: get\n  operationId: get_object_v3_v3_objects__object_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/objects/{object_id}\n  method: put\n  operationId: update_object_v3_v3_objects__object_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /v3/objects/{object_id}\n  method: delete\n  operationId: delete_object_v3_v3_objects__object_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/objects/{object_id}/refresh\n  method: get\n  operationId: get_object_refresh_v3_v3_objects__object_id__refresh_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/objects/{object_id}/refresh\n  method: post\n  operationId: refresh_object_v3_v3_objects__object_id__refresh_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/objects/{object_id}/links\n  method: post\n  operationId: add_links_v3_v3_objects__object_id__links_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/objects/{object_id}/links\n  method: get\n  operationId: list_links_v3_v3_objects__object_id__links_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/objects/{object_id}/links/{link_id}\n  method: put\n  operationId: update_link_v3_v3_objects__object_id__links__link_id__put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/objects/{object_id}/links/{link_id}\n  method: delete\n  operationId: remove_link_v3_v3_objects__object_id__links__link_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/objects/{object_id}/hidden-reviews\n  method: post\n  operationId: hide_reviews_v3_v3_objects__object_id__hidden_reviews_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v3/objects/{object_id}/hidden-reviews\n  method: delete\n  operationId: unhide_reviews_v3_v3_objects__object_id__hidden_reviews_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/objects/{object_id}/hidden-reviews\n  method: get\n  operationId: list_hidden_reviews_v3_v3_objects__object_id__hidden_reviews_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/objects/{object_id}/pinned-reviews\n  method: put\n  operationId: set_pinned_reviews_v3_v3_objects__object_id__pinned_reviews_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/objects/{object_id}/pinned-reviews\n  method: post\n  operationId: add_pinned_reviews_v3_v3_objects__object_id__pinned_reviews_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/objects/{object_id}/pinned-reviews\n  method: delete\n  operationId: remove_pinned_reviews_v3_v3_objects__object_id__pinned_reviews_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v3/objects/{object_id}/pinned-reviews\n  method: get\n  operationId: list_pinned_reviews_v3_v3_objects__object_id__pinned_reviews_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/folders\n  method: post\n  operationId: create_folder_v3_v3_folders_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/folders\n  method: get\n  operationId: list_folders_v3_v3_folders_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/folders/{folder_id}\n  method: get\n  operationId: get_folder_v3_v3_folders__folder_id__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/folders/{folder_id}\n  method: patch\n  operationId: update_folder_v3_v3_folders__folder_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/folders/{folder_id}\n  method: delete\n  operationId: delete_folder_v3_v3_folders__folder_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/folders/{folder_id}/refresh\n  method: get\n  operationId: get_folder_refresh_v3_v3_folders__folder_id__refresh_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/folders/{folder_id}/refresh\n  method: post\n  operationId: refresh_folder_v3_v3_folders__folder_id__refresh_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/analytics\n  method: get\n  operationId: get_analytics_v3_v3_analytics_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/analytics/timeseries\n  method: get\n  operationId: get_timeseries_v3_v3_analytics_timeseries_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v3/sources\n  method: get\n  operationId: list_sources_v3_v3_sources_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/webhooks\n  method: get\n  operationId: list_webhooks_v3_v3_webhooks_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/webhooks\n  method: post\n  operationId: create_webhook_v3_v3_webhooks_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/webhooks/secret\n  method: get\n  operationId: get_account_secret_v3_v3_webhooks_secret_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/webhooks/rotate-secret\n  method: post\n  operationId: rotate_account_secret_v3_v3_webhooks_rotate_secret_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/webhooks/{webhook_id}\n  method: patch\n  operationId: update_webhook_v3_v3_webhooks__webhook_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/webhooks/{webhook_id}\n  method: delete\n  operationId: delete_webhook_v3_v3_webhooks__webhook_id__delete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/webhooks/{webhook_id}/test\n  method: post\n  operationId: test_webhook_v3_v3_webhooks__webhook_id__test_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/reviews/{review_id}/reply\n  method: get\n  operationId: get_reply_v3_v3_reviews__review_id__reply_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reviews/{review_id}/reply\n  method: put\n  operationId:\
  \ put_reply_v3_v3_reviews__review_id__reply_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/reviews/{review_id}/reply\n  method: delete\n  operationId: delete_reply_v3_v3_reviews__review_id__reply_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/reviews/{review_id}/complaints\n  method: get\n  operationId: get_review_complaints_v3_v3_reviews__review_id__complaints_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v3/reviews/{review_id}/complaints\n  method: post\n  operationId: post_review_complaint_v3_v3_reviews__review_id__complaints_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/support/message\n  method: post\n  operationId: send_support_message_v3_v3_support_message_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/reviews/{review_id}/skip\n  method: put\n  operationId: skip_review_v3_v3_reviews__review_id__skip_put\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/reviews/{review_id}/skip\n  method: delete\n  operationId: unskip_review_v3_v3_reviews__review_id__skip_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/complaints\n  method: get\n  operationId: get_complaints_v3_v3_complaints_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/rewio-ru/agentic-access/rewio-ru-agentic-access.yml
summary_line: 53 operations · 28 acting
tags:
- Reviews
- Aggregation
- Russian
- Maps
---
