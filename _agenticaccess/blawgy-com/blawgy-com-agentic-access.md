---
acting_count: 130
action_class_counts:
  acting: 130
  connected: 72
api_specs:
- filename: blawgy-com-account-api-openapi.yml
  format: yaml
  label: blawgy-com Account API
  slug: blawgy-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-account-api-openapi.yml
- filename: blawgy-com-articles-api-openapi.yml
  format: yaml
  label: blawgy-com Articles API
  slug: blawgy-com-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-articles-api-openapi.yml
- filename: blawgy-com-builder-api-openapi.yml
  format: yaml
  label: blawgy-com Builder API
  slug: blawgy-com-builder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-builder-api-openapi.yml
- filename: blawgy-com-existing-pages-api-openapi.yml
  format: yaml
  label: blawgy-com Existing pages API
  slug: blawgy-com-existing-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-existing-pages-api-openapi.yml
- filename: blawgy-com-images-api-openapi.yml
  format: yaml
  label: blawgy-com Images API
  slug: blawgy-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-images-api-openapi.yml
- filename: blawgy-com-integrations-api-openapi.yml
  format: yaml
  label: blawgy-com Integrations API
  slug: blawgy-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-integrations-api-openapi.yml
- filename: blawgy-com-keywords-api-openapi.yml
  format: yaml
  label: blawgy-com Keywords API
  slug: blawgy-com-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-keywords-api-openapi.yml
- filename: blawgy-com-location-pages-api-openapi.yml
  format: yaml
  label: blawgy-com Location pages API
  slug: blawgy-com-location-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-location-pages-api-openapi.yml
- filename: blawgy-com-metrics-api-openapi.yml
  format: yaml
  label: blawgy-com Metrics API
  slug: blawgy-com-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-metrics-api-openapi.yml
- filename: blawgy-com-partner-api-openapi.yml
  format: yaml
  label: blawgy-com Partner API
  slug: blawgy-com-partner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-partner-api-openapi.yml
- filename: blawgy-com-plan-api-openapi.yml
  format: yaml
  label: blawgy-com Plan API
  slug: blawgy-com-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-plan-api-openapi.yml
- filename: blawgy-com-products-api-openapi.yml
  format: yaml
  label: blawgy-com Products API
  slug: blawgy-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-products-api-openapi.yml
- filename: blawgy-com-public-content-api-openapi.yml
  format: yaml
  label: blawgy-com Public content API
  slug: blawgy-com-public-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-public-content-api-openapi.yml
- filename: blawgy-com-refresh-api-openapi.yml
  format: yaml
  label: blawgy-com Refresh API
  slug: blawgy-com-refresh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-refresh-api-openapi.yml
- filename: blawgy-com-settings-api-openapi.yml
  format: yaml
  label: blawgy-com Settings API
  slug: blawgy-com-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-settings-api-openapi.yml
- filename: blawgy-com-support-api-openapi.yml
  format: yaml
  label: blawgy-com Support API
  slug: blawgy-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-support-api-openapi.yml
- filename: blawgy-com-team-and-billing-api-openapi.yml
  format: yaml
  label: blawgy-com Team and billing API
  slug: blawgy-com-team-and-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-team-and-billing-api-openapi.yml
- filename: blawgy-com-updates-api-openapi.yml
  format: yaml
  label: blawgy-com Updates API
  slug: blawgy-com-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-updates-api-openapi.yml
