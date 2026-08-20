---
acting_count: 6
action_class_counts:
  acting: 6
api_specs:
- filename: amazon-textract-async-operations-api-openapi.yml
  format: yaml
  label: Amazon Textract Async Operations API
  slug: amazon-textract-async-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-textract/refs/heads/main/openapi/amazon-textract-async-operations-api-openapi.yml
- filename: amazon-textract-document-analysis-api-openapi.yml
  format: yaml
  label: Amazon Textract Document Analysis API
  slug: amazon-textract-document-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-textract/refs/heads/main/openapi/amazon-textract-document-analysis-api-openapi.yml
- filename: amazon-textract-expense-analysis-api-openapi.yml
  format: yaml
  label: Amazon Textract Expense Analysis API
  slug: amazon-textract-expense-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-textract/refs/heads/main/openapi/amazon-textract-expense-analysis-api-openapi.yml
- filename: amazon-textract-id-analysis-api-openapi.yml
  format: yaml
  label: Amazon Textract ID Analysis API
  slug: amazon-textract-id-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-textract/refs/heads/main/openapi/amazon-textract-id-analysis-api-openapi.yml
- filename: amazon-textract-text-detection-api-openapi.yml
  format: yaml
  label: Amazon Textract Text Detection API
  slug: amazon-textract-text-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-textract/refs/heads/main/openapi/amazon-textract-text-detection-api-openapi.yml
consequence_counts:
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Textract Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Amazon Textract exposes 6 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Textract
provider_slug: amazon-textract
slug: amazon-textract-agentic-access
source_filename: amazon-textract-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amazon-textract-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 6\n  by_consequence:\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: post\n  operationId: DetectDocumentText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#AnalyzeDocument\n  method: post\n  operationId: AnalyzeDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#StartDocumentTextDetection\n  method: post\n  operationId: StartDocumentTextDetection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#GetDocumentTextDetection\n  method: post\n  operationId: GetDocumentTextDetection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#AnalyzeExpense\n  method: post\n  operationId: AnalyzeExpense\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /#AnalyzeID\n  method: post\n  operationId: AnalyzeID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-textract/refs/heads/main/agentic-access/amazon-textract-agentic-access.yml
summary_line: 6 operations · 6 acting
tags:
- Document Processing
- Machine-Learning
- OCR
---
