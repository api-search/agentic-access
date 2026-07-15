---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 17
api_specs:
- filename: tint-openapi.yml
  format: yaml
  label: Tint Programs API
  slug: tint-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Quotes API
  slug: tint-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Policies API
  slug: tint-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Claims API
  slug: tint-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Decisions API
  slug: tint-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Questionnaires API
  slug: tint-questionnaires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Webhooks API
  slug: tint-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
consequence_counts:
  physical: 3
  read: 17
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tint Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /claim/{claimId}/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /claim/{id}/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /policy/{id}/payment
operation_count: 41
overview: 'Tint exposes 41 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 21 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tint
provider_slug: tint
slug: tint-agentic-access
source_filename: tint-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tint-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 41\n  by_action_class:\n    connected: 17\n    acting: 24\n  by_consequence:\n    read: 17\n    write: 21\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /insurance-products\n  method: get\n  operationId: listInsuranceProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insurance-products/{productSlug}/plans\n  method: get\n  operationId: listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /policy\n  method: post\n  operationId: createPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/{id}\n  method: get\n  operationId: getPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/{id}\n  method: put\n  operationId: updatePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/{id}/issue\n  method: post\n  operationId: issuePolicy\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/{id}/report-usage\n  method: post\n  operationId: reportPolicyUsage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/{id}/payment\n  method: post\n  operationId: recordPolicyPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /policy/{id}/cancel\n  method: post\n  operationId: cancelPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/{id}/void\n  method: post\n  operationId: voidPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/{policyId}/quotes\n  method: get\n  operationId: getPolicyQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/{policyId}/decisions/{decisionType}\n  method:\
  \ get\n  operationId: getPolicyDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/{policyId}/scores\n  method: get\n  operationId: computePolicyScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/{policyId}/score/{scoreId}\n  method: get\n  operationId: getPolicyScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/{policyId}/endorsement\n  method: post\n  operationId: createEndorsement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /policy/{policyId}/endorsements\n  method: get\n  operationId: listEndorsements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/{policyId}/endorsement/{id}\n  method: get\n  operationId: getEndorsement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/{policyId}/endorsement/{id}\n  method: put\n  operationId: updateEndorsement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/{policyId}/endorsement/{id}/approve\n  method: post\n  operationId: approveEndorsement\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/{policyId}/endorsement/{id}/cancel\n  method: post\n  operationId: cancelEndorsement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/{policyId}/endorsement/{id}/quotes\n  method: get\n  operationId: getEndorsementQuotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/{policyId}/endorsement/{id}/decisions/{decisionType}\n  method: get\n  operationId: getEndorsementDecision\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/{policyId}/questionnaire/{slug}\n  method: get\n  operationId: getPolicyQuestionnaire\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/{policyId}/claim\n  method: post\n  operationId: createClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/{policyId}/claims\n  method: get\n  operationId: listPolicyClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/{policyId}/claim/{claimId}\n\
  \  method: put\n  operationId: updatePolicyClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims\n  method: get\n  operationId: listClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claim/{id}\n  method: get\n  operationId: getClaim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claim/{id}\n  method: put\n  operationId: updateClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/{id}/receive\n  method: post\n  operationId: receiveClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/{id}/incomplete\n  method: post\n  operationId: markClaimIncomplete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/{id}/review\n  method: post\n  operationId: reviewClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/{id}/approve\n  method: post\n  operationId: approveClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/{id}/settle\n  method: post\n  operationId: settleClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/{id}/deny\n  method: post\n  operationId: denyClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/{id}/withdraw\n  method: post\n  operationId: withdrawClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/{claimId}/notes\n  method: get\n  operationId: listClaimNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claim/{claimId}/note\n  method: post\n  operationId: createClaimNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/{claimId}/note/{noteId}\n  method: put\n  operationId: updateClaimNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/{claimId}/payment\n  method: post\n  operationId: createClaimPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/{claimId}/upload-url\n  method: get\n\
  \  operationId: getClaimUploadUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/agentic-access/tint-agentic-access.yml
summary_line: 41 operations · 24 acting
tags:
- Insurance
- Embedded Insurance
- InsurTech
- Insurance as a Service
- Protection
---
