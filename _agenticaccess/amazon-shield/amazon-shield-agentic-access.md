---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 1
api_specs:
- filename: amazon-shield-amazon-shield-rest-api-api-openapi.yml
  format: yaml
  label: Amazon Shield Amazon Shield REST API
  slug: amazon-shield-amazon-shield-rest-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/openapi/amazon-shield-amazon-shield-rest-api-api-openapi.yml
consequence_counts:
  read: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Shield Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Amazon Shield exposes 7 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Shield
provider_slug: amazon-shield
slug: amazon-shield-agentic-access
source_filename: amazon-shield-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/amazon-shield-amazon-shield-rest-api-api-openapi.yml, openapi/amazon-shield-createprotectiongroup-api-openapi.yml,\n  openapi/amazon-shield-createsubscription-api-openapi.yml, openapi/amazon-shield-describeattack-api-openapi.yml,\n  openapi/amazon-shield-describeprotection-api-openapi.yml, openapi/amazon-shield-describesubscription-api-openapi.yml,\n  openapi/amazon-shield-listprotections-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 6\n    connected: 1\n  by_consequence:\n    write: 6\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: createProtection\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#CreateProtectionGroup\n  method: post\n  operationId: createProtectionGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#CreateSubscription\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeAttack\n  method: post\n\
  \  operationId: describeAttack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeProtection\n  method: post\n  operationId: describeProtection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#DescribeSubscription\n  method: post\n  operationId: describeSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /#ListProtections\n  method: post\n  operationId: listProtections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/agentic-access/amazon-shield-agentic-access.yml
summary_line: 7 operations · 6 acting
tags:
- DDoS Protection
- Networking
- Security
---
