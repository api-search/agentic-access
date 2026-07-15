---
acting_count: 32
action_class_counts:
  acting: 32
  connected: 17
api_specs:
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Events API
  slug: novu-co-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Subscribers API
  slug: novu-co-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Topics API
  slug: novu-co-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Inbox API
  slug: novu-co-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Messages API
  slug: novu-co-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Notifications API
  slug: novu-co-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Workflows API
  slug: novu-co-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Integrations API
  slug: novu-co-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Layouts API
  slug: novu-co-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Subscriber Preferences API
  slug: novu-co-subscriber-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Environments API
  slug: novu-co-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Translations API
  slug: novu-co-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-asyncapi.yml
  format: yaml
  label: Novu Inbox Realtime API
  slug: novu-co-inbox-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/asyncapi/novu-co-asyncapi.yml
consequence_counts:
  read: 17
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Novu Co Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 49
overview: 'Novu exposes 49 API operations that an AI agent could call, of which 32 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 32 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Novu
provider_slug: novu-co
slug: novu-co-agentic-access
source_filename: novu-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/novu-co-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    acting: 32\n    connected: 17\n  by_consequence:\n    write: 32\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /events/trigger\n  method: post\n  operationId: triggerEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/trigger/bulk\n  method: post\n  operationId: bulkTriggerEvents\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/broadcast\n  method: post\n  operationId: broadcastEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/trigger/{transactionId}\n  method: delete\n  operationId: cancelTriggeredEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers\n  method: post\n  operationId:\
  \ createSubscriber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers/bulk\n  method: post\n  operationId: bulkCreateSubscribers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers/{subscriberId}\n  method: get\n  operationId: getSubscriber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers/{subscriberId}\n  method: put\n  operationId: updateSubscriber\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers/{subscriberId}\n  method: delete\n  operationId: deleteSubscriber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers/{subscriberId}/credentials/{providerId}\n  method: put\n  operationId: updateSubscriberCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /subscribers/{subscriberId}/preferences\n  method: get\n  operationId: getSubscriberPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers/{subscriberId}/preferences\n  method: patch\n  operationId: updateSubscriberPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscribers/{subscriberId}/notifications/feed\n  method: get\n  operationId: getInAppNotificationFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers/{subscriberId}/notifications/unseen\n  method: get\n  operationId: getUnseenCount\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscribers/{subscriberId}/messages/markAs\n  method: post\n  operationId: markMessagesAs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /topics\n  method: post\n  operationId: createTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /topics\n  method: get\n  operationId: listTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topics/{topicKey}\n  method: get\n  operationId: getTopic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topics/{topicKey}\n  method: delete\n  operationId: deleteTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /topics/{topicKey}/subscribers\n  method: post\n  operationId: addSubscribersToTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /topics/{topicKey}/subscribers\n  method: delete\n  operationId: removeSubscribersFromTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/{messageId}\n  method: delete\n  operationId: deleteMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications\n  method: get\n  operationId: listNotifications\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/{notificationId}\n  method: get\n  operationId: getNotification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflows\n  method: post\n  operationId: createWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workflows\n  method: get\n  operationId: listWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflows/{workflowId}\n  method: get\n  operationId: getWorkflow\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workflows/{workflowId}\n  method: put\n  operationId: updateWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workflows/{workflowId}\n  method: patch\n  operationId: patchWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workflows/{workflowId}\n  method: delete\n  operationId: deleteWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workflows/{workflowId}/sync\n  method: post\n  operationId: syncWorkflow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations\n  method: post\n  operationId: createIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations\n  method: get\n  operationId: listIntegrations\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/active\n  method: get\n  operationId: listActiveIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/{integrationId}\n  method: put\n  operationId: updateIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/{integrationId}\n  method: delete\n  operationId: deleteIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/{integrationId}/set-primary\n  method: post\n  operationId: setIntegrationPrimary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /layouts\n  method: post\n  operationId: createLayout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /layouts\n  method: get\n  operationId: listLayouts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /layouts/{layoutId}\n  method: get\n  operationId: getLayout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /layouts/{layoutId}\n  method: put\n  operationId: updateLayout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /layouts/{layoutId}\n  method: delete\n  operationId: deleteLayout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments\n  method: post\n  operationId: createEnvironment\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments\n  method: get\n  operationId: listEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/publish\n  method: post\n  operationId: publishEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /translations\n  method: post\n  operationId: createTranslation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /translations/{resourceType}/{resourceId}/{locale}\n  method: get\n  operationId: getTranslation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /translations/{resourceType}/{resourceId}/{locale}\n  method: delete\n  operationId: deleteTranslation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/agentic-access/novu-co-agentic-access.yml
summary_line: 49 operations · 32 acting
tags:
- Notifications
- Multi-Channel
- Email
- SMS
- Push
- Chat
- In-App Inbox
- Open Source
- WebSocket
---
