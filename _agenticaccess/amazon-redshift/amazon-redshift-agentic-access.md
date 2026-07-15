---
acting_count: 10
action_class_counts:
  acting: 10
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon Redshift API
  slug: amazon-redshift-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/redshift/2012-12-01/openapi.yaml
- filename: amazon-redshift-data-api-openapi.yml
  format: yaml
  label: Amazon Redshift Data API
  slug: amazon-redshift-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/openapi/amazon-redshift-data-api-openapi.yml
consequence_counts:
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Redshift Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Amazon Redshift exposes 10 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Redshift
provider_slug: amazon-redshift
slug: amazon-redshift-agentic-access
source_filename: amazon-redshift-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-redshift-data-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 10\n  by_consequence:\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /ExecuteStatement\n  method: post\n  operationId: executeStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BatchExecuteStatement\n  method: post\n  operationId: batchExecuteStatement\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /DescribeStatement\n  method: post\n  operationId: describeStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ListStatements\n  method: post\n  operationId: listStatements\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CancelStatement\n  method: post\n  operationId: cancelStatement\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GetStatementResult\n  method: post\n  operationId: getStatementResult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ListDatabases\n  method: post\n  operationId: listDatabases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ListSchemas\n\
  \  method: post\n  operationId: listSchemas\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ListTables\n  method: post\n  operationId: listTables\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /DescribeTable\n  method: post\n  operationId: describeTable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/agentic-access/amazon-redshift-agentic-access.yml
summary_line: 10 operations · 10 acting
tags:
- Analytics
- Big Data
- Cloud
- Data Lake
- Data Warehouse
- ETL
- Machine Learning
- Serverless
- SQL
---
