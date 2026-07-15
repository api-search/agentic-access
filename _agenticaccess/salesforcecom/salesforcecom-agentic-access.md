---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 8
api_specs:
- filename: salesforcecom-rest-openapi.yml
  format: yaml
  label: Salesforce REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforcecom/refs/heads/main/openapi/salesforcecom-rest-openapi.yml
consequence_counts:
  read: 8
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Salesforcecom Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Salesforce exposes 13 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Salesforce
provider_slug: salesforcecom
slug: salesforcecom-agentic-access
source_filename: salesforcecom-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/salesforcecom-rest-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 8\n    acting: 5\n  by_consequence:\n    read: 8\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /services/data\n  method: get\n  operationId: listApiVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/data/v{version}/sobjects\n  method: get\n  operationId: listSObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/data/v{version}/sobjects/{sObjectName}\n\
  \  method: post\n  operationId: createSObjectRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/data/v{version}/sobjects/{sObjectName}/describe\n  method: get\n  operationId: describeSObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/data/v{version}/sobjects/{sObjectName}/{id}\n  method: get\n  operationId: getSObjectRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/data/v{version}/sobjects/{sObjectName}/{id}\n  method: patch\n  operationId: updateSObjectRecord\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/data/v{version}/sobjects/{sObjectName}/{id}\n  method: delete\n  operationId: deleteSObjectRecord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/data/v{version}/query\n  method: get\n  operationId: executeQuery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/data/v{version}/queryAll\n  method: get\n  operationId: executeQueryAll\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/data/v{version}/search\n  method: get\n  operationId: executeSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/data/v{version}/limits\n  method: get\n  operationId: getOrgLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/data/v{version}/composite/batch\n  method: post\n  operationId: compositeBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/data/v{version}/composite\n  method: post\n \
  \ operationId: compositeRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforcecom/refs/heads/main/agentic-access/salesforcecom-agentic-access.yml
summary_line: 13 operations · 5 acting
tags:
- CRM
- Cloud
- Sales
- Marketing
- Automation
- AI
- Fortune 500
---
