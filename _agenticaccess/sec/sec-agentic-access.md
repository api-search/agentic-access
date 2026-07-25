---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 11
api_specs:
- filename: sec-company-concept-api-openapi.yml
  format: yaml
  label: SEC EDGAR Company Concept API
  slug: sec-company-concept-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-company-concept-api-openapi.yml
- filename: sec-company-facts-api-openapi.yml
  format: yaml
  label: SEC EDGAR Company Facts API
  slug: sec-company-facts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-company-facts-api-openapi.yml
- filename: sec-edgar-operational-status-api-api-openapi.yml
  format: yaml
  label: SEC EDGAR EDGAR Operational Status API API
  slug: sec-edgar-operational-status-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-edgar-operational-status-api-api-openapi.yml
- filename: sec-filer-management-api-api-openapi.yml
  format: yaml
  label: SEC EDGAR Filer Management API API
  slug: sec-filer-management-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-filer-management-api-api-openapi.yml
- filename: sec-frames-api-openapi.yml
  format: yaml
  label: SEC EDGAR Frames API
  slug: sec-frames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-frames-api-openapi.yml
- filename: sec-search-api-openapi.yml
  format: yaml
  label: SEC EDGAR Search API
  slug: sec-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-search-api-openapi.yml
- filename: sec-submission-api-api-openapi.yml
  format: yaml
  label: SEC EDGAR Submission API API
  slug: sec-submission-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-submission-api-api-openapi.yml
- filename: sec-submission-status-api-api-openapi.yml
  format: yaml
  label: SEC EDGAR Submission Status API API
  slug: sec-submission-status-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-submission-status-api-api-openapi.yml
- filename: sec-submissions-api-openapi.yml
  format: yaml
  label: SEC EDGAR Submissions API
  slug: sec-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-submissions-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sec Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fm/{cik}/delegations
operation_count: 23
overview: 'SEC EDGAR exposes 23 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 11 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SEC EDGAR
provider_slug: sec
slug: sec-agentic-access
source_filename: sec-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sec-edgar-data-openapi.yml, openapi/sec-edgar-filer-openapi.yml, openapi/sec-edgar-full-text-search-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 11\n    acting: 12\n  by_consequence:\n    read: 11\n    write: 11\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /submissions/CIK{cik}.json\n  method: get\n  operationId: getCompanySubmissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/xbrl/companyfacts/CIK{cik}.json\n  method: get\n  operationId: getCompanyFacts\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/xbrl/companyconcept/CIK{cik}/{taxonomy}/{tag}.json\n  method: get\n  operationId: getCompanyConcept\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/xbrl/frames/{taxonomy}/{tag}/{unit}/{period}.json\n  method: get\n  operationId: getXBRLFrame\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fm/{cik}\n  method: get\n  operationId: View Filer Account Information\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fm/{cik}/ccc\n  method: post\n  operationId: Generate CCC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fm/{cik}/ccc\n  method: put\n  operationId: Create Custom CCC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fm/{cik}/delegationRequests\n  method: post\n  operationId: Request Delegation Invitations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fm/{cik}/delegations\n  method: post\n  operationId: Send Delegation\
  \ Invitations\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fm/{cik}/delegations\n  method: get\n  operationId: View Delegations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fm/{cik}/individuals\n  method: post\n  operationId: Add Individuals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fm/{cik}/individuals\n  method: get\n  operationId: View Individuals\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fm/{cik}/individuals\n  method: put\n  operationId: Change Roles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fm/{cik}/individuals\n  method: delete\n  operationId: Remove Individuals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fm/{cik}/verify\n  method: get\n  operationId: Filing Credentials Verification\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: EDGAR System Status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /submission/bulk/live\n  method: post\n  operationId: Bulk Live Submission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/bulk/test\n  method: post\n  operationId: Bulk Test Submission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /submission/single/live\n  method: post\n  operationId: Single Live Submission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/single/test\n  method: post\n  operationId: Single Test Submission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/status\n  method: post\n  operationId: Check Multiple Submission Statuses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submission/{accessionNumber}/status\n  method: get\n  operationId: Check Single Submission Status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /LATEST/search-index/efts\n  method: get\n  operationId: searchFilings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/agentic-access/sec-agentic-access.yml
summary_line: 23 operations · 12 acting
tags:
- Financial Data
- SEC
- EDGAR
- Public Company Filings
- XBRL
- Regulatory
- Government
- Financial Reporting
- Company Submissions
- Securities
---
