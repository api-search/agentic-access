---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 9
api_specs:
- filename: anymailfinder-com-account-api-openapi.yml
  format: yaml
  label: Anymail Finder Account API
  slug: anymailfinder-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-account-api-openapi.yml
- filename: anymailfinder-com-bulk-api-openapi.yml
  format: yaml
  label: Anymail Finder Bulk API
  slug: anymailfinder-com-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-bulk-api-openapi.yml
- filename: anymailfinder-com-domain-api-openapi.yml
  format: yaml
  label: Anymail Finder Domain API
  slug: anymailfinder-com-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-domain-api-openapi.yml
- filename: anymailfinder-com-find-email-api-openapi.yml
  format: yaml
  label: Anymail Finder Find Email API
  slug: anymailfinder-com-find-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-find-email-api-openapi.yml
- filename: anymailfinder-com-geo-lead-api-openapi.yml
  format: yaml
  label: Anymail Finder Geo Lead API
  slug: anymailfinder-com-geo-lead-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-geo-lead-api-openapi.yml
- filename: anymailfinder-com-report-api-openapi.yml
  format: yaml
  label: Anymail Finder Report API
  slug: anymailfinder-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-report-api-openapi.yml
- filename: anymailfinder-com-verify-email-api-openapi.yml
  format: yaml
  label: Anymail Finder Verify Email API
  slug: anymailfinder-com-verify-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anymailfinder-com/openapi/anymailfinder-com-verify-email-api-openapi.yml
consequence_counts:
  physical: 2
  read: 9
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Anymailfinder Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v5.1/bulk/json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v5.1/domain/{domain}/email/order
operation_count: 17
overview: 'Anymail Finder exposes 17 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 6 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Anymail Finder
provider_slug: anymailfinder-com
slug: anymailfinder-com-agentic-access
source_filename: anymailfinder-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/anymailfinder-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 9\n    acting: 8\n  by_consequence:\n    read: 9\n    physical: 2\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v5.1/account\n  method: get\n  operationId: account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5.1/domain/{domain}/email/download\n  method: get\n  operationId: download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v5.1/domain/{domain}/email/order\n  method: post\n  operationId: domainEmailOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5.1/domain/{domain}/email\n  method: get\n  operationId: domainEmailInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5.1/report/bad-email\n  method: post\n  operationId: badEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /v5.1/bulk/json\n  method: post\n  operationId: createWithJson\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5.1/bulk/multipart\n  method: post\n  operationId: createWithMultipart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5.1/bulk/{searchId}/download\n  method: get\n  operationId: download\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5.1/bulk/{searchId}\n\
  \  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5.1/find-email/company\n  method: post\n  operationId: company\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5.1/find-email/decision-maker\n  method: post\n  operationId: decisionMaker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5.1/find-email/linkedin-url\n  method: post\n  operationId: linkedinUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v5.1/find-email/person\n  method: post\n  operationId: person\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5.1/geo-lead\n  method: post\n  operationId: searchBulkGeoLeadCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5.1/geo-lead/{searchId}\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5.1/geo-lead/{searchId}/download\n  method: get\n  operationId: download\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v5.1/verify-email\n  method: post\n  operationId: validate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/anymailfinder-com/agentic-access/anymailfinder-com-agentic-access.yml
summary_line: 17 operations · 8 acting
tags:
- Email Finder
- B2B
- Lead Generation
- Verification
---
