---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 32
api_specs:
- filename: facebook-graph-api.yaml
  format: yaml
  label: Facebook Graph API
  slug: facebook-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-graph-api.yaml
- filename: facebook-marketing-api.yaml
  format: yaml
  label: Facebook Marketing API
  slug: facebook-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-marketing-api.yaml
- filename: facebook-instagram-api.yaml
  format: yaml
  label: Instagram API
  slug: instagram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-instagram-api.yaml
- filename: facebook-messenger-api.yaml
  format: yaml
  label: Messenger Platform API
  slug: messenger-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-messenger-api.yaml
- filename: facebook-threads-api.yaml
  format: yaml
  label: Threads API
  slug: threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-threads-api.yaml
- filename: facebook-whatsapp-api.yaml
  format: yaml
  label: WhatsApp Business API
  slug: whatsapp-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-whatsapp-api.yaml
consequence_counts:
  physical: 2
  read: 32
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Facebook Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{page-id}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{phone-number-id}/messages
operation_count: 47
overview: 'Facebook exposes 47 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 13 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Facebook
provider_slug: facebook
slug: facebook-agentic-access
source_filename: facebook-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/facebook-graph-api.yaml, openapi/facebook-instagram-api.yaml, openapi/facebook-marketing-api.yaml,\n  openapi/facebook-messenger-api.yaml, openapi/facebook-threads-api.yaml, openapi/facebook-whatsapp-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 47\n  by_action_class:\n    connected: 32\n    acting: 15\n  by_consequence:\n    read: 32\n    write: 13\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /me\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{user-id}\n  method: get\n  operationId: getUser\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{user-id}/feed\n  method: get\n  operationId: getUserFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{user-id}/feed\n  method: post\n  operationId: createPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{page-id}\n  method: get\n  operationId: getPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{page-id}/feed\n  method: get\n  operationId: getPageFeed\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{post-id}\n  method: get\n  operationId: getPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{post-id}\n  method: delete\n  operationId: deletePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{post-id}/comments\n  method: get\n  operationId: getPostComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{post-id}/comments\n  method: post\n  operationId: createComment\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{user-id}/photos\n  method: get\n  operationId: getUserPhotos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{photo-id}\n  method: get\n  operationId: getPhoto\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /debug_token\n  method: get\n  operationId: debugToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ig-user-id}\n  method: get\n  operationId: getInstagramUser\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ig-user-id}/media\n  method: get\n  operationId: listInstagramMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ig-user-id}/media\n  method: post\n  operationId: createInstagramMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{ig-user-id}/media_publish\n  method: post\n  operationId: publishInstagramMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /{media-id}/comments\n  method: get\n  operationId: getInstagramComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ig-user-id}/insights\n  method: get\n  operationId: getInstagramInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ig-user-id}/tags\n  method: get\n  operationId: getInstagramTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad-account-id}\n  method: get\n  operationId: getAdAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad-account-id}/campaigns\n  method: get\n  operationId:\
  \ listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad-account-id}/campaigns\n  method: post\n  operationId: createCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{campaign-id}\n  method: get\n  operationId: getCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad-account-id}/adsets\n  method: get\n  operationId: listAdSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad-account-id}/adsets\n\
  \  method: post\n  operationId: createAdSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /act_{ad-account-id}/ads\n  method: get\n  operationId: listAds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad-account-id}/insights\n  method: get\n  operationId: getAccountInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /act_{ad-account-id}/customaudiences\n  method: get\n  operationId: listCustomAudiences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /act_{ad-account-id}/customaudiences\n  method: post\n  operationId: createCustomAudience\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{page-id}/messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{page-id}/messenger_profile\n  method: get\n  operationId: getMessengerProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /{page-id}/messenger_profile\n  method: post\n  operationId: updateMessengerProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{conversation-id}\n  method: get\n  operationId: getConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{page-id}/conversations\n  method: get\n  operationId: listConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{threads-user-id}\n  method: get\n  operationId: getThreadsUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{threads-user-id}/threads\n  method: post\n  operationId: createThreadsMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{threads-user-id}/threads_publish\n  method: post\n  operationId: publishThreadsMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{threads-media-id}\n  method: get\n  operationId: getThreadsMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /{threads-media-id}/replies\n  method: get\n  operationId: getThreadsReplies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{threads-user-id}/insights\n  method: get\n  operationId: getThreadsInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{phone-number-id}/messages\n  method: post\n  operationId: sendWhatsAppMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{phone-number-id}/media\n  method: post\n  operationId: uploadWhatsAppMedia\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{phone-number-id}\n  method: get\n  operationId: getWhatsAppPhoneNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{waba-id}/message_templates\n  method: get\n  operationId: listMessageTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{waba-id}/message_templates\n  method: post\n  operationId: createMessageTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{waba-id}/phone_numbers\n  method: get\n  operationId: listWhatsAppPhoneNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/agentic-access/facebook-agentic-access.yml
summary_line: 47 operations · 15 acting
tags:
- Fortune 500
- Advertising
- Content Publishing
- Messaging
- Social Media
- Social Networking
---
