---
acting_count: 1218
action_class_counts:
  acting: 1218
  connected: 1166
api_specs:
- filename: automattic-wordpress-com-rest-v1-1-openapi.yml
  format: yaml
  label: WordPress.com REST API v1.1
  slug: wordpresscom-rest-api-v11
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-rest-v1-1-openapi.yml
- filename: automattic-wordpress-com-rest-v1-2-openapi.yml
  format: yaml
  label: WordPress.com REST API v1.2
  slug: wordpresscom-rest-api-v12
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-rest-v1-2-openapi.yml
- filename: automattic-wordpress-com-rest-v1-3-openapi.yml
  format: yaml
  label: WordPress.com REST API v1.3
  slug: wordpresscom-rest-api-v13
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-rest-v1-3-openapi.yml
- filename: automattic-wordpress-com-wp-v2-openapi.yml
  format: yaml
  label: WordPress.com REST API - wp/v2 namespace
  slug: wordpresscom-rest-api-wpv2-namespace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-wp-v2-openapi.yml
- filename: automattic-wordpress-com-wpcom-v2-openapi.yml
  format: yaml
  label: WordPress.com REST API - wpcom/v2 namespace
  slug: wordpresscom-rest-api-wpcomv2-namespace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-wpcom-v2-openapi.yml
- filename: automattic-akismet-openapi.yml
  format: yaml
  label: Akismet API
  slug: akismet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-akismet-openapi.yml
- filename: automattic-jetpack-ai-plugin-openapi.yaml
  format: yaml
  label: Jetpack AI-Plugin API
  slug: jetpack-ai-plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-jetpack-ai-plugin-openapi.yaml
consequence_counts:
  physical: 96
  read: 1166
  safety-critical: 20
  write: 1102
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 20
kind: agentic-access
layout: agentic-access
method: generated
name: Automattic Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/experiments/0.1.0/experiments/preset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/experiments/0.1.0/flags/preset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/gravatar/developers/applications/{app_id}/reset-secret
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /wpcom/v2/gravatar/developers/applications/{app_id}/reset-secret
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /wpcom/v2/gravatar/developers/applications/{app_id}/reset-secret
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/jetpack-partners/{partner_id}/key/{key_id}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /wpcom/v2/jetpack-partners/{partner_id}/key/{key_id}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /wpcom/v2/jetpack-partners/{partner_id}/key/{key_id}/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/reader/greader/api/greader.php/reader/api/0/disable-tag
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/reader/greader/greader.php/reader/api/0/disable-tag
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/reader/greader/reader/api/0/disable-tag
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/sites/{wpcom_site}/invites/links/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/sites/{wpcom_site}/posts-to-podcast
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/sites/{wpcom_site}/posts-to-podcast/post-publish-promo/dismiss
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/sites/{wpcom_site}/reset-migration
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/sites/{wpcom_site}/reset-site
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/sites/{wpcom_site}/site-importer/paid-newsletter/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/sites/{wpcom_site}/subscribers/import/reset-state
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /wpcom/v2/sites/{wpcom_site}/subscribers/import/reset_state
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /wpcom/v2/sites/{wpcom_site}/wc/partners/{partner}/revoke-token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /manual_payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /me/two-step/sms/new
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sites/{site}/posts/delete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sites/{site}/posts/{post_ID}/delete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wp/v2/sites/{wpcom_site}/jp_pay_order
operation_count: 2384
overview: 'Automattic exposes 2384 API operations that an AI agent could call, of which 1218 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1166 read, 1102 write, 96 physical, and 20 safety-critical.


  20 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Automattic
