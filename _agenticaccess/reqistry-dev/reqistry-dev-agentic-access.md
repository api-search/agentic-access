---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 35
api_specs:
- filename: reqistry-dev-agentkeys-api-openapi.yml
  format: yaml
  label: reqistry-dev Agent Keys API
  slug: reqistry-dev-agentkeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-agentkeys-api-openapi.yml
- filename: reqistry-dev-api-detail-api-openapi.yml
  format: yaml
  label: reqistry-dev API Detail API
  slug: reqistry-dev-api-detail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-api-detail-api-openapi.yml
- filename: reqistry-dev-auth-api-openapi.yml
  format: yaml
  label: reqistry-dev Auth API
  slug: reqistry-dev-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-auth-api-openapi.yml
- filename: reqistry-dev-bookmarks-api-openapi.yml
  format: yaml
  label: reqistry-dev Bookmarks API
  slug: reqistry-dev-bookmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-bookmarks-api-openapi.yml
- filename: reqistry-dev-categories-api-openapi.yml
  format: yaml
  label: reqistry-dev Categories API
  slug: reqistry-dev-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-categories-api-openapi.yml
- filename: reqistry-dev-contact-api-openapi.yml
  format: yaml
  label: reqistry-dev Contact API
  slug: reqistry-dev-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-contact-api-openapi.yml
- filename: reqistry-dev-discover-api-openapi.yml
  format: yaml
  label: reqistry-dev Discover API
  slug: reqistry-dev-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-discover-api-openapi.yml
- filename: reqistry-dev-folders-api-openapi.yml
  format: yaml
  label: reqistry-dev Folders API
  slug: reqistry-dev-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-folders-api-openapi.yml
- filename: reqistry-dev-growth-api-openapi.yml
  format: yaml
  label: reqistry-dev Growth API
  slug: reqistry-dev-growth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-growth-api-openapi.yml
- filename: reqistry-dev-health-api-openapi.yml
  format: yaml
  label: reqistry-dev Health API
  slug: reqistry-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-health-api-openapi.yml
- filename: reqistry-dev-metadata-api-openapi.yml
  format: yaml
  label: reqistry-dev Metadata API
  slug: reqistry-dev-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-metadata-api-openapi.yml
- filename: reqistry-dev-notifications-api-openapi.yml
  format: yaml
  label: reqistry-dev Notifications API
  slug: reqistry-dev-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-notifications-api-openapi.yml
- filename: reqistry-dev-projects-api-openapi.yml
  format: yaml
  label: reqistry-dev Projects API
  slug: reqistry-dev-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-projects-api-openapi.yml
- filename: reqistry-dev-public-apis-mobile-client-api-api-openapi.yml
  format: yaml
  label: reqistry-dev Public APIs — Mobile Client API
  slug: reqistry-dev-public-apis-mobile-client-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-public-apis-mobile-client-api-api-openapi.yml
- filename: reqistry-dev-push-notifications-api-openapi.yml
  format: yaml
  label: reqistry-dev Push Notifications API
  slug: reqistry-dev-push-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-push-notifications-api-openapi.yml
- filename: reqistry-dev-reports-api-openapi.yml
  format: yaml
  label: reqistry-dev Reports API
  slug: reqistry-dev-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-reports-api-openapi.yml
- filename: reqistry-dev-search-api-openapi.yml
  format: yaml
  label: reqistry-dev Search API
  slug: reqistry-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-search-api-openapi.yml
- filename: reqistry-dev-submit-api-openapi.yml
  format: yaml
  label: reqistry-dev Submit API
  slug: reqistry-dev-submit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-submit-api-openapi.yml
- filename: reqistry-dev-tracking-api-openapi.yml
  format: yaml
  label: reqistry-dev Tracking API
  slug: reqistry-dev-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-tracking-api-openapi.yml
- filename: reqistry-dev-watchlists-api-openapi.yml
  format: yaml
  label: reqistry-dev Watchlists API
  slug: reqistry-dev-watchlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reqistry-dev/openapi/reqistry-dev-watchlists-api-openapi.yml
