---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 2
api_specs:
- filename: amazon-kinesis-firehose-openapi.yml
  format: yaml
  label: Amazon Kinesis Data Firehose API
  slug: amazon-kinesis-data-firehose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis-firehose/refs/heads/main/openapi/amazon-kinesis-firehose-openapi.yml
consequence_counts:
  read: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Kinesis Firehose Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Amazon Kinesis Data Firehose exposes 7 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Kinesis Data Firehose
provider_slug: amazon-kinesis-firehose
slug: amazon-kinesis-firehose-agentic-access
source_filename: amazon-kinesis-firehose-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-kinesis-firehose-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 5\n    connected: 2\n  by_consequence:\n    write: 5\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /delivery-streams\n  method: post\n  operationId: CreateDeliveryStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery-streams\n  method: get\n  operationId: ListDeliveryStreams\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /delivery-streams/{DeliveryStreamName}\n  method: get\n  operationId: DescribeDeliveryStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /delivery-streams/{DeliveryStreamName}\n  method: delete\n  operationId: DeleteDeliveryStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery-streams/{DeliveryStreamName}/destination\n  method: put\n  operationId: UpdateDestination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery-streams/{DeliveryStreamName}/records\n  method: post\n  operationId: PutRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery-streams/{DeliveryStreamName}/records/batch\n  method: post\n  operationId: PutRecordBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis-firehose/refs/heads/main/agentic-access/amazon-kinesis-firehose-agentic-access.yml
summary_line: 7 operations · 5 acting
tags:
- Analytics
- Data Delivery
- Streaming
---
