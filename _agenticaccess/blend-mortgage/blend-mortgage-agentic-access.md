---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 27
api_specs:
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Home Lending Applications API
  slug: blend-mortgage-home-lending-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Borrowers & Parties API
  slug: blend-mortgage-borrowers-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Documents & Disclosures API
  slug: blend-mortgage-documents-disclosures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Products & Pricing API
  slug: blend-mortgage-products-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Closings & eSignature API
  slug: blend-mortgage-closings-esign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Follow-ups (Tasks) API
  slug: blend-mortgage-follow-ups-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Events & Webhooks API
  slug: blend-mortgage-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Consumer Lending & Deposit Accounts API
  slug: blend-mortgage-consumer-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Lenders & Assignments API
  slug: blend-mortgage-lenders-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
- filename: blend-mortgage-openapi.yml
  format: yaml
  label: Blend Reporting API
  slug: blend-mortgage-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/openapi/blend-mortgage-openapi.yml
consequence_counts:
  physical: 2
  read: 27
  safety-critical: 1
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Blend Mortgage Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /applications/{id}/assignments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /closings/{closingId}/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /consumer-lending/applications/{id}
operation_count: 52
overview: 'Blend exposes 52 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read, 22 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Blend
provider_slug: blend-mortgage
slug: blend-mortgage-agentic-access
source_filename: blend-mortgage-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/blend-mortgage-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 27\n    acting: 25\n  by_consequence:\n    read: 27\n    write: 22\n    physical: 2\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /home-lending/applications\n  method: get\n  operationId: listHomeLendingApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /home-lending/applications\n  method: post\n  operationId: createHomeLendingApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /home-lending/applications/{id}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /home-lending/applications/{id}\n  method: patch\n  operationId: patchApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /home-lending/applications/{id}\n  method: delete\n  operationId: deleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /home-lending/applications/{id}/file-export\n  method: get\n  operationId: exportApplicationFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /home-lending/applications/export-statuses\n  method: get\n  operationId: getExportStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /home-lending/applications/{id}/export-status\n  method: post\n  operationId: setExportStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /applications/{id}/parties\n  method: get\n  operationId: listParties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{id}/parties\n  method: post\n  operationId: createParty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{id}/parties/{partyId}\n  method: patch\n  operationId: patchParty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{id}/parties/{partyId}\n\
  \  method: delete\n  operationId: deleteParty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{id}/borrower-positions\n  method: get\n  operationId: getBorrowerPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{id}/borrower-positions\n  method: put\n  operationId: putBorrowerPositions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{id}/documents\n  method: get\n \
  \ operationId: getApplicationDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: get\n  operationId: getDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{documentId}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{documentId}\n  method:\
  \ patch\n  operationId: patchDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{documentId}/metadata\n  method: get\n  operationId: getDocumentMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{id}/product\n  method: put\n  operationId: putPricedProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /closings\n  method: post\n  operationId: createClosing\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /closings\n  method: get\n  operationId: listClosings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /closings/{closingId}\n  method: get\n  operationId: getClosing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /closings/{closingId}\n  method: patch\n  operationId: updateClosing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /closings/{closingId}/send\n  method: post\n  operationId: submitClosing\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{id}/packages\n  method: get\n  operationId: listPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{id}/packages\n  method: post\n  operationId: createPackage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /applications/{id}/packages/{packageId}/issue\n  method: post\n  operationId: issuePackage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{id}/follow-ups\n  method: get\n  operationId: listFollowUps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{id}/follow-ups\n  method: post\n  operationId: createFollowUp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /applications/{id}/follow-ups/{followUpId}\n  method: get\n  operationId: getFollowUp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{id}/follow-ups/{followUpId}\n  method: patch\n  operationId: patchFollowUp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{id}/follow-ups/{followUpId}\n  method: delete\n  operationId: removeFollowUp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /events\n  method: get\n  operationId: getEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/descriptions\n  method: get\n  operationId: getEventDescriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{eventId}/status\n  method: post\n  operationId: setEventStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /consumer-lending/applications/{id}\n  method: get\n  operationId: getConsumerLendingApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consumer-lending/applications/{id}\n  method: patch\n  operationId: patchConsumerLendingApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account-opening/applications/{id}\n  method: get\n  operationId: getAccountOpeningApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deposit-accounts/applications\n  method: get\n\
  \  operationId: listDepositAccountApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deposit-accounts/products\n  method: get\n  operationId: listDepositAccountProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lenders\n  method: get\n  operationId: listLenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lenders\n  method: post\n  operationId: createLenders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lenders\n\
  \  method: patch\n  operationId: updateLenders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lenders\n  method: delete\n  operationId: removeLenders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{id}/assignments\n  method: get\n  operationId: listAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{id}/assignments\n  method: put\n  operationId: overrideAssignments\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /reports/loans\n  method: get\n  operationId: getLoansReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/lenders\n  method: get\n  operationId: getLendersReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/borrowers\n  method: get\n  operationId: getBorrowersReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blend-mortgage/refs/heads/main/agentic-access/blend-mortgage-agentic-access.yml
summary_line: 52 operations · 25 acting · 1 human-in-the-loop
tags:
- Digital Lending
- Mortgage
- Consumer Lending
- Account Opening
- FinTech
- Loan Origination
- Banking
- Financial Services
---
