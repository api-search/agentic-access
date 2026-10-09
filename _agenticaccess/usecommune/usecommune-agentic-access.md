---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 44
api_specs:
- filename: usecommune-articles-api-openapi.yml
  format: yaml
  label: Commune Articles API
  slug: usecommune-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-articles-api-openapi.yml
- filename: usecommune-engagement-api-openapi.yml
  format: yaml
  label: Commune Engagement API
  slug: usecommune-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-engagement-api-openapi.yml
- filename: usecommune-event-delivery-api-openapi.yml
  format: yaml
  label: Commune Event delivery API
  slug: usecommune-event-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-event-delivery-api-openapi.yml
- filename: usecommune-highlights-api-openapi.yml
  format: yaml
  label: Commune Highlights API
  slug: usecommune-highlights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-highlights-api-openapi.yml
- filename: usecommune-messages-api-openapi.yml
  format: yaml
  label: Commune Messages API
  slug: usecommune-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-messages-api-openapi.yml
- filename: usecommune-metrics-api-openapi.yml
  format: yaml
  label: Commune Metrics API
  slug: usecommune-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-metrics-api-openapi.yml
- filename: usecommune-newsletters-api-openapi.yml
  format: yaml
  label: Commune Newsletters API
  slug: usecommune-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-newsletters-api-openapi.yml
- filename: usecommune-platform-api-openapi.yml
  format: yaml
  label: Commune Platform API
  slug: usecommune-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-platform-api-openapi.yml
- filename: usecommune-search-api-openapi.yml
  format: yaml
  label: Commune Search API
  slug: usecommune-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-search-api-openapi.yml
- filename: usecommune-senders-api-openapi.yml
  format: yaml
  label: Commune Senders API
  slug: usecommune-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-senders-api-openapi.yml
- filename: usecommune-sends-api-openapi.yml
  format: yaml
  label: Commune Sends API
  slug: usecommune-sends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-sends-api-openapi.yml
- filename: usecommune-subscriber-tags-api-openapi.yml
  format: yaml
  label: Commune Subscriber tags API
  slug: usecommune-subscriber-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-subscriber-tags-api-openapi.yml
- filename: usecommune-subscribers-api-openapi.yml
  format: yaml
  label: Commune Subscribers API
  slug: usecommune-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-subscribers-api-openapi.yml
- filename: usecommune-team-api-openapi.yml
  format: yaml
  label: Commune Team API
  slug: usecommune-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-team-api-openapi.yml
- filename: usecommune-threads-api-openapi.yml
  format: yaml
  label: Commune Threads API
  slug: usecommune-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-threads-api-openapi.yml
- filename: usecommune-users-api-openapi.yml
  format: yaml
  label: Commune Users API
  slug: usecommune-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-users-api-openapi.yml
- filename: usecommune-webhooks-api-openapi.yml
  format: yaml
  label: Commune Webhooks API
  slug: usecommune-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-webhooks-api-openapi.yml
- filename: usecommune-website-domains-api-openapi.yml
  format: yaml
  label: Commune Website domains API
  slug: usecommune-website-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/openapi/usecommune-website-domains-api-openapi.yml