consequence_counts:
  physical: 2
  read: 35
  safety-critical: 3
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Reqistry Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/agent-keys/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/fcm-tokens
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/v1/contact-messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/ship-check
operation_count: 66
overview: 'reqistry-dev exposes 66 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read, 26 write, 2 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: reqistry-dev
provider_slug: reqistry-dev
slug: reqistry-dev-agentic-access
source_filename: reqistry-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/reqistry-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 66\n  by_action_class:\n    connected: 35\n    acting: 31\n  by_consequence:\n    read: 35\n    write: 26\n    safety-critical: 3\n    physical: 2\n  human_in_the_loop_required: 3\noperations:\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: root\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method:\
  \ get\n  operationId: searchApis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: get\n  operationId: getCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{id}\n  method: get\n  operationId: getCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{id}/image\n  method: get\n  operationId: getCategoryImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories/{id}/apis\n  method: get\n  operationId: getCategoryApis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /trendy-categories\n  method: get\n  operationId: getTrendyCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submit\n  method: post\n  operationId: submitApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apis\n  method: post\n  operationId: submitAttributedApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/anonymous\n  method: post\n\
  \  operationId: anonymousAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/refresh\n  method: post\n  operationId: refreshToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/revoke\n  method: post\n  operationId: revokeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /v1/auth/link-email\n  method: post\n  operationId: linkEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/login-email\n  method: post\n  operationId: loginEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/me\n  method: put\n  operationId: updateMe\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/me\n  method: delete\n  operationId: deleteMe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recently-added\n  method: get\n  operationId: getRecentlyAdded\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recommend\n  method: get\n  operationId: getPersonalizedRecommend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/apis/{slug}\n  method: get\n  operationId: getApiDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apis/{id}/alternatives\n  method: get\n  operationId: getApiAlternatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apis/{id}/health-check\n  method: post\n  operationId: refreshApiHealth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/apis/{id}/health-checks/{checkId}\n  method: get\n  operationId: pollApiHealth\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apis/{id}/reports\n  method: post\n  operationId: reportApiInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/apis\n  method: post\n  operationId: addApiToProjectById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/projects/{projectId}/apis/{apiId}\n  method: delete\n  operationId: removeApiFromProjectById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookmarks\n  method: get\n  operationId: listBookmarks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/bookmarks\n  method: post\n  operationId: addBookmark\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/bookmarks/{id}\n  method: delete\n  operationId: removeBookmark\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/folders\n  method: get\n  operationId: listFolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/folders\n  method: post\n  operationId: createFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/folders/{id}\n  method: get\n  operationId: getFolder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/folders/{id}\n  method: put\n  operationId: updateFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/folders/{id}\n  method: delete\n  operationId: deleteFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/folders/{id}/api-links\n  method: post\n  operationId: addApiToFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/folders/{id}/api-links/{link}\n  method: delete\n  operationId: removeApiFromFolder\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/folders/{id}/metadata\n  method: get\n  operationId: getFolderMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fcm-tokens\n  method: get\n  operationId: listFcmTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fcm-tokens\n  method: post\n  operationId: registerFcmToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fcm-tokens\n  method: delete\n  operationId: revokeFcmToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /track\n  method: post\n  operationId: trackEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /metadata\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/trust-scores/{id}\n  method: get\n  operationId: getTrustScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/apis/compare\n  method: get\n  operationId: compareApis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/change-feed\n  method: get\n  operationId: getChangeFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/use-case-collections\n  method: get\n  operationId: getUseCaseCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/stack\n  method: get\n  operationId: getStack\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notifications/preferences\n  method: get\n  operationId: getNotificationPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notifications/preferences\n  method: patch\n  operationId: updateNotificationPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications/events\n  method: post\n  operationId: trackNotificationEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/categories\n  method: get\n  operationId: getV1Categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/categories/{id}\n  method: get\n  operationId: getV1Category\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/categories/{id}/apis\n  method: get\n  operationId: getV1CategoryApis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/categories/{id}/image\n  method: get\n  operationId: getV1CategoryImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/submissions/mine\n\
  \  method: get\n  operationId: listMySubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/v1/contact-messages\n  method: post\n  operationId: sendContactMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ship-check\n  method: post\n  operationId: shipCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/watchlists\n  method: get\n  operationId: listWatchlists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/watchlists\n  method: post\n  operationId: addWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/watchlists/{id}\n  method: delete\n  operationId: removeWatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent-keys/config\n  method: get\n  operationId: getAgentClientConfig\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent-keys\n  method: get\n  operationId: listAgentKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent-keys\n  method: post\n  operationId: createAgentKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent-keys/{id}\n  method: delete\n  operationId: revokeAgentKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n   \
  \   proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/stack/history\n  method: get\n  operationId: getStackHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/reqistry-dev/agentic-access/reqistry-dev-agentic-access.yml
summary_line: 66 operations · 31 acting · 3 human-in-the-loop
tags:
- Company
- Catalog
- Intelligence
- Builder
- Agents
---
