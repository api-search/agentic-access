---
acting_count: 27
action_class_counts:
  acting: 27
api_specs:
- filename: amazon-snow-family.yaml
  format: yaml
  label: AWS Snow Device Management API
  slug: aws-snow-device-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/openapi/amazon-snow-family.yaml
consequence_counts:
  physical: 3
  write: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Snow Family Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=AWSIESnowballJobManagementService.CreateReturnShippingLabel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=AWSIESnowballJobManagementService.DescribeReturnShippingLabel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /#X-Amz-Target=AWSIESnowballJobManagementService.UpdateJobShipmentState
operation_count: 27
overview: 'Amazon Snow Family exposes 27 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 write and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
slug: amazon-snow-family-agentic-access
source_filename: amazon-snow-family-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-snow-family.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 27\n  by_consequence:\n    write: 24\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.CancelCluster\n  method: post\n  operationId: CancelCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.CancelJob\n  method: post\n  operationId:\
  \ CancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.CreateAddress\n  method: post\n  operationId: CreateAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.CreateCluster\n  method: post\n  operationId: CreateCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.CreateJob\n  method: post\n  operationId: CreateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.CreateLongTermPricing\n  method: post\n  operationId: CreateLongTermPricing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.CreateReturnShippingLabel\n  method: post\n  operationId: CreateReturnShippingLabel\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.DescribeAddress\n  method: post\n  operationId: DescribeAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.DescribeAddresses\n  method: post\n  operationId: DescribeAddresses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.DescribeCluster\n  method: post\n  operationId: DescribeCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.DescribeJob\n  method: post\n  operationId: DescribeJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.DescribeReturnShippingLabel\n\
  \  method: post\n  operationId: DescribeReturnShippingLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.GetJobManifest\n  method: post\n  operationId: GetJobManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.GetJobUnlockCode\n  method: post\n  operationId: GetJobUnlockCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.GetSnowballUsage\n  method: post\n  operationId: GetSnowballUsage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.GetSoftwareUpdates\n  method: post\n  operationId: GetSoftwareUpdates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.ListClusterJobs\n\
  \  method: post\n  operationId: ListClusterJobs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.ListClusters\n  method: post\n  operationId: ListClusters\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.ListCompatibleImages\n  method: post\n  operationId: ListCompatibleImages\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.ListJobs\n  method: post\n  operationId: ListJobs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.ListLongTermPricing\n  method: post\n  operationId: ListLongTermPricing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.ListPickupLocations\n\
  \  method: post\n  operationId: ListPickupLocations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.ListServiceVersions\n  method: post\n  operationId: ListServiceVersions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.UpdateCluster\n  method: post\n  operationId: UpdateCluster\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.UpdateJob\n  method: post\n  operationId: UpdateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.UpdateJobShipmentState\n  method: post\n  operationId: UpdateJobShipmentState\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#X-Amz-Target=AWSIESnowballJobManagementService.UpdateLongTermPricing\n\
  \  method: post\n  operationId: UpdateLongTermPricing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/agentic-access/amazon-snow-family-agentic-access.yml
summary_line: 27 operations · 27 acting
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
---
