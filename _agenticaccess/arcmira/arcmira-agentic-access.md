---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 44
api_specs:
- filename: arcmira-channels-api-openapi.yml
  format: yaml
  label: Arcmira Channels API
  slug: arcmira-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcmira/openapi/arcmira-channels-api-openapi.yml
- filename: arcmira-entities-api-openapi.yml
  format: yaml
  label: Arcmira Entities API
  slug: arcmira-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcmira/openapi/arcmira-entities-api-openapi.yml
- filename: arcmira-feedback-api-openapi.yml
  format: yaml
  label: Arcmira Feedback API
  slug: arcmira-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcmira/openapi/arcmira-feedback-api-openapi.yml
- filename: arcmira-mentions-api-openapi.yml
  format: yaml
  label: Arcmira Mentions API
  slug: arcmira-mentions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcmira/openapi/arcmira-mentions-api-openapi.yml
- filename: arcmira-meta-api-openapi.yml
  format: yaml
  label: Arcmira Meta API
  slug: arcmira-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcmira/openapi/arcmira-meta-api-openapi.yml
- filename: arcmira-monitors-api-openapi.yml
  format: yaml
  label: Arcmira Monitors API
  slug: arcmira-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcmira/openapi/arcmira-monitors-api-openapi.yml
- filename: arcmira-recommendations-api-openapi.yml
  format: yaml
  label: Arcmira Recommendations API
  slug: arcmira-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcmira/openapi/arcmira-recommendations-api-openapi.yml
- filename: arcmira-search-api-openapi.yml
  format: yaml
  label: Arcmira Search API
  slug: arcmira-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcmira/openapi/arcmira-search-api-openapi.yml
- filename: arcmira-trackers-api-openapi.yml
  format: yaml
  label: Arcmira Trackers API
  slug: arcmira-trackers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcmira/openapi/arcmira-trackers-api-openapi.yml
- filename: arcmira-transcriptions-api-openapi.yml
  format: yaml
  label: Arcmira Transcriptions API
  slug: arcmira-transcriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcmira/openapi/arcmira-transcriptions-api-openapi.yml
- filename: arcmira-transcripts-api-openapi.yml
  format: yaml
  label: Arcmira Transcripts API
  slug: arcmira-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcmira/openapi/arcmira-transcripts-api-openapi.yml
- filename: arcmira-channels-api-openapi.yml
  format: yaml
  label: Arcmira Channels API
  slug: arcmira-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcmira/openapi/arcmira-channels-api-openapi.yml
