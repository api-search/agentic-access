---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 3
api_specs:
- filename: amazon-marketplace-cancelchangeset-catalog-changesetid-api-openapi.yml
  format: yaml
  label: Amazon Marketplace CancelChangeSet#catalog&changeSetId API
  slug: amazon-marketplace-cancelchangeset-catalog-changesetid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-cancelchangeset-catalog-changesetid-api-openapi.yml
- filename: amazon-marketplace-deleteresourcepolicy-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon Marketplace DeleteResourcePolicy#resourceArn API
  slug: amazon-marketplace-deleteresourcepolicy-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-deleteresourcepolicy-resourcearn-api-openapi.yml
- filename: amazon-marketplace-describechangeset-catalog-changesetid-api-openapi.yml
  format: yaml
  label: Amazon Marketplace DescribeChangeSet#catalog&changeSetId API
  slug: amazon-marketplace-describechangeset-catalog-changesetid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-describechangeset-catalog-changesetid-api-openapi.yml
- filename: amazon-marketplace-describeentity-catalog-entityid-api-openapi.yml
  format: yaml
  label: Amazon Marketplace DescribeEntity#catalog&entityId API
  slug: amazon-marketplace-describeentity-catalog-entityid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-describeentity-catalog-entityid-api-openapi.yml
- filename: amazon-marketplace-getresourcepolicy-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon Marketplace GetResourcePolicy#resourceArn API
  slug: amazon-marketplace-getresourcepolicy-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-getresourcepolicy-resourcearn-api-openapi.yml
- filename: amazon-marketplace-listchangesets-api-openapi.yml
  format: yaml
  label: Amazon Marketplace ListChangeSets API
  slug: amazon-marketplace-listchangesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-listchangesets-api-openapi.yml
- filename: amazon-marketplace-listentities-api-openapi.yml
  format: yaml
  label: Amazon Marketplace ListEntities API
  slug: amazon-marketplace-listentities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-listentities-api-openapi.yml
- filename: amazon-marketplace-listtagsforresource-api-openapi.yml
  format: yaml
  label: Amazon Marketplace ListTagsForResource API
  slug: amazon-marketplace-listtagsforresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-listtagsforresource-api-openapi.yml
- filename: amazon-marketplace-putresourcepolicy-api-openapi.yml
  format: yaml
  label: Amazon Marketplace PutResourcePolicy API
  slug: amazon-marketplace-putresourcepolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-putresourcepolicy-api-openapi.yml
- filename: amazon-marketplace-startchangeset-api-openapi.yml
  format: yaml
  label: Amazon Marketplace StartChangeSet API
  slug: amazon-marketplace-startchangeset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-startchangeset-api-openapi.yml
- filename: amazon-marketplace-tagresource-api-openapi.yml
  format: yaml
  label: Amazon Marketplace TagResource API
  slug: amazon-marketplace-tagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-tagresource-api-openapi.yml
- filename: amazon-marketplace-untagresource-api-openapi.yml
  format: yaml
  label: Amazon Marketplace UntagResource API
  slug: amazon-marketplace-untagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-untagresource-api-openapi.yml
consequence_counts:
  read: 3
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Marketplace Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Amazon Marketplace exposes 12 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
slug: amazon-marketplace-agentic-access
source_filename: amazon-marketplace-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-marketplace-openapi-original.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 9\n    connected: 3\n  by_consequence:\n    write: 9\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /CancelChangeSet#catalog&changeSetId\n  method: patch\n  operationId: CancelChangeSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /DeleteResourcePolicy#resourceArn\n  method: delete\n  operationId: DeleteResourcePolicy\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /DescribeChangeSet#catalog&changeSetId\n  method: get\n  operationId: DescribeChangeSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /DescribeEntity#catalog&entityId\n  method: get\n  operationId: DescribeEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /GetResourcePolicy#resourceArn\n  method: get\n  operationId: GetResourcePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ListChangeSets\n\
  \  method: post\n  operationId: ListChangeSets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ListEntities\n  method: post\n  operationId: ListEntities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ListTagsForResource\n  method: post\n  operationId: ListTagsForResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /PutResourcePolicy\n  method: post\n  operationId: PutResourcePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /StartChangeSet\n  method: post\n  operationId: StartChangeSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /TagResource\n  method: post\n  operationId: TagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /UntagResource\n  method: post\n  operationId: UntagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/agentic-access/amazon-marketplace-agentic-access.yml
summary_line: 12 operations · 9 acting
tags:
- Commerce
- ISV
- Marketplace
- Software Catalog
---