provider_slug: automattic
slug: automattic-agentic-access
source_filename: automattic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: generated\nsource: openapi/automattic-akismet-openapi.yml, openapi/automattic-jetpack-ai-plugin-openapi.yaml,\n  openapi/automattic-wordpress-com-rest-v1-1-openapi.yml, openapi/automattic-wordpress-com-rest-v1-2-openapi.yml,\n  openapi/automattic-wordpress-com-rest-v1-3-openapi.yml, openapi/automattic-wordpress-com-wp-v2-openapi.yml,\n  openapi/automattic-wordpress-com-wpcom-v2-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2384\n  by_action_class:\n    acting: 1218\n    connected: 1166\n  by_consequence:\n    write: 1102\n    read: 1166\n    physical: 96\n    safety-critical: 20\n  human_in_the_loop_required: 20\noperations:\n- path: /1.1/verify-key\n  method: post\n  operationId: postVerifyKey\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.1/comment-check\n  method: post\n  operationId: postCommentCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.1/submit-spam\n  method: post\n  operationId: postSubmitSpam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.1/submit-ham\n\
  \  method: post\n  operationId: postSubmitHam\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /1.2/key-sites\n  method: get\n  operationId: getKeySites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /1.2/usage-limit\n  method: get\n  operationId: getUsageLimit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wpcom/v2/ai-plugin/sites\n  method: get\n  operationId: getSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wpcom/v2/sites/{site_id}/ai-plugin/posts\n\
  \  method: get\n  operationId: getPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wpcom/v2/sites/{site_id}/ai-plugin/posts\n  method: post\n  operationId: createPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wpcom/v2/sites/{site_id}/ai-plugin/posts/{post_id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch/\n  method: get\n  operationId: getBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /freshly-pressed/\n  method: get\n  operationId: getFreshlyPressed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights\n  method: get\n  operationId: getInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/{slug}\n  method: get\n  operationId: getInsightsBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jetpack-blogs/\n  method: get\n  operationId: getJetpackBlogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jetpack-blogs/{blog_id}/\n  method: get\n  operationId: getJetpackBlogsByBlogId\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jetpack-blogs/{blog_id}/\n  method: post\n  operationId: postJetpackBlogsByBlogId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jetpack-blogs/{blog_id}/mine/delete\n  method: post\n  operationId: postJetpackBlogsByBlogIdMineDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jetpack-blogs/{blog_id}/test-connection\n  method: get\n  operationId: getJetpackBlogsByBlogIdTestConnection\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jetpack-blogs/{dest_blog_id}/source/{source_blog_id}/migrate/\n  method: post\n  operationId: postJetpackBlogsByDestBlogIdSourceBySourceBlogIdMigrate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /manual_payment\n  method: post\n  operationId: postManualPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /manual_payment/%s\n \
  \ method: get\n  operationId: getManualPaymentS\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketing/survey\n  method: post\n  operationId: postMarketingSurvey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/billing-history\n  method: get\n  operationId: getMeBillingHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/connected-applications/\n\
  \  method: get\n  operationId: getMeConnectedApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/connected-applications/{ID}\n  method: get\n  operationId: getMeConnectedApplicationsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/connected-applications/{ID}/delete\n  method: post\n  operationId: postMeConnectedApplicationsByIdDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/keyring-connections/\n  method: get\n  operationId: getMeKeyringConnections\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/keyring-connections/{keyring_connection_ID}\n  method: get\n  operationId: getMeKeyringConnectionsByKeyringConnectionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/keyring-connections/{keyring_connection_ID}/delete\n  method: post\n  operationId: postMeKeyringConnectionsByKeyringConnectionIdDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/likes/\n  method: get\n  operationId: getMeLikes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /me/mailboxes\n  method: get\n  operationId: getMeMailboxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/posts\n  method: get\n  operationId: getMePosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/preferences/\n  method: get\n  operationId: getMePreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/preferences/\n  method: post\n  operationId: postMePreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/publicize-connections/\n\
  \  method: get\n  operationId: getMePublicizeConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/publicize-connections/{publicize_connection_ID}\n  method: get\n  operationId: getMePublicizeConnectionsByPublicizeConnectionId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/publicize-connections/{publicize_connection_ID}\n  method: post\n  operationId: postMePublicizeConnectionsByPublicizeConnectionId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/publicize-connections/{publicize_connection_ID}/delete\n  method: post\n  operationId:\
  \ postMePublicizeConnectionsByPublicizeConnectionIdDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/settings/\n  method: get\n  operationId: getMeSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/settings/\n  method: post\n  operationId: postMeSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/settings/password/validate\n  method: post\n  operationId: postMeSettingsPasswordValidate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/settings/profile-links/\n  method: get\n  operationId: getMeSettingsProfileLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/settings/profile-links/new\n  method: post\n  operationId: postMeSettingsProfileLinksNew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/settings/profile-links/{slug}/delete\n  method: post\n  operationId: postMeSettingsProfileLinksBySlugDelete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/sites\n  method: get\n  operationId: getMeSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/sites/compact\n  method: get\n  operationId: getMeSitesCompact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/sites/features\n  method: get\n  operationId: getMeSitesFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/sites/plugins\n  method: get\n  operationId: getMeSitesPlugins\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/two-step\n  method: get\n  operationId: getMeTwoStep\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/two-step/sms/new\n  method: post\n  operationId: postMeTwoStepSmsNew\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /meta/external-services/\n  method: get\n  operationId: getMetaExternalServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /meta/external-services/{service}\n  method: get\n  operationId: getMetaExternalServicesByService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meta/sharing-buttons\n  method: get\n  operationId: getMetaSharingButtons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/read\n  method: post\n  operationId: postNotificationsRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications/seen\n  method: post\n  operationId: postNotificationsSeen\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /read/email-settings/\n  method: get\n  operationId: getReadEmailSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/email-settings/\n  method: post\n  operationId: postReadEmailSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /read/feed/\n  method: get\n  operationId: getReadFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /read/feed/{feed_url_or_id}\n  method: get\n  operationId: getReadFeedByFeedUrlOrId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/following/\n  method: get\n  operationId: getReadFollowing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/following/mine\n  method: get\n  operationId: getReadFollowingMine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/following/mine/delete\n  method: post\n  operationId: postReadFollowingMineDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /read/following/mine/new\n  method: post\n  operationId: postReadFollowingMineNew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /read/liked/\n  method: get\n  operationId: getReadLiked\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/lists/{user_slug}\n  method: get\n  operationId: getReadListsByUserSlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/menu/\n  method: get\n  operationId: getReadMenu\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/recommendations/mine/\n  method: get\n  operationId: getReadRecommendationsMine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/sites/{site}/posts/{post_ID}\n  method: get\n  operationId: getReadSitesBySitePostsByPostId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/subscriptions-count/\n  method: get\n  operationId: getReadSubscriptionsCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/tags\n  method: get\n  operationId: getReadTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /read/tags/alphabetic\n  method: get\n  operationId: getReadTagsAlphabetic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/tags/{tag}\n  method: get\n  operationId: getReadTagsByTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/tags/{tag}/mine\n  method: get\n  operationId: getReadTagsByTagMine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/tags/{tag}/mine/delete\n  method: post\n  operationId: postReadTagsByTagMineDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /read/tags/{tag}/mine/new\n  method: post\n  operationId: postReadTagsByTagMineNew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /read/tags/{tag}/posts\n  method: get\n  operationId: getReadTagsByTagPosts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /read/trending/tags\n  method: get\n  operationId: getReadTrendingTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}\n  method: get\n  operationId: getSitesBySite\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/automated-transfers/status\n  method: get\n  operationId: getSitesBySiteAutomatedTransfersStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/categories\n  method: get\n  operationId: getSitesBySiteCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/categories/new\n  method: post\n  operationId: postSitesBySiteCategoriesNew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/categories/slug:{category}\n\
  \  method: get\n  operationId: getSitesBySiteCategoriesSlugCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/categories/slug:{category}\n  method: post\n  operationId: postSitesBySiteCategoriesSlugCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/categories/slug:{category}/delete\n  method: post\n  operationId: postSitesBySiteCategoriesSlugCategoryDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /sites/{site}/comment-counts\n  method: get\n  operationId: getSitesBySiteCommentCounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/comment-history/{comment_ID}\n  method: get\n  operationId: getSitesBySiteCommentHistoryByCommentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/comments-tree\n  method: get\n  operationId: getSitesBySiteCommentsTree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/comments/\n  method: get\n  operationId: getSitesBySiteComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /sites/{site}/comments/{comment_ID}\n  method: get\n  operationId: getSitesBySiteCommentsByCommentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/comments/{comment_ID}\n  method: post\n  operationId: postSitesBySiteCommentsByCommentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/comments/{comment_ID}/delete\n  method: post\n  operationId: postSitesBySiteCommentsByCommentIdDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/comments/{comment_ID}/likes/\n  method: get\n  operationId: getSitesBySiteCommentsByCommentIdLikes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/comments/{comment_ID}/likes/mine/\n  method: get\n  operationId: getSitesBySiteCommentsByCommentIdLikesMine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/comments/{comment_ID}/likes/mine/delete\n  method: post\n  operationId: postSitesBySiteCommentsByCommentIdLikesMineDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /sites/{site}/comments/{comment_ID}/likes/new\n  method: post\n  operationId: postSitesBySiteCommentsByCommentIdLikesNew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/comments/{comment_ID}/replies/new\n  method: post\n  operationId: postSitesBySiteCommentsByCommentIdRepliesNew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/dropdown-pages/\n  method: get\n  operationId: getSitesBySiteDropdownPages\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/embeds\n  method: get\n  operationId: getSitesBySiteEmbeds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/embeds/render\n  method: get\n  operationId: getSitesBySiteEmbedsRender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/followers\n  method: get\n  operationId: getSitesBySiteFollowers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/followers/{subscriber_id}\n  method: get\n  operationId: getSitesBySiteFollowersBySubscriberId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/follows/\n  method: get\n  operationId: getSitesBySiteFollows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/follows/mine\n  method: get\n  operationId: getSitesBySiteFollowsMine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/follows/mine/delete\n  method: post\n  operationId: postSitesBySiteFollowsMineDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/follows/new\n  method: post\n  operationId: postSitesBySiteFollowsNew\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/headers/mine\n  method: get\n  operationId: getSitesBySiteHeadersMine\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/headers/mine\n  method: post\n  operationId: postSitesBySiteHeadersMine\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/headers/{theme_slug}\n  method: get\n  operationId: getSitesBySiteHeadersByThemeSlug\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/imports/\n  method: get\n  operationId: getSitesBySiteImports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/imports/library/new\n  method: post\n  operationId: postSitesBySiteImportsLibraryNew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/imports/new\n  method: post\n  operationId: postSitesBySiteImportsNew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/imports/{import_id}\n  method: get\n  operationId: getSitesBySiteImportsByImportId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site}/imports/{import_id}\n  method: post\n  operationId: postSitesBySiteImportsByImportId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sites/{site}/invites/new\n  method: post\n  operationId: postSitesBySiteInvitesNew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: c\n\n# --- truncated at 32 KB (769 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/agentic-access/automattic-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/agentic-access/automattic-agentic-access.yml
summary_line: 2384 operations · 1218 acting · 20 human-in-the-loop
tags:
- Company
- Content Management
- Publishing
- Blogging
- Website Hosting
- Web Publishing
- Content
- Comments
- Spam Filtering
- Media
- Analytics
- Domains
- E-Commerce
- Open Source
- Developer Tools
- Model Context Protocol
---
