---
acting_count: 36
action_class_counts:
  acting: 36
  connected: 3
api_specs:
- filename: amazon-kinesis-account-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Account API
  slug: amazon-kinesis-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-account-api-openapi.yml
- filename: amazon-kinesis-consumers-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Consumers API
  slug: amazon-kinesis-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-consumers-api-openapi.yml
- filename: amazon-kinesis-encryption-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Encryption API
  slug: amazon-kinesis-encryption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-encryption-api-openapi.yml
- filename: amazon-kinesis-monitoring-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Monitoring API
  slug: amazon-kinesis-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-monitoring-api-openapi.yml
- filename: amazon-kinesis-policies-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Policies API
  slug: amazon-kinesis-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-policies-api-openapi.yml
- filename: amazon-kinesis-records-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Records API
  slug: amazon-kinesis-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-records-api-openapi.yml
- filename: amazon-kinesis-shards-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Shards API
  slug: amazon-kinesis-shards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-shards-api-openapi.yml
- filename: amazon-kinesis-streams-api-openapi.yml
  format: yaml
  label: Amazon Kinesis Streams API
  slug: amazon-kinesis-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-streams-api-openapi.yml
- filename: amazon-kinesis-x-amz-target-kinesis-20131202-addtagstostream-api-openapi.yml
  format: yaml
  label: 'Amazon Kinesis #X Amz Target=Kinesis 20131202.AddTagsToStream API'
  slug: amazon-kinesis-x-amz-target-kinesis-20131202-addtagstostream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-x-amz-target-kinesis-20131202-addtagstostream-api-openapi.yml
- filename: amazon-kinesis-x-amz-target-kinesis-20131202-listtagsforstream-api-openapi.yml
  format: yaml
  label: 'Amazon Kinesis #X Amz Target=Kinesis 20131202.ListTagsForStream API'
  slug: amazon-kinesis-x-amz-target-kinesis-20131202-listtagsforstream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-x-amz-target-kinesis-20131202-listtagsforstream-api-openapi.yml
- filename: amazon-kinesis-x-amz-target-kinesis-20131202-removetagsfromstream-api-openapi.yml
  format: yaml
  label: 'Amazon Kinesis #X Amz Target=Kinesis 20131202.RemoveTagsFromStream API'
  slug: amazon-kinesis-x-amz-target-kinesis-20131202-removetagsfromstream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/openapi/amazon-kinesis-x-amz-target-kinesis-20131202-removetagsfromstream-api-openapi.yml
consequence_counts:
  read: 3
  safety-critical: 2
  write: 34
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Kinesis Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=Kinesis_20131202.DisableEnhancedMonitoring
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#X-Amz-Target=Kinesis_20131202.StopStreamEncryption
operation_count: 39
overview: 'Amazon Kinesis exposes 39 API operations that an AI agent could call, of which 36 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 34 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Kinesis
provider_slug: amazon-kinesis
slug: amazon-kinesis-agentic-access
source_filename: amazon-kinesis-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-kinesis-data-streams-openapi.yml, openapi/amazon-kinesis-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    acting: 36\n    connected: 3\n  by_consequence:\n    write: 34\n    safety-critical: 2\n    read: 3\n  human_in_the_loop_required: 2\noperations:\n- path: /#X-Amz-Target=Kinesis_20131202.CreateStream\n  method: post\n  operationId: CreateStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.DeleteStream\n\
  \  method: post\n  operationId: DeleteStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.DescribeStream\n  method: post\n  operationId: DescribeStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.DescribeStreamSummary\n  method: post\n  operationId: DescribeStreamSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.ListStreams\n  method: post\n  operationId: ListStreams\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.UpdateStreamMode\n  method: post\n  operationId: UpdateStreamMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.ListShards\n  method: post\n  operationId: ListShards\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.SplitShard\n  method: post\n  operationId: SplitShard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.MergeShards\n  method: post\n  operationId: MergeShards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.UpdateShardCount\n\
  \  method: post\n  operationId: UpdateShardCount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.PutRecord\n  method: post\n  operationId: PutRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.PutRecords\n  method: post\n  operationId: PutRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.GetShardIterator\n  method: post\n  operationId: GetShardIterator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.GetRecords\n  method: post\n  operationId: GetRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.RegisterStreamConsumer\n  method: post\n  operationId: RegisterStreamConsumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.DeregisterStreamConsumer\n  method: post\n  operationId: DeregisterStreamConsumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.DescribeStreamConsumer\n  method: post\n  operationId: DescribeStreamConsumer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /#X-Amz-Target=Kinesis_20131202.ListStreamConsumers\n  method: post\n  operationId: ListStreamConsumers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.SubscribeToShard\n  method: post\n  operationId: SubscribeToShard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.EnableEnhancedMonitoring\n  method: post\n  operationId: EnableEnhancedMonitoring\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.DisableEnhancedMonitoring\n  method: post\n  operationId: DisableEnhancedMonitoring\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.StartStreamEncryption\n  method: post\n  operationId: StartStreamEncryption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /#X-Amz-Target=Kinesis_20131202.StopStreamEncryption\n  method: post\n  operationId: StopStreamEncryption\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.IncreaseStreamRetentionPeriod\n  method: post\n  operationId: IncreaseStreamRetentionPeriod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.DecreaseStreamRetentionPeriod\n  method: post\n  operationId: DecreaseStreamRetentionPeriod\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.AddTagsToStream\n  method: post\n  operationId: AddTagsToStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.ListTagsForStream\n  method: post\n  operationId: ListTagsForStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /#X-Amz-Target=Kinesis_20131202.RemoveTagsFromStream\n  method: post\n  operationId: RemoveTagsFromStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.PutResourcePolicy\n  method: post\n  operationId: PutResourcePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.GetResourcePolicy\n  method: post\n  operationId: GetResourcePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.DeleteResourcePolicy\n  method: post\n  operationId: DeleteResourcePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=Kinesis_20131202.DescribeLimits\n  method: post\n  operationId: DescribeLimits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams\n  method: post\n  operationId: CreateStream\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams\n  method: get\n  operationId: ListStreams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streams/{StreamName}/summary\n  method: get\n  operationId: DescribeStreamSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streams/{StreamName}\n  method: delete\n  operationId: DeleteStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams/{StreamName}/records\n  method: post\n  operationId: PutRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams/{StreamName}/records\n  method: get\n  operationId: GetRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streams/{StreamName}/records/batch\n  method: post\n  operationId: PutRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/agentic-access/amazon-kinesis-agentic-access.yml
summary_line: 39 operations · 36 acting · 2 human-in-the-loop
tags:
- Analytics
- Big Data
- Data Processing
- Real-Time
- Streaming
---
