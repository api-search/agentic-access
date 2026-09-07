---
acting_count: 2
action_class_counts:
  acting: 2
api_specs:
- filename: sofi-technologies-program-api-openapi.json
  format: json
  label: SoFi Tech Solutions Program API
  slug: sofi-tech-solutions-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-program-api-openapi.json
- filename: sofi-technologies-payment-hub-api-openapi.json
  format: json
  label: SoFi Tech Solutions Payment Hub API 2.0
  slug: sofi-tech-solutions-payment-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-payment-hub-api-openapi.json
- filename: sofi-technologies-dispute-api-3-0-openapi.json
  format: json
  label: SoFi Tech Solutions Dispute API 3.0
  slug: sofi-tech-solutions-dispute-api-30
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-dispute-api-3-0-openapi.json
- filename: sofi-technologies-dispute-api-2-0-openapi.json
  format: json
  label: SoFi Tech Solutions Dispute API 2.0
  slug: sofi-tech-solutions-dispute-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-dispute-api-2-0-openapi.json
- filename: sofi-technologies-loan-api-openapi.json
  format: json
  label: SoFi Tech Solutions Loan API
  slug: sofi-tech-solutions-loan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-loan-api-openapi.json
- filename: sofi-technologies-risk-api-2-0-openapi.json
  format: json
  label: SoFi Tech Solutions Risk API 2.0
  slug: sofi-tech-solutions-risk-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-risk-api-2-0-openapi.json
- filename: sofi-technologies-risk-api-1-0-openapi.json
  format: json
  label: SoFi Tech Solutions Risk API 1.0
  slug: sofi-tech-solutions-risk-api-10
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-risk-api-1-0-openapi.json
- filename: sofi-technologies-public-config-api-openapi.json
  format: json
  label: SoFi Tech Solutions Public Config API
  slug: sofi-tech-solutions-public-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-public-config-api-openapi.json
- filename: sofi-technologies-events-api-openapi.json
  format: json
  label: SoFi Tech Solutions Events API
  slug: sofi-tech-solutions-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-events-api-openapi.json
- filename: sofi-technologies-auth-api-openapi.json
  format: json
  label: SoFi Tech Solutions Auth API
  slug: sofi-tech-solutions-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-auth-api-openapi.json
- filename: sofi-technologies-external-trans-api-openapi.json
  format: json
  label: SoFi Tech Solutions External Trans API
  slug: sofi-tech-solutions-external-trans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-external-trans-api-openapi.json
consequence_counts:
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sofi Technologies Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 2
overview: 'SoFi Technologies exposes 2 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SoFi Technologies
provider_slug: sofi-technologies
slug: sofi-technologies-agentic-access
source_filename: sofi-technologies-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/sofi-home-loan-affiliate-lead-api-openapi.yml, openapi/sofi-partner-offer-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 2\n  by_consequence:\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /afpq/api/v1/affiliate/lead/home-loan\n  method: post\n  operationId: createHomeLoanLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /po/api/v2/loan-offer/json\n  method: post\n  operationId:\
  \ getLoanOffer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/agentic-access/sofi-technologies-agentic-access.yml
summary_line: 2 operations · 2 acting
tags:
- Fintech
- Payments
- Banking
- Card Issuing
- Banking as a Service
- Personal Finance
- Lending
- ACH
- ISO 20022
- Disputes
- Identity Verification
- Webhooks
---
