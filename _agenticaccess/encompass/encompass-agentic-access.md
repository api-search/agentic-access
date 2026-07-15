---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 22
api_specs:
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Loan Management API
  slug: encompass-loan-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Loan Pipeline API
  slug: encompass-loan-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Borrower Pair & Applications API
  slug: encompass-borrower-pair-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Contacts API
  slug: encompass-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass eFolder Documents & Attachments API
  slug: encompass-efolder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Milestones & Associates API
  slug: encompass-milestones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Conditions API
  slug: encompass-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Users API
  slug: encompass-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Webhooks API
  slug: encompass-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
consequence_counts:
  read: 22
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Encompass Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 43
overview: 'Encompass exposes 43 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 21 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Encompass
provider_slug: encompass
slug: encompass-agentic-access
source_filename: encompass-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/encompass-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    acting: 21\n    connected: 22\n  by_consequence:\n    write: 21\n    read: 22\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth2/v1/token\n  method: post\n  operationId: getToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v3/loans\n  method: post\n  operationId: createLoan\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v3/loans/{loanId}\n  method: get\n  operationId: getLoan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v3/loans/{loanId}\n  method: patch\n  operationId: updateLoan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v3/loans/{loanId}\n  method: delete\n  operationId: deleteLoan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v3/loans/{loanId}/ucdFields\n  method: get\n  operationId: getLoanUcdFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v1/loans/{loanId}/moveToFolder\n  method: patch\n  operationId: moveLoanToFolder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v3/loanPipeline\n  method: post\n  operationId: viewPipeline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v3/loanPipeline/cursor\n  method: post\n  operationId: createPipelineCursor\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v3/loanPipeline/canonicalNames\n  method: get\n  operationId: getPipelineCanonicalNames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v3/loans/{loanId}/applications\n  method: get\n  operationId: listBorrowerPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /encompass/v3/loans/{loanId}/applications\n  method: post\n  operationId: createBorrowerPair\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v3/loans/{loanId}/applications/{applicationId}\n  method: get\n  operationId: getBorrowerPair\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v3/loans/{loanId}/applications/{applicationId}\n  method: delete\n  operationId: deleteBorrowerPair\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /encompass/v1/borrowerContacts\n  method: get\n  operationId: listBorrowerContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v1/borrowerContacts\n  method: post\n  operationId: createBorrowerContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v1/borrowerContacts/{contactId}\n  method: get\n  operationId: getBorrowerContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v1/borrowerContacts/{contactId}\n  method: patch\n  operationId: updateBorrowerContact\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v1/businessContacts\n  method: get\n  operationId: listBusinessContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v1/businessContacts\n  method: post\n  operationId: createBusinessContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v3/loans/{loanId}/documents\n  method: get\n  operationId: listEfolderDocuments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v3/loans/{loanId}/documents\n  method: post\n  operationId: createEfolderDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v3/loans/{loanId}/attachments\n  method: get\n  operationId: listEfolderAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v3/loans/{loanId}/attachments/{attachmentId}\n  method: get\n  operationId: getEfolderAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /encompass/v3/loans/{loanId}/milestones\n  method: get\n  operationId: listMilestones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v3/loans/{loanId}/milestones/{milestoneId}\n  method: patch\n  operationId: updateMilestone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v3/loans/{loanId}/associates\n  method: get\n  operationId: listLoanAssociates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v1/loans/{loanId}/conditions/underwriting\n  method: get\n  operationId: listUnderwritingConditions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v1/loans/{loanId}/conditions/underwriting\n  method: post\n  operationId: createUnderwritingCondition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v1/loans/{loanId}/conditions/underwriting/{conditionId}\n  method: patch\n  operationId: updateUnderwritingCondition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v1/users\n  method: get\n\
  \  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v1/users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /encompass/v1/users/{userId}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encompass/v1/users/{userId}\n  method: patch\n  operationId: updateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/v1/subscriptions\n  method: get\n  operationId: listWebhookSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/v1/subscriptions\n  method: post\n  operationId: createWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/v1/subscriptions/{id}\n  method: get\n  operationId: getWebhookSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/v1/subscriptions/{id}\n  method: put\n  operationId:\
  \ updateWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/v1/subscriptions/{id}\n  method: delete\n  operationId: deleteWebhookSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/v1/resources\n  method: get\n  operationId: listWebhookResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/v1/resources/{id}/events\n  method: get\n  operationId: getWebhookResourceEvents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/v1/events\n  method: get\n  operationId: listWebhookEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/v1/events/{id}\n  method: get\n  operationId: getWebhookEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/agentic-access/encompass-agentic-access.yml
summary_line: 43 operations · 21 acting
tags:
- Mortgage
- Loan Origination
- LOS
- Fintech
- ICE Mortgage Technology
- Ellie Mae
- Lending
---
