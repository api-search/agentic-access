---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 17
api_specs:
- filename: email-on-acid-openapi.yml
  format: yaml
  label: Email on Acid API
  slug: email-on-acid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/email-on-acid/refs/heads/main/openapi/email-on-acid-openapi.yml
consequence_counts:
  read: 17
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Email On Acid Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Email on Acid exposes 23 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Email on Acid
provider_slug: email-on-acid
slug: email-on-acid-agentic-access
source_filename: email-on-acid-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/email-on-acid-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 17\n    acting: 6\n  by_consequence:\n    read: 17\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /auth\n  method: get\n  operationId: testAuth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/clients\n  method: get\n  operationId: getEmailClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/clients/default\n  method: get\n\
  \  operationId: getDefaultEmailClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/clients/default\n  method: put\n  operationId: setDefaultEmailClients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/tests\n  method: get\n  operationId: getEmailTests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/tests\n  method: post\n  operationId: createEmailTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/tests/{testId}\n  method: get\n  operationId: getEmailTest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/tests/{testId}\n  method: delete\n  operationId: deleteEmailTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/tests/{testId}/results\n  method: get\n  operationId: getEmailTestResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/tests/{testId}/results/{clientId}\n  method: get\n  operationId:\
  \ getEmailTestResultByClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/tests/{testId}/results/reprocess\n  method: put\n  operationId: reprocessScreenshots\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/tests/{testId}/content\n  method: get\n  operationId: getEmailTestContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/tests/{testId}/content/inlinecss\n  method: get\n  operationId: getEmailTestContentInlineCss\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /email/tests/{testId}/content/textonly\n  method: get\n  operationId: getEmailTestContentTextOnly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/tests/{testId}/spam/results\n  method: get\n  operationId: getEmailTestSpamResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/tests/{testId}/spam/seedlist\n  method: get\n  operationId: getEmailTestSpamSeedList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spam/clients\n  method: get\n  operationId: getSpamClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /spam/tests\n  method: get\n  operationId: getSpamTests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spam/tests\n  method: post\n  operationId: createSpamTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spam/tests/{testId}\n  method: get\n  operationId: getSpamTestResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spam/tests/{testId}\n  method: delete\n  operationId: deleteSpamTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spam/tests/{testId}/seedlist\n  method: get\n  operationId: getSpamTestSeedList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /spam/seedlist\n  method: get\n  operationId: reserveSeedList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/email-on-acid/refs/heads/main/agentic-access/email-on-acid-agentic-access.yml
summary_line: 23 operations · 6 acting
tags:
- Email Testing
- Email Previews
- Email Clients
- Spam Testing
- Accessibility
- HTML Validation
- Email Quality Assurance
- Pre-Deployment Testing
---
