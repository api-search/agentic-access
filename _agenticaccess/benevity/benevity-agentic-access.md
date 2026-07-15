---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Causes API
  slug: benevity-causes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Giving API
  slug: benevity-giving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Receipts API
  slug: benevity-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Spark Giving Opportunities API
  slug: benevity-spark-giving-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
- filename: benevity-openapi.yml
  format: yaml
  label: Benevity Spark Volunteer Opportunities API
  slug: benevity-spark-volunteer-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/openapi/benevity-openapi.yml
consequence_counts:
  physical: 1
  read: 4
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Benevity Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/card/transactions
operation_count: 8
overview: 'Benevity exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Benevity
provider_slug: benevity
slug: benevity-agentic-access
source_filename: benevity-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/benevity-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 4\n    connected: 4\n  by_consequence:\n    write: 3\n    read: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth2/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/causes\n  method: get\n  operationId: searchCauses\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /donations\n  method: post\n  operationId: createPostpaidDonation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/card/transactions\n  method: post\n  operationId: createCreditCardDonation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /receipts/{backendReceiptId}\n  method: get\n  operationId: getReceiptPdf\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /receipts/{backendReceiptId}/email\n  method: post\n  operationId: emailReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search/givingopportunities\n  method: get\n  operationId: searchGivingOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/volunteeropportunities\n  method: get\n  operationId: searchVolunteerOpportunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benevity/refs/heads/main/agentic-access/benevity-agentic-access.yml
summary_line: 8 operations · 4 acting
tags:
- Corporate Social Responsibility
- Workplace Giving
- Donations
- Volunteering
- Nonprofits
- Matching Gifts
- CSR
- ESG
---