consequence_counts:
  physical: 2
  read: 44
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Arcmira Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/signups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/signups
operation_count: 69
overview: 'Arcmira exposes 69 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 44 read, 23 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Arcmira
provider_slug: arcmira
slug: arcmira-agentic-access
source_filename: arcmira-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/arcmira-entities-api-openapi.yml, openapi/arcmira-feedback-api-openapi.yml,\n  openapi/arcmira-mentions-api-openapi.yml, openapi/arcmira-meta-api-openapi.yml, openapi/arcmira-monitors-api-openapi.yml,\n  openapi/arcmira-openapi.json, openapi/arcmira-recommendations-api-openapi.yml, openapi/arcmira-search-api-openapi.yml,\n  openapi/arcmira-trackers-api-openapi.yml, openapi/arcmira-transcriptions-api-openapi.yml,\n  openapi/arcmira-transcripts-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 69\n  by_action_class:\n    connected: 44\n    acting: 25\n  by_consequence:\n    read: 44\n    write: 23\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/entities/resolve\n\
  \  method: get\n  operationId: resolve_entity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/{id}\n  method: get\n  operationId: get_entity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/{id}/momentum\n  method: get\n  operationId: get_entity_momentum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feedback\n  method: post\n  operationId: submit_feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/feedback/{feedback_id}\n\
  \  method: get\n  operationId: get_feedback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mentions\n  method: get\n  operationId: list_mentions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mentions/counts\n  method: get\n  operationId: count_mentions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: get_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/openapi.json\n  method: get\n  operationId: get_openapi_document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: get_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/settings\n  method: patch\n  operationId: update_my_settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signups\n  method: post\n  operationId: create_signup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/signups/verify\n  method: post\n  operationId: verify_signup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors\n  method: get\n  operationId: list_monitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors\n  method: post\n  operationId: create_monitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}\n  method: patch\n  operationId: update_monitor\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}\n  method: delete\n  operationId: delete_monitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}/webhook-secret/rotate\n  method: post\n  operationId: rotate_monitor_webhook_secret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /v1/monitors/{id}/trackers\n  method: get\n  operationId: list_monitor_trackers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors/{id}/trackers\n  method: post\n  operationId: add_monitor_trackers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}/alerts\n  method: get\n  operationId: list_monitor_alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors/{id}/entities\n  method: post\n  operationId: add_monitor_entities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations/slack\n  method: get\n  operationId: list_slack_integrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: get_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/openapi.json\n  method: get\n  operationId: get_openapi_document\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: get_me\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me/settings\n  method: patch\n  operationId: update_my_settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signups\n  method: post\n  operationId: create_signup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signups/verify\n  method: post\n  operationId: verify_signup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/entities/resolve\n  method: get\n  operationId: resolve_entity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/{id}\n  method: get\n  operationId: get_entity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mentions\n  method: get\n  operationId: list_mentions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recommendations\n  method: get\n  operationId: list_recommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/feedback\n  method: post\n  operationId: submit_feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/feedback/{feedback_id}\n  method: get\n  operationId: get_feedback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/channels/{channel_id}/sponsors\n  method: get\n  operationId: list_channel_sponsors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/entities/{id}/momentum\n  method: get\n  operationId: get_entity_momentum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/channels/{channel_id}/coverage\n  method: get\n  operationId: get_channel_coverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/channels/{channel_id}/videos\n  method: get\n  operationId: list_channel_videos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mentions/counts\n  method: get\n  operationId: count_mentions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors\n\
  \  method: get\n  operationId: list_monitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors\n  method: post\n  operationId: create_monitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}\n  method: patch\n  operationId: update_monitor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}\n  method: delete\n  operationId: delete_monitor\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}/webhook-secret/rotate\n  method: post\n  operationId: rotate_monitor_webhook_secret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}/trackers\n  method: get\n  operationId: list_monitor_trackers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors/{id}/trackers\n  method: post\n  operationId: add_monitor_trackers\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/monitors/{id}/alerts\n  method: get\n  operationId: list_monitor_alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/monitors/{id}/entities\n  method: post\n  operationId: add_monitor_entities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrations/slack\n  method: get\n  operationId: list_slack_integrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trackers\n  method: get\n  operationId: list_trackers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trackers/{id}\n  method: patch\n  operationId: update_tracker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trackers/{id}\n  method: delete\n  operationId: delete_tracker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trackers/{id}/alerts\n\
  \  method: get\n  operationId: list_tracker_alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcripts/{video_id}\n  method: get\n  operationId: get_transcript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcripts/{video_id}/quote\n  method: get\n  operationId: quote_transcription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcriptions\n  method: get\n  operationId: list_transcriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recommendations\n  method: get\n  operationId: list_recommendations\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/channels/{channel_id}/sponsors\n  method: get\n  operationId: list_channel_sponsors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trackers\n  method: get\n  operationId: list_trackers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/trackers\n  method: post\n  operationId: create_tracker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trackers/{id}\n  method: patch\n  operationId: update_tracker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trackers/{id}\n  method: delete\n  operationId: delete_tracker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trackers/{id}/alerts\n  method: get\n  operationId: list_tracker_alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcriptions\n  method: get\n  operationId: list_transcriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcripts/{video_id}\n  method: get\n  operationId: get_transcript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transcripts/{video_id}/quote\n  method: get\n  operationId: quote_transcription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/arcmira/agentic-access/arcmira-agentic-access.yml
summary_line: 69 operations · 25 acting
tags:
- Artificial Intelligence
- Search
- YouTube
- Transcripts
- SDK
---
