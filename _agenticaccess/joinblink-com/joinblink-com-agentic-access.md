---
acting_count: 30
action_class_counts:
  acting: 30
  connected: 21
api_specs:
- filename: joinblink-com-access-api-openapi.yml
  format: yaml
  label: Blink Access API
  slug: joinblink-com-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-access-api-openapi.yml
- filename: joinblink-com-chats-api-openapi.yml
  format: yaml
  label: Blink Chats API
  slug: joinblink-com-chats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-chats-api-openapi.yml
- filename: joinblink-com-feed-api-openapi.yml
  format: yaml
  label: Blink Feed API
  slug: joinblink-com-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-feed-api-openapi.yml
- filename: joinblink-com-forms-api-openapi.yml
  format: yaml
  label: Blink Forms API
  slug: joinblink-com-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-forms-api-openapi.yml
- filename: joinblink-com-group-api-openapi.yml
  format: yaml
  label: Blink Group API
  slug: joinblink-com-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-group-api-openapi.yml
- filename: joinblink-com-linked-account-api-openapi.yml
  format: yaml
  label: Blink Linked Account API
  slug: joinblink-com-linked-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-linked-account-api-openapi.yml
- filename: joinblink-com-linked-accounts-api-openapi.yml
  format: yaml
  label: Blink Linked Accounts API
  slug: joinblink-com-linked-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-linked-accounts-api-openapi.yml
- filename: joinblink-com-members-api-openapi.yml
  format: yaml
  label: Blink Members API
  slug: joinblink-com-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-members-api-openapi.yml
- filename: joinblink-com-messages-api-openapi.yml
  format: yaml
  label: Blink Messages API
  slug: joinblink-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-messages-api-openapi.yml
- filename: joinblink-com-user-api-openapi.yml
  format: yaml
  label: Blink User API
  slug: joinblink-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-user-api-openapi.yml
- filename: joinblink-com-service-provider-config-api-openapi.yml
  format: yaml
  label: Blink Service Provider Config API
  slug: joinblink-com-service-provider-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinblink-com/openapi/joinblink-com-service-provider-config-api-openapi.yml
consequence_counts:
  physical: 2
  read: 21
  safety-critical: 4
  write: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Joinblink Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /Groups/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /Users/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /chats/{chatId}/grants/apps/{appIdentityId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /chats/{chatId}/grants/users/{userId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chats/{chatId}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /feed/events
operation_count: 51
overview: 'Blink exposes 51 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 24 write, 2 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Blink
provider_slug: joinblink-com
slug: joinblink-com-agentic-access
source_filename: joinblink-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: generated\nsource: openapi/joinblink-com-blink-api-v2-api-openapi.yml, openapi/joinblink-com-blink-chat-api-openapi.yml,\n  openapi/joinblink-com-scim-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 51\n  by_action_class:\n    connected: 21\n    acting: 30\n  by_consequence:\n    read: 21\n    physical: 2\n    write: 24\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /feed/categories\n  method: get\n  operationId: get-feed-event-categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feed/event-by-external-id\n  method: get\n  operationId: get-feed-event-id-by-external-id\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feed/events\n  method: post\n  operationId: send-feed-event\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feed/events/{event_id}\n  method: put\n  operationId: update-feed-event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feed/events/{event_id}/archive\n  method: post\n  operationId: archive-feed-event\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feed/events/{event_id}/user/{user_id}/archive\n  method: post\n  operationId: archive-feed-event-for-user\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /forms\n  method: get\n  operationId: get-forms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forms/{id}/submissions\n  method: get\n  operationId: form-submissions\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linked-account/{linked_account_id}\n  method: get\n  operationId: get-linked-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /linked-accounts\n  method: get\n  operationId: get-linked-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user\n  method: get\n  operationId: get-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{user_id}/linked-account/{linked_account_id}\n  method: delete\n  operationId: delete-user-linked-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{user_id}/linked-accounts\n  method: post\n  operationId: add-user-linked-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{user_id}/linked-accounts\n  method: get\n  operationId: get-user-linked-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{user_id}/linked-accounts/{linked_account_id}\n  method: put\n  operationId: update-user-linked-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chats\n  method: post\n  operationId: createChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chats/inbox\n  method: get\n  operationId: listChatInbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chats/{chatId}\n  method: get\n  operationId: getChat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chats/{chatId}\n  method: patch\n  operationId: updateChat\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chats/{chatId}\n  method: delete\n  operationId: deleteChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chats/{chatId}/grants\n  method: get\n  operationId: listGrants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chats/{chatId}/grants\n  method: post\n  operationId: grantAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chats/{chatId}/grants/apps/{appIdentityId}\n  method: delete\n  operationId: revokeAppAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /chats/{chatId}/grants/users/{userId}\n  method: delete\n  operationId: revokeUserAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /chats/{chatId}/members\n  method: get\n  operationId: listMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chats/{chatId}/members/apps/{appIdentityId}\n  method: patch\n  operationId: updateAppMemberRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chats/{chatId}/members/apps/{appIdentityId}\n  method: delete\n  operationId: removeAppMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /chats/{chatId}/members/me\n  method: get\n  operationId: getMyMembership\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chats/{chatId}/members/users/{userId}\n  method: patch\n  operationId: updateUserMemberRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chats/{chatId}/members/users/{userId}\n  method: delete\n  operationId: removeUserMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chats/{chatId}/messages\n\
  \  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chats/{chatId}/messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chats/{chatId}/messages/{messageId}\n  method: get\n  operationId: getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chats/{chatId}/messages/{messageId}\n  method: patch\n  operationId: updateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chats/{chatId}/messages/{messageId}\n  method: delete\n  operationId: deleteMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chats/{chatId}/messages/{messageId}/permalink\n  method: get\n  operationId: getMessagePermalink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chats/{chatId}:join\n  method: post\n  operationId: joinChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chats/{chatId}:leave\n  method: post\n  operationId: leaveChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Groups\n  method: get\n  operationId: searchGroupViaGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Groups\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Groups/{id}\n  method: get\n  operationId: getGroupById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Groups/{id}\n  method: put\n  operationId: replaceGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Groups/{id}\n  method: patch\n  operationId: groupUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Groups/{id}\n  method:\
  \ delete\n  operationId: deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /ServiceProviderConfig\n  method: get\n  operationId: getServiceProviderConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Users\n  method: get\n  operationId: searchViaGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Users/{id}\n  method: get\n  operationId: getUserById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Users/{id}\n  method: put\n  operationId: replaceUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Users/{id}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /Users/{id}\n  method: patch\n  operationId: patchUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/joinblink-com/agentic-access/joinblink-com-agentic-access.yml
summary_line: 51 operations · 30 acting · 4 human-in-the-loop
tags:
- Company
- Employee Experience
- MobileFirst
- Frontline Workers
- Communications
---