consequence_counts:
  physical: 3
  read: 44
  safety-critical: 1
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Usecommune Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api-keys/{key}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /articles/{article}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /articles/{article}/test-send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /delivery-attempts/{attempt}/replay
operation_count: 63
overview: 'Commune exposes 63 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 44 read, 15 write, 3 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Commune
provider_slug: usecommune
slug: usecommune-agentic-access
source_filename: usecommune-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: generated\nsource: openapi/usecommune-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 63\n  by_action_class:\n    connected: 44\n    acting: 19\n  by_consequence:\n    read: 44\n    write: 15\n    physical: 3\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rate-limit\n  method: get\n  operationId: getRateLimit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters\n\
  \  method: get\n  operationId: listNewsletters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}\n  method: get\n  operationId: getNewsletter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/articles\n  method: get\n  operationId: listNewsletterArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/articles\n  method: post\n  operationId: createArticle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - content:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /articles/{article}\n  method: get\n  operationId: getArticle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article}\n  method: patch\n  operationId: updateArticle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - content:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /articles/{article}/authors\n  method: get\n  operationId: listArticleAuthors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article}/images\n\
  \  method: post\n  operationId: createArticleImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - content:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /articles/{article}/test-send\n  method: post\n  operationId: sendArticleTest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - sending:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /articles/{article}/schedule\n  method: post\n  operationId: scheduleArticle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - sending:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /articles/{article}/unschedule\n  method: post\n  operationId: unscheduleArticle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sending:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /articles/{article}/send\n  method: post\n  operationId: sendArticle\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - sending:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /newsletters/{newsletter}/senders\n  method: get\n  operationId: listNewsletterSenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sending:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /senders/{sender}\n  method: get\n  operationId: getSender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sending:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/domains\n  method: get\n  operationId: listNewsletterDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - settings:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{domain}\n  method: get\n  operationId: getDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - settings:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article}/highlights\n  method: get\n  operationId: listArticleHighlights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /highlights/{highlight}\n  method: get\n  operationId: getHighlight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/tags\n  method: get\n  operationId: listNewsletterTags\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - audience:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/tags\n  method: post\n  operationId: createTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - audience:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/{tag}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - audience:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/{tag}\n  method: patch\n  operationId: updateTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - audience:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/{tag}\n  method: delete\n  operationId: deleteTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - audience:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/{tag}/subscribers\n  method: post\n  operationId: addTagSubscribers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - audience:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /newsletters/{newsletter}/members\n  method: get\n  operationId: listNewsletterMembers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - settings:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/subscribers\n  method: get\n  operationId: listNewsletterSubscribers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - audience:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers/{subscriber}\n  method: get\n  operationId: getSubscriber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - audience:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers/{subscriber}/tags/{tag}\n  method: post\n  operationId: addSubscriberTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - audience:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers/{subscriber}/tags/{tag}\n  method: delete\n  operationId: removeSubscriberTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - audience:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /newsletters/{newsletter}/threads\n  method: get\n  operationId: listNewsletterThreads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/threads\n  method: post\n  operationId: createThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - content:write\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /threads/{thread}\n  method: get\n  operationId: getThread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /threads/{thread}/publish\n  method: post\n  operationId: publishThread\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - content:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /threads/{thread}/messages\n  method: get\n  operationId: listThreadMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /threads/{thread}/messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - content:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/{message}\n  method: get\n  operationId: getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - content:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /memberships\n  method: get\n  operationId: listMemberships\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /saved-articles\n  method: get\n  operationId: listSavedArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /liked-articles\n  method: get\n  operationId: listLikedArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - account:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/insights\n  method: get\n  operationId: listNewsletterInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - insights:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/events\n  method: get\n  operationId: listNewsletterEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - insights:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/stats\n  method: get\n  operationId: getNewsletterStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - insights:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/growth\n  method: get\n  operationId:\
  \ getNewsletterGrowth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - insights:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/timeseries\n  method: get\n  operationId: getNewsletterTimeseries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - insights:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{article}/stats\n  method: get\n  operationId: getArticleStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - insights:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/destinations\n  method: get\n  operationId: listNewsletterDestinations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /newsletters/{newsletter}/delivery-attempts\n  method: get\n  operationId: listNewsletterDeliveryAttempts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sending:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /delivery-attempts/{attempt}\n  method: get\n  operationId: getDeliveryAttempt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sending:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /delivery-attempts/{attempt}/replay\n  method: post\n  operationId: replayDeliveryAttempt\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - sending:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /newsletters/{newsletter}/portal-session\n  method: post\n  operationId: createPortalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /newsletters/{newsletter}/community\n  method: get\n  operationId: listNewsletterCommunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - audience:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/sends\n  method: get\n  operationId: listNewsletterSends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sending:read\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /sends/{send}\n  method: get\n  operationId: getSend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sending:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/entitlements\n  method: get\n  operationId: getNewsletterEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - settings:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /newsletters/{newsletter}/api-keys\n  method: get\n  operationId: listNewsletterApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - settings:write\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys/{key}\n  method: get\n  operationId: getApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - settings:write\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys/{key}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - settings:write\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usecommune/refs/heads/main/agentic-access/usecommune-agentic-access.yml
summary_line: 63 operations · 19 acting · 1 human-in-the-loop
tags:
- Newsletters
- Email
- Community
- Publishing
- Creator Economy
- Subscribers
- Webhooks
- MCP
- Analytics
- Content
---