- filename: blawgy-com-webhooks-api-openapi.yml
  format: yaml
  label: blawgy-com Webhooks API
  slug: blawgy-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blawgy-com/openapi/blawgy-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 72
  safety-critical: 2
  write: 126
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Blawgy Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /me/credentials/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /sites/{site}/team/invites/{inviteId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sites/{site}/team/invites/{inviteId}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sites/{site}/webhooks/{webhookId}/test
operation_count: 202
overview: 'blawgy-com exposes 202 API operations that an AI agent could call, of which 130 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 72 read, 126 write, 2 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: blawgy-com
provider_slug: blawgy-com
slug: blawgy-com-agentic-access
source_filename: blawgy-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/blawgy-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 202\n  by_action_class:\n    connected: 72\n    acting: 130\n  by_consequence:\n    read: 72\n    write: 126\n    safety-critical: 2\n    physical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /help/search\n  method: get\n  operationId: search_help\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: whoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/credentials\n\
  \  method: get\n  operationId: list_api_credentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/credentials\n  method: post\n  operationId: create_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/credentials/{id}\n  method: delete\n  operationId: revoke_api_credential\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /me/notifications\n  method: get\n  operationId:\
  \ get_notification_prefs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/notifications\n  method: patch\n  operationId: update_notification_prefs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/usage\n  method: get\n  operationId: get_api_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: get_openapi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/clients\n  method: get\n \
  \ operationId: list_clients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/clients\n  method: post\n  operationId: create_client\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/clients/{clientId}/approve\n  method: post\n  operationId: approve_client\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/clients/{clientId}/decline\n  method: post\n  operationId: decline_client\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/domain\n  method: put\n  operationId: set_partner_domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/domain\n  method: delete\n  operationId: remove_partner_domain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/guardrails\n  method:\
  \ get\n  operationId: list_partner_guardrails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/guardrails\n  method: post\n  operationId: create_partner_guardrail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/guardrails/{guardrailId}\n  method: patch\n  operationId: update_partner_guardrail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/guardrails/{guardrailId}\n  method: delete\n  operationId:\
  \ delete_partner_guardrail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/logo\n  method: post\n  operationId: upload_partner_logo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /partner/report\n  method: get\n  operationId: get_client_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/settings\n  method: get\n  operationId: get_partner_settings\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /partner/settings\n  method: patch\n  operationId: update_partner_settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/sites/{site}/posts\n  method: get\n  operationId: list_public_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/sites/{site}/posts/{slugOrId}\n  method: get\n  operationId: get_public_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites\n  method: get\n  operationId: list_sites\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites\n  method: post\n  operationId: create_site\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/analyze\n  method: post\n  operationId: analyze_new_site\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}\n  method: delete\n  operationId: delete_site\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/ai-mentions\n  method: get\n  operationId: get_ai_mentions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/ai-mentions/scan\n  method: post\n  operationId: run_ai_mentions_scan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles\n  method: get\n  operationId: list_articles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/articles/bulk-delete\n\
  \  method: post\n  operationId: delete_articles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles/export\n  method: get\n  operationId: export_articles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/articles/write\n  method: post\n  operationId: write_article_now\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles/{id}\n  method: get\n  operationId: get_article\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/articles/{id}\n  method: patch\n  operationId: update_article\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles/{id}\n  method: delete\n  operationId: delete_article\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles/{id}/content\n  method: put\n  operationId: sync_article_content\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles/{id}/preview-url\n  method: get\n  operationId: get_article_preview_url\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/articles/{id}/publish\n  method: post\n  operationId: publish_draft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles/{id}/published\n  method: post\n  operationId: mark_published\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles/{id}/release\n  method: post\n  operationId: release_held_article\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles/{id}/republish\n  method: post\n  operationId: republish_article\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles/{id}/schedule\n\
  \  method: patch\n  operationId: reschedule_article\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles/{id}/versions\n  method: get\n  operationId: list_article_versions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/articles/{id}/versions/{versionId}\n  method: get\n  operationId: get_article_version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/articles/{id}/versions/{versionId}/restore\n  method: post\n  operationId: restore_article_version\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles/{postId}/image\n  method: get\n  operationId: get_post_image\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/articles/{postId}/image/apply\n  method: post\n  operationId: apply_post_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles/{postId}/image/revert\n  method: post\n  operationId: revert_post_image\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/articles/{postId}/image/upload\n  method: post\n  operationId: upload_post_image\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/behavior\n  method: get\n  operationId: get_behavior\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/billing\n  method: get\n  operationId: get_billing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/billing/upgrade-link\n  method: post\n  operationId: get_upgrade_link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/brand-colors/extract\n  method: post\n  operationId: extract_brand_colors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/builder/drafts\n  method: get\n  operationId: list_builder_drafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/builder/drafts\n  method: post\n  operationId: save_builder_draft\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/builder/drafts/{draftId}\n  method: get\n  operationId: get_builder_draft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/builder/drafts/{draftId}\n  method: delete\n  operationId: delete_builder_draft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/builder/images\n  method: post\n  operationId: upload_builder_image\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/builder/outline\n  method: post\n  operationId: generate_outline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/builder/outline/regenerate\n  method: post\n  operationId: regenerate_outline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/builder/publish\n\
  \  method: post\n  operationId: publish_article_from_builder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/builder/remix\n  method: post\n  operationId: remix_from_urls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/builder/sections/regenerate\n  method: post\n  operationId: regenerate_section\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/builder/titles\n  method: post\n  operationId: generate_titles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/builder/write\n  method: post\n  operationId: write_from_outline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/guardrails\n  method: get\n  operationId: get_site_guardrails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /sites/{site}/guardrails\n  method: put\n  operationId: update_site_guardrails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/guardrails/library\n  method: get\n  operationId: list_guardrails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/guardrails/library\n  method: post\n  operationId: create_guardrail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /sites/{site}/guardrails/library/{guardrailId}\n  method: patch\n  operationId: update_guardrail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/guardrails/library/{guardrailId}\n  method: delete\n  operationId: delete_guardrail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/images/posts\n  method: get\n  operationId: list_image_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /sites/{site}/images/usage\n  method: get\n  operationId: get_image_preview_usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/indexing\n  method: get\n  operationId: get_indexing_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/indexing/recheck\n  method: post\n  operationId: recheck_indexing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/integrations/bing\n  method: post\n  operationId: connect_bing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/integrations/bing\n  method: delete\n  operationId: disconnect_bing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/integrations/dutchie\n  method: get\n  operationId: get_dutchie_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/integrations/dutchie\n  method: post\n  operationId: connect_dutchie\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/integrations/dutchie/locations/{locationRef}\n  method: delete\n  operationId: remove_dutchie_location\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/integrations/dutchie/sync\n  method: post\n  operationId: sync_dutchie\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/integrations/gsc\n  method: delete\n  operationId:\
  \ disconnect_gsc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/integrations/gsc/connections/{connectId}\n  method: get\n  operationId: list_gsc_properties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/integrations/gsc/connections/{connectId}\n  method: post\n  operationId: connect_gsc_property\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/integrations/{provider}/connect-link\n\
  \  method: post\n  operationId: get_connect_link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/jobs/{kind}\n  method: get\n  operationId: get_job\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/keywords\n  method: get\n  operationId: get_keywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/keywords\n  method: put\n  operationId: save_keywords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /sites/{site}/keywords/archived\n  method: get\n  operationId: list_archived_keywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/keywords/archived/delete\n  method: post\n  operationId: delete_archived_keywords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/keywords/archived/restore\n  method: post\n  operationId: restore_archived_keywords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /sites/{site}/keywords/brief\n  method: get\n  operationId: get_research_brief\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/keywords/brief\n  method: patch\n  operationId: update_research_brief\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/keywords/brief/regenerate\n  method: post\n  operationId: regenerate_research_brief\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/keywords/exclude\n\
  \  method: post\n  operationId: exclude_keyword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/keywords/mine\n  method: get\n  operationId: list_my_keywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/keywords/mine\n  method: post\n  operationId: add_my_keywords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/keywords/mine/remove\n  method: post\n  operationId: remove_my_keywords\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/keywords/recommendations\n  method: get\n  operationId: get_keyword_recommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/keywords/research\n  method: post\n  operationId: run_keyword_research\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/keywords/research/runs\n  method: get\n  operationId: list_research_runs\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/keywords/research/runs/{runId}\n  method: get\n  operationId: get_research_run\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/keywords/research/status\n  method: get\n  operationId: get_research_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/keywords/restore\n  method: post\n  operationId: restore_keyword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  \n\n# --- truncated at 32 KB (61 KB total) ---\n# Full source: https://artifacts.apis.io/blawgy-com/agentic-access/blawgy-com-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/blawgy-com/agentic-access/blawgy-com-agentic-access.yml
summary_line: 202 operations · 130 acting · 2 human-in-the-loop
tags:
- Content AI
- SEO
- Blog Publishing
- AI Search
- Agency Tools
---
