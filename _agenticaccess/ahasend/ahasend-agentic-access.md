---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 19
api_specs:
- filename: ahasend-openapi.yml
  format: yaml
  label: AhaSend
  slug: ahasend
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-openapi.yml
consequence_counts:
  physical: 25
  read: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ahasend Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /email/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/accounts/{account_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/accounts/{account_id}/api-keys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/accounts/{account_id}/api-keys/{key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/accounts/{account_id}/api-keys/{key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/accounts/{account_id}/domains
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/accounts/{account_id}/domains/{domain}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/accounts/{account_id}/domains/{domain}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/accounts/{account_id}/domains/{domain}/check-dns
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/accounts/{account_id}/members
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/accounts/{account_id}/members/{user_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/accounts/{account_id}/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/accounts/{account_id}/messages/conversation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/accounts/{account_id}/messages/{message_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/accounts/{account_id}/routes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/accounts/{account_id}/routes/{route_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/accounts/{account_id}/routes/{route_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/accounts/{account_id}/smtp-credentials
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/accounts/{account_id}/smtp-credentials/{smtp_credential_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/accounts/{account_id}/suppressions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/accounts/{account_id}/suppressions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/accounts/{account_id}/suppressions/all
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/accounts/{account_id}/webhooks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/accounts/{account_id}/webhooks/{webhook_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/accounts/{account_id}/webhooks/{webhook_id}
operation_count: 44
overview: 'AhaSend exposes 44 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 25 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AhaSend
provider_slug: ahasend
slug: ahasend-agentic-access
source_filename: ahasend-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ahasend-openapi-v2.yaml, openapi/ahasend-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 19\n    acting: 25\n  by_consequence:\n    read: 19\n    physical: 25\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/api-keys\n  method: get\n  operationId: getAPIKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api-keys:read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v2/accounts/{account_id}/api-keys\n  method: post\n  operationId: createAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - api-keys:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/api-keys/{key_id}\n  method: get\n  operationId: getAPIKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api-keys:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/api-keys/{key_id}\n  method: put\n  operationId: updateAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - api-keys:write\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/api-keys/{key_id}\n  method: delete\n  operationId: deleteAPIKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - api-keys:delete\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/domains\n  method: get\n  operationId: getDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - domains:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/domains\n  method: post\n\
  \  operationId: createDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - domains:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/domains/{domain}\n  method: get\n  operationId: getDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - domains:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/domains/{domain}\n  method: put\n  operationId: updateDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - domains:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/domains/{domain}\n  method: delete\n  operationId: deleteDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - domains:delete:all\n    - domains:delete:{domain}\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/domains/{domain}/check-dns\n  method: post\n  operationId: checkDomainDNS\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - domains:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/messages\n  method: get\n  operationId: getMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - messages:read:all\n    - messages:read:{domain}\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/messages\n  method: post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - messages:send:all\n    - messages:send:{domain}\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/messages/conversation\n  method: post\n  operationId: createConversationMessage\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - messages:send:all\n    - messages:send:{domain}\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/messages/{message_id}\n  method: get\n  operationId: getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - messages:read:all\n    - messages:read:{domain}\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/messages/{message_id}/cancel\n  method: delete\n  operationId: cancelMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - messages:cancel:all\n    - messages:cancel:{domain}\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}\n  method: put\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/members\n  method: get\n  operationId: getAccountMembers\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:members:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/members\n  method: post\n  operationId: addAccountMember\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounts:members:add\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/members/{user_id}\n  method: delete\n  operationId: removeAccountMember\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounts:members:remove\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/suppressions\n  method: get\n  operationId: getSuppressions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - suppressions:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/suppressions\n  method: post\n  operationId: createSuppression\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - suppressions:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/suppressions\n  method: delete\n  operationId: deleteSuppression\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - suppressions:delete\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/suppressions/all\n  method: delete\n  operationId: deleteAllSuppressions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - suppressions:wipe\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/routes\n  method: get\n  operationId: getRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - routes:read:all\n    - routes:read:{domain}\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/routes\n  method: post\n  operationId: createRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - routes:write:all\n    - routes:write:{domain}\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/routes/{route_id}\n  method: get\n  operationId: getRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - routes:read:all\n    - routes:read:{domain}\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/routes/{route_id}\n  method: put\n  operationId: updateRoute\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - routes:write:all\n    - routes:write:{domain}\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/routes/{route_id}\n  method: delete\n  operationId: deleteRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - routes:delete:all\n    - routes:delete:{domain}\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/webhooks\n  method: get\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:read:all\n    - webhooks:read:{domain}\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - webhooks:write:all\n    - webhooks:write:{domain}\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/webhooks/{webhook_id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:read:all\n    - webhooks:read:{domain}\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/webhooks/{webhook_id}\n\
  \  method: put\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - webhooks:write:all\n    - webhooks:write:{domain}\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - webhooks:delete:all\n    - webhooks:delete:{domain}\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/smtp-credentials\n\
  \  method: get\n  operationId: getSMTPCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - smtp-credentials:read:all\n    - smtp-credentials:read:{domain}\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/smtp-credentials\n  method: post\n  operationId: createSMTPCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - smtp-credentials:write:all\n    - smtp-credentials:write:{domain}\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/smtp-credentials/{smtp_credential_id}\n  method: get\n  operationId: getSMTPCredential\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    scope:\n    - smtp-credentials:read:all\n    - smtp-credentials:read:{domain}\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/smtp-credentials/{smtp_credential_id}\n  method: delete\n  operationId: deleteSMTPCredential\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - smtp-credentials:delete:all\n    - smtp-credentials:delete:{domain}\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{account_id}/statistics/transactional/deliverability\n  method: get\n  operationId: getDeliverabilityStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - statistics-transactional:read:all\n    - statistics-transactional:read:{domain}\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/statistics/transactional/bounce\n  method: get\n  operationId: getBounceStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - statistics-transactional:read:all\n    - statistics-transactional:read:{domain}\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{account_id}/statistics/transactional/delivery-time\n  method: get\n  operationId: getDeliveryTimeStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - statistics-transactional:read:all\n    - statistics-transactional:read:{domain}\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/send\n  method: post\n  operationId: sendEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - read:email\n    - write:email\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/agentic-access/ahasend-agentic-access.yml
summary_line: 44 operations · 25 acting
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
---
