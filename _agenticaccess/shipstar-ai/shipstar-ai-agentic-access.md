---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 22
api_specs:
- filename: shipstar-ai-authentication-api-openapi.yml
  format: yaml
  label: shipstar-ai Authentication API
  slug: shipstar-ai-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-authentication-api-openapi.yml
- filename: shipstar-ai-banner-api-openapi.yml
  format: yaml
  label: shipstar-ai Banner API
  slug: shipstar-ai-banner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-banner-api-openapi.yml
- filename: shipstar-ai-blog-api-openapi.yml
  format: yaml
  label: shipstar-ai Blog API
  slug: shipstar-ai-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-blog-api-openapi.yml
- filename: shipstar-ai-changelog-api-openapi.yml
  format: yaml
  label: shipstar-ai Changelog API
  slug: shipstar-ai-changelog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-changelog-api-openapi.yml
- filename: shipstar-ai-changelog-subscriptions-api-openapi.yml
  format: yaml
  label: shipstar-ai Changelog Subscriptions API
  slug: shipstar-ai-changelog-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-changelog-subscriptions-api-openapi.yml
- filename: shipstar-ai-health-api-openapi.yml
  format: yaml
  label: shipstar-ai Health API
  slug: shipstar-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-health-api-openapi.yml
- filename: shipstar-ai-kb-api-openapi.yml
  format: yaml
  label: shipstar-ai Kb API
  slug: shipstar-ai-kb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-kb-api-openapi.yml
- filename: shipstar-ai-mailing-lists-api-openapi.yml
  format: yaml
  label: shipstar-ai Mailing Lists API
  slug: shipstar-ai-mailing-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-mailing-lists-api-openapi.yml
- filename: shipstar-ai-team-invitations-api-openapi.yml
  format: yaml
  label: shipstar-ai Team Invitations API
  slug: shipstar-ai-team-invitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipstar-ai/openapi/shipstar-ai-team-invitations-api-openapi.yml
consequence_counts:
  read: 22
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Shipstar Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'shipstar-ai exposes 30 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: shipstar-ai
provider_slug: shipstar-ai
slug: shipstar-ai-agentic-access
source_filename: shipstar-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/shipstar-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 22\n    acting: 8\n  by_consequence:\n    read: 22\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelogs\n  method: get\n  operationId: list_published_changelogs_changelogs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelog/{public_slug}\n\
  \  method: get\n  operationId: get_public_changelog_changelog__public_slug__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelog/{public_slug}/feed\n  method: get\n  operationId: get_public_changelog_feed_changelog__public_slug__feed_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelogs/feed\n  method: get\n  operationId: get_all_changelogs_feed_changelogs_feed_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blogs\n  method: get\n  operationId: list_published_blog_posts_blogs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blog/{public_slug}\n\
  \  method: get\n  operationId: get_public_blog_post_blog__public_slug__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blog/{public_slug}/feed\n  method: get\n  operationId: get_public_blog_feed_blog__public_slug__feed_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blogs/feed\n  method: get\n  operationId: get_all_blogs_feed_blogs_feed_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kb\n  method: get\n  operationId: list_published_kb_articles_kb_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kb/{public_slug}\n  method: get\n  operationId: get_public_kb_articles_kb__public_slug__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banner\n  method: get\n  operationId: get_live_banner_banner_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banner/{public_slug}\n  method: get\n  operationId: get_public_banner_banner__public_slug__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelog/subscribe\n  method: post\n  operationId: subscribe_to_changelog_changelog_subscribe_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /changelog/confirm/{token}\n  method: get\n  operationId: confirm_changelog_subscription_changelog_confirm__token__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelog/unsubscribe/{token}\n  method: get\n  operationId: unsubscribe_from_changelog_changelog_unsubscribe__token__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelog/unsubscribe/{token}\n  method: post\n  operationId: unsubscribe_from_changelog_one_click_changelog_unsubscribe__token__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/unsubscribe/{token}\n\
  \  method: get\n  operationId: unsubscribe_from_mailing_list_email_unsubscribe__token__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/unsubscribe/{token}\n  method: post\n  operationId: unsubscribe_from_mailing_list_one_click_email_unsubscribe__token__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/lists\n  method: get\n  operationId: list_mailing_lists_email_lists_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/lists\n  method: post\n  operationId: create_mailing_list_email_lists_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/lists/{list_id}\n  method: get\n  operationId: get_mailing_list_email_lists__list_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/lists/{list_id}/recipients\n  method: get\n  operationId: list_mailing_list_recipients_email_lists__list_id__recipients_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/lists/{list_id}/recipients\n  method: post\n  operationId: add_mailing_list_recipients_email_lists__list_id__recipients_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/lists/{list_id}/recipients\n  method: put\n  operationId: upsert_mailing_list_recipients_email_lists__list_id__recipients_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/lists/{list_id}/recipients/remove\n  method: post\n  operationId: remove_mailing_list_recipients_email_lists__list_id__recipients_remove_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /email/lists/{list_id}/recipients/export.csv\n  method: get\n  operationId: export_mailing_list_recipients_email_lists__list_id__recipients_export_csv_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/lists/{list_id}/recipients/{identifier}\n  method: delete\n  operationId: remove_mailing_list_recipient_email_lists__list_id__recipients__identifier__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me\n  method: get\n  operationId: get_current_user_me_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /team-invitations/{token}\n  method: get\n  operationId: get_team_invitation_team_invitations__token__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/shipstar-ai/agentic-access/shipstar-ai-agentic-access.yml
summary_line: 30 operations · 8 acting
tags:
- Company
- Marketing
- Developer Tools
- Automation
- Open Source
---
