---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Quotes API
  slug: coterie-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Policies API
  slug: coterie-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Applications API
  slug: coterie-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Industry / NAICS API
  slug: coterie-industry-naics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Documents API
  slug: coterie-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Webhooks API
  slug: coterie-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
consequence_counts:
  read: 7
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Coterie Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Coterie Insurance exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Coterie Insurance
provider_slug: coterie
slug: coterie-agentic-access
source_filename: coterie-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/coterie-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 6\n    connected: 7\n  by_consequence:\n    write: 6\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /commercial/applications\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commercial/applications/{applicationId}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial/applications/{applicationId}\n  method: put\n  operationId: updateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commercial/quotes\n  method: post\n  operationId: createQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commercial/quotes/{quoteId}\n  method: get\n  operationId: getQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial/quotes/{quoteId}/underwriting-questions\n  method: get\n  operationId: getUnderwritingQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial/policies\n  method: post\n  operationId: bindPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commercial/policies/{policyId}\n  method: get\n  operationId: getPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /industry-classifications\n  method: get\n  operationId: searchIndustryClassifications\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commercial/policies/{policyId}/documents\n  method: get\n  operationId: getPolicyDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: delete\n  operationId:\
  \ deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/agentic-access/coterie-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Insurance
- Commercial Insurance
- Small Business
- Embedded Insurance
- Insurtech
---
