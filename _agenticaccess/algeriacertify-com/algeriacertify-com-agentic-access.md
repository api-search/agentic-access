---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: algeriacertify-com-certificates-api-openapi.yml
  format: yaml
  label: Algeria Certify Certificates API
  slug: algeriacertify-com-certificates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algeriacertify-com/openapi/algeriacertify-com-certificates-api-openapi.yml
- filename: algeriacertify-com-system-api-openapi.yml
  format: yaml
  label: Algeria Certify System API
  slug: algeriacertify-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algeriacertify-com/openapi/algeriacertify-com-system-api-openapi.yml
- filename: algeriacertify-com-verification-api-openapi.yml
  format: yaml
  label: Algeria Certify Verification API
  slug: algeriacertify-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algeriacertify-com/openapi/algeriacertify-com-verification-api-openapi.yml
- filename: algeriacertify-com-zapier-api-openapi.yml
  format: yaml
  label: Algeria Certify Zapier API
  slug: algeriacertify-com-zapier-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/algeriacertify-com/openapi/algeriacertify-com-zapier-api-openapi.yml
consequence_counts:
  read: 6
  safety-critical: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Algeriacertify Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /institution/certificates/{id}/revoke
operation_count: 9
overview: 'Algeria Certify exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 2 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Algeria Certify
provider_slug: algeriacertify-com
slug: algeriacertify-com-agentic-access
source_filename: algeriacertify-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/algeriacertify-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 6\n    acting: 3\n  by_consequence:\n    read: 6\n    write: 2\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zapier/auth/test\n  method: get\n  operationId: zapierAuthTest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zapier/triggers/new-certificate\n\
  \  method: get\n  operationId: zapierTriggerNewCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zapier/triggers/revoked-certificate\n  method: get\n  operationId: zapierTriggerRevokedCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zapier/actions/issue-certificate\n  method: post\n  operationId: zapierActionIssueCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /institution/certificates\n  method: post\n  operationId: issueCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /institution/issued-certificates\n  method: get\n  operationId: listIssuedCertificates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /institution/certificates/{id}/revoke\n  method: patch\n  operationId: revokeCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /public/verify/{token}\n  method: get\n  operationId: verifyCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/algeriacertify-com/agentic-access/algeriacertify-com-agentic-access.yml
summary_line: 9 operations · 3 acting · 1 human-in-the-loop
tags:
- Certificate Management
- Digital Verification
- Education
- Algeria
- Security
---
