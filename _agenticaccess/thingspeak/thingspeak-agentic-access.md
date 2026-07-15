---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 12
api_specs:
- filename: thingspeak-channels-api-openapi.yml
  format: yaml
  label: ThingSpeak Channels API
  slug: thingspeak-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/openapi/thingspeak-channels-api-openapi.yml
- filename: thingspeak-feeds-api-openapi.yml
  format: yaml
  label: ThingSpeak Feeds API
  slug: thingspeak-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/openapi/thingspeak-feeds-api-openapi.yml
- filename: thingspeak-update-api-openapi.yml
  format: yaml
  label: ThingSpeak Update API
  slug: thingspeak-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/openapi/thingspeak-update-api-openapi.yml
- filename: thingspeak-mqtt-asyncapi.yml
  format: yaml
  label: ThingSpeak MQTT API
  slug: thingspeak-mqtt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/asyncapi/thingspeak-mqtt-asyncapi.yml
- filename: thingspeak-talkback-api-openapi.yml
  format: yaml
  label: ThingSpeak TalkBack API
  slug: thingspeak-talkback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/openapi/thingspeak-talkback-api-openapi.yml
consequence_counts:
  read: 12
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Thingspeak Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'ThingSpeak exposes 21 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ThingSpeak
provider_slug: thingspeak
slug: thingspeak-agentic-access
source_filename: thingspeak-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/thingspeak-channels-api-openapi.yml, openapi/thingspeak-feeds-api-openapi.yml,\n  openapi/thingspeak-talkback-api-openapi.yml, openapi/thingspeak-update-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 12\n    acting: 9\n  by_consequence:\n    read: 12\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /channels.json\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels.json\n  method: post\n  operationId: createChannel\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channels/public.json\n  method: get\n  operationId: listPublicChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{channel_id}.json\n  method: get\n  operationId: readChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{channel_id}.json\n  method: put\n  operationId: updateChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /channels/{channel_id}.json\n  method: delete\n  operationId: deleteChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channels/{channel_id}/feeds.json\n  method: delete\n  operationId: clearChannelFeed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channels/{channel_id}/feeds.json\n  method: get\n  operationId: readChannelFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /channels/{channel_id}/fields/{field_id}.json\n  method: get\n  operationId: readFieldFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{channel_id}/feeds/last.json\n  method: get\n  operationId: readLastEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{channel_id}/fields/{field_id}/last.json\n  method: get\n  operationId: readLastFieldEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{channel_id}/status.json\n  method: get\n  operationId: readStatusUpdates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /talkbacks/{talkback_id}/commands.json\n  method: get\n  operationId: listCommands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /talkbacks/{talkback_id}/commands.json\n  method: post\n  operationId: addCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /talkbacks/{talkback_id}/commands/execute.json\n  method: get\n  operationId: executeNextCommand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /talkbacks/{talkback_id}/commands/{command_id}.json\n  method: get\n  operationId: readCommand\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /talkbacks/{talkback_id}/commands/{command_id}.json\n  method: put\n  operationId: updateCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /talkbacks/{talkback_id}/commands/{command_id}.json\n  method: delete\n  operationId: deleteCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update\n  method: get\n  operationId: updateChannelFeedGet\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /update\n  method: post\n  operationId: updateChannelFeedPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /channels/{channel_id}/bulk_update.json\n  method: post\n  operationId: bulkUpdateChannel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/agentic-access/thingspeak-agentic-access.yml
summary_line: 21 operations · 9 acting
tags:
- IoT
- Internet of Things
- Analytics
- Time Series
- MQTT
- MATLAB
- Sensors
- Telemetry
---
