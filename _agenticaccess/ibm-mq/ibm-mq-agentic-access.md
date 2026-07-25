---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 12
api_specs:
- filename: ibm-mq-messaging-asyncapi.yml
  format: yaml
  label: IBM MQ JMS API
  slug: ibm-mq-jms-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/asyncapi/ibm-mq-messaging-asyncapi.yml
- filename: ibm-mq-channels-api-openapi.yml
  format: yaml
  label: IBM MQ Channels API
  slug: ibm-mq-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-channels-api-openapi.yml
- filename: ibm-mq-installations-api-openapi.yml
  format: yaml
  label: IBM MQ Installations API
  slug: ibm-mq-installations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-installations-api-openapi.yml
- filename: ibm-mq-login-api-openapi.yml
  format: yaml
  label: IBM MQ Login API
  slug: ibm-mq-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-login-api-openapi.yml
- filename: ibm-mq-queue-managers-api-openapi.yml
  format: yaml
  label: IBM MQ Queue Managers API
  slug: ibm-mq-queue-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-queue-managers-api-openapi.yml
- filename: ibm-mq-queue-messaging-api-openapi.yml
  format: yaml
  label: IBM MQ Queue Messaging API
  slug: ibm-mq-queue-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-queue-messaging-api-openapi.yml
- filename: ibm-mq-queues-api-openapi.yml
  format: yaml
  label: IBM MQ Queues API
  slug: ibm-mq-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-queues-api-openapi.yml
- filename: ibm-mq-subscriptions-api-openapi.yml
  format: yaml
  label: IBM MQ Subscriptions API
  slug: ibm-mq-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-subscriptions-api-openapi.yml
- filename: ibm-mq-topic-messaging-api-openapi.yml
  format: yaml
  label: IBM MQ Topic Messaging API
  slug: ibm-mq-topic-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-topic-messaging-api-openapi.yml
- filename: ibm-mq-topics-api-openapi.yml
  format: yaml
  label: IBM MQ Topics API
  slug: ibm-mq-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/openapi/ibm-mq-topics-api-openapi.yml
consequence_counts:
  physical: 1
  read: 12
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ibm Mq Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messaging/qmgr/{qmgrName}/queue/{queueName}/message
operation_count: 28
overview: 'IBM MQ exposes 28 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 15 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IBM MQ
provider_slug: ibm-mq
slug: ibm-mq-agentic-access
source_filename: ibm-mq-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ibm-mq-admin-rest-openapi.yml, openapi/ibm-mq-messaging-rest-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 12\n    acting: 16\n  by_consequence:\n    read: 12\n    write: 15\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /admin/qmgr\n  method: get\n  operationId: listQueueManagers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/qmgr/{qmgrName}\n  method: get\n  operationId: getQueueManager\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /admin/qmgr/{qmgrName}/queue\n  method: get\n  operationId: listQueues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/qmgr/{qmgrName}/queue\n  method: post\n  operationId: createQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/qmgr/{qmgrName}/queue/{queueName}\n  method: get\n  operationId: getQueue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/qmgr/{qmgrName}/queue/{queueName}\n  method: patch\n  operationId: updateQueue\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/qmgr/{qmgrName}/queue/{queueName}\n  method: delete\n  operationId: deleteQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/qmgr/{qmgrName}/topic\n  method: get\n  operationId: listTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/qmgr/{qmgrName}/topic\n  method: post\n  operationId: createTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/qmgr/{qmgrName}/topic/{topicName}\n  method: get\n  operationId: getTopic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/qmgr/{qmgrName}/topic/{topicName}\n  method: patch\n  operationId: updateTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/qmgr/{qmgrName}/topic/{topicName}\n  method: delete\n  operationId: deleteTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/qmgr/{qmgrName}/subscription\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/qmgr/{qmgrName}/subscription\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/qmgr/{qmgrName}/subscription/{subscriptionId}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /admin/qmgr/{qmgrName}/subscription/{subscriptionId}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/qmgr/{qmgrName}/channel\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/qmgr/{qmgrName}/channel\n  method: post\n  operationId: createChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /admin/qmgr/{qmgrName}/channel/{channelName}\n  method: get\n  operationId: getChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/qmgr/{qmgrName}/channel/{channelName}\n  method: patch\n  operationId: updateChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/qmgr/{qmgrName}/channel/{channelName}\n  method: delete\n  operationId: deleteChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /admin/installation\n  method: get\n  operationId: listInstallations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/qmgr/{qmgrName}/queue/{queueName}/message\n  method: post\n  operationId: sendMessageToQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/qmgr/{qmgrName}/queue/{queueName}/message\n  method: get\n  operationId: receiveMessageFromQueue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/qmgr/{qmgrName}/queue/{queueName}/message\n\
  \  method: delete\n  operationId: browseMessageFromQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/qmgr/{qmgrName}/topic/{topicString}/message\n  method: post\n  operationId: publishMessageToTopic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /login\n  method: delete\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibm-mq/refs/heads/main/agentic-access/ibm-mq-agentic-access.yml
summary_line: 28 operations · 16 acting
tags:
- Async
- Enterprise
- Integration
- Messaging
- Middleware
- Queue
---
