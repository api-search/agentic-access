---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 4
api_specs:
- filename: allianz-docs-certificates-api-openapi.yml
  format: yaml
  label: Allianz Certificates API
  slug: allianz-docs-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/openapi/allianz-docs-certificates-api-openapi.yml
- filename: allianz-docs-leads-api-openapi.yml
  format: yaml
  label: Allianz Leads API
  slug: allianz-docs-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/openapi/allianz-docs-leads-api-openapi.yml
- filename: allianz-docs-policy-details-api-openapi.yml
  format: yaml
  label: Allianz Policy Details API
  slug: allianz-docs-policy-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/openapi/allianz-docs-policy-details-api-openapi.yml
- filename: allianz-docs-price-estimates-api-openapi.yml
  format: yaml
  label: Allianz Price Estimates API
  slug: allianz-docs-price-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/openapi/allianz-docs-price-estimates-api-openapi.yml
consequence_counts:
  physical: 1
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Allianz Docs Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /price-estimate/email
operation_count: 9
overview: 'Allianz exposes 9 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Allianz
provider_slug: allianz-docs
slug: allianz-docs-agentic-access
source_filename: allianz-docs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/allianz-docs-certificates-api-openapi.yml, openapi/allianz-docs-leads-api-openapi.yml,\n  openapi/allianz-docs-policy-details-api-openapi.yml, openapi/allianz-docs-price-estimates-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 4\n    acting: 5\n  by_consequence:\n    read: 4\n    write: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /certificates/{policy_number}\n  method: get\n  operationId: getCertificateOfCurrency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads\n  method: post\n  operationId:\
  \ createInstantLeadReferral\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy-details/assisted\n  method: post\n  operationId: getPolicyDetailsAssisted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy-details/self-service\n  method: post\n  operationId: createPolicyDetailsSelfService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /price-estimate/assisted\n  method: post\n  operationId: createPriceEstimateAssisted\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /price-estimate/email\n  method: post\n  operationId: sendPriceEstimateEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /price-estimate/self-service\n  method: post\n  operationId: createPriceEstimateSelfService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /price-estimate/{estimate_id}/summary\n  method: get\n  operationId: getPriceEstimateSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price-estimate/{estimate_id}/rating-factors\n  method: get\n  operationId: getPriceEstimateRatingFactors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/agentic-access/allianz-docs-agentic-access.yml
summary_line: 9 operations · 5 acting
tags:
- Financial Services
- Insurance
- Asset Management
---
