---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: sendbridge-com-account-api-openapi.yml
  format: yaml
  label: SendBridge Account API
  slug: sendbridge-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendbridge-com/openapi/sendbridge-com-account-api-openapi.yml
- filename: sendbridge-com-dmarc-api-openapi.yml
  format: yaml
  label: SendBridge DMARC API
  slug: sendbridge-com-dmarc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendbridge-com/openapi/sendbridge-com-dmarc-api-openapi.yml
- filename: sendbridge-com-mail-tester-api-openapi.yml
  format: yaml
  label: SendBridge Mail Tester API
  slug: sendbridge-com-mail-tester-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendbridge-com/openapi/sendbridge-com-mail-tester-api-openapi.yml
- filename: sendbridge-com-validation-api-openapi.yml
  format: yaml
  label: SendBridge Validation API
  slug: sendbridge-com-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendbridge-com/openapi/sendbridge-com-validation-api-openapi.yml
consequence_counts:
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sendbridge Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'SendBridge exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SendBridge
provider_slug: sendbridge-com
slug: sendbridge-com-agentic-access
source_filename: sendbridge-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/sendbridge-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 7\n    acting: 2\n  by_consequence:\n    read: 7\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /dmarc/domains\n  method: get\n  operationId: listDmarcDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dmarc/domains/{id}/stats\n  method: get\n  operationId: getDmarcDomainStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dmarc/domains/{id}/reports\n\
  \  method: get\n  operationId: listDmarcReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailtester/tests\n  method: post\n  operationId: createMailTest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mailtester/get_address\n  method: post\n  operationId: getMailTestAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mailtester/tests/{token}\n  method: get\n  operationId: getMailTestResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /mailtester/get_result\n  method: post\n  operationId: getMailTestResultRpc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /validation/verify\n  method: post\n  operationId: verifyEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/sendbridge-com/agentic-access/sendbridge-com-agentic-access.yml
summary_line: 9 operations · 2 acting
tags:
- Email
- Verification
- Deliverability
- Validation
- Marketing
- Services
---
