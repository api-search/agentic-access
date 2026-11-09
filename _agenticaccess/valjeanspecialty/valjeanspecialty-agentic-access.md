---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 17
api_specs:
- filename: valjeanspecialty-account-api-openapi.yml
  format: yaml
  label: Valjean Specialty Account API
  slug: valjeanspecialty-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-account-api-openapi.yml
- filename: valjeanspecialty-answers-api-openapi.yml
  format: yaml
  label: Valjean Specialty Answers API
  slug: valjeanspecialty-answers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-answers-api-openapi.yml
- filename: valjeanspecialty-appetite-api-openapi.yml
  format: yaml
  label: Valjean Specialty Appetite API
  slug: valjeanspecialty-appetite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-appetite-api-openapi.yml
- filename: valjeanspecialty-bind-api-openapi.yml
  format: yaml
  label: Valjean Specialty Bind API
  slug: valjeanspecialty-bind-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-bind-api-openapi.yml
- filename: valjeanspecialty-documents-api-openapi.yml
  format: yaml
  label: Valjean Specialty Documents API
  slug: valjeanspecialty-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-documents-api-openapi.yml
- filename: valjeanspecialty-events-api-openapi.yml
  format: yaml
  label: Valjean Specialty Events API
  slug: valjeanspecialty-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-events-api-openapi.yml
- filename: valjeanspecialty-instant-quotes-api-openapi.yml
  format: yaml
  label: Valjean Specialty Instant quotes API
  slug: valjeanspecialty-instant-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-instant-quotes-api-openapi.yml
- filename: valjeanspecialty-invoices-api-openapi.yml
  format: yaml
  label: Valjean Specialty Invoices API
  slug: valjeanspecialty-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-invoices-api-openapi.yml
- filename: valjeanspecialty-policies-api-openapi.yml
  format: yaml
  label: Valjean Specialty Policies API
  slug: valjeanspecialty-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-policies-api-openapi.yml
- filename: valjeanspecialty-public-api-openapi.yml
  format: yaml
  label: Valjean Specialty Public API
  slug: valjeanspecialty-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-public-api-openapi.yml
- filename: valjeanspecialty-quotes-api-openapi.yml
  format: yaml
  label: Valjean Specialty Quotes API
  slug: valjeanspecialty-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-quotes-api-openapi.yml
- filename: valjeanspecialty-requirements-api-openapi.yml
  format: yaml
  label: Valjean Specialty Requirements API
  slug: valjeanspecialty-requirements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-requirements-api-openapi.yml
- filename: valjeanspecialty-submissions-api-openapi.yml
  format: yaml
  label: Valjean Specialty Submissions API
  slug: valjeanspecialty-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-submissions-api-openapi.yml
- filename: valjeanspecialty-webhooks-api-openapi.yml
  format: yaml
  label: Valjean Specialty Webhooks API
  slug: valjeanspecialty-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valjeanspecialty/openapi/valjeanspecialty-webhooks-api-openapi.yml
consequence_counts:
  physical: 4
  read: 17
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Valjeanspecialty Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /intake
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /submissions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /submissions/{id}/bind-requests/{bindRequestId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhooks/{id}/test
operation_count: 32
overview: 'Valjean Specialty exposes 32 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 11 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Valjean Specialty
provider_slug: valjeanspecialty
slug: valjeanspecialty-agentic-access
source_filename: valjeanspecialty-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/valjeanspecialty-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 17\n    acting: 15\n  by_consequence:\n    read: 17\n    write: 11\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appetite\n  method: post\n  operationId: checkAppetite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /requirements\n  method: post\n  operationId: getRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions\n  method: get\n  operationId: listSubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions\n  method: post\n  operationId: createSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - submit\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /intake\n  method: post\n  operationId: sendDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - submit\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submissions/{id}\n  method: get\n  operationId: getSubmission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions/{id}/answers\n  method: patch\n  operationId: answerQuestions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - submit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submissions/{id}/answers\n  method: post\n  operationId: answerQuestionsViaPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - submit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submissions/{id}/flags\n  method: get\n  operationId: getUnderwriterFlags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions/{id}/documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions/{id}/documents\n\
  \  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - submit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submissions/{id}/documents/upload-url\n  method: post\n  operationId: getUploadLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - submit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submissions/{id}/documents/complete\n  method: post\n  operationId: completeUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - submit\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submissions/{id}/documents/{docId}\n  method: get\n  operationId: getDocumentLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions/{id}/quotes\n  method: get\n  operationId: listQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions/{id}/quotes/{quoteId}/bind-request\n  method: post\n  operationId: requestBind\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - submit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /submissions/{id}/bind-requests\n  method: get\n  operationId: listBindRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submissions/{id}/bind-requests/{bindRequestId}\n  method: delete\n  operationId: withdrawBindRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - submit\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submissions/{id}/instant-quotes\n  method: post\n  operationId: askInstantQuotes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - submit\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policies\n  method: get\n  operationId: listPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /policies/{id}\n  method: get\n  operationId: getPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoices\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/appetite\n  method: post\n  operationId: publicCheckAppetite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read\n- path: /api/appetite\n  method: get\n  operationId: publicCheckAppetiteGet\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /api/guides\n  method: get\n  operationId: listGuides\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n- path: /api/guides/{key}\n  method: get\n  operationId: getGuide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read\n"
source_yaml_url: https://artifacts.apis.io/valjeanspecialty/agentic-access/valjeanspecialty-agentic-access.yml
summary_line: 32 operations · 15 acting
tags:
- Insurance
- Wholesale
- Brokerage
- E&S
- Insurance Tech
---
