---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 13
api_specs:
- filename: recruitee-c-api-openapi.yml
  format: yaml
  label: Recruitee C API
  slug: recruitee-c-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recruitee/refs/heads/main/openapi/recruitee-c-api-openapi.yml
- filename: recruitee-i-api-openapi.yml
  format: yaml
  label: Recruitee I API
  slug: recruitee-i-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recruitee/refs/heads/main/openapi/recruitee-i-api-openapi.yml
- filename: recruitee-offers-api-openapi.yml
  format: yaml
  label: Recruitee Offers API
  slug: recruitee-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recruitee/refs/heads/main/openapi/recruitee-offers-api-openapi.yml
- filename: recruitee-p-api-openapi.yml
  format: yaml
  label: Recruitee P API
  slug: recruitee-p-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recruitee/refs/heads/main/openapi/recruitee-p-api-openapi.yml
consequence_counts:
  read: 13
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Recruitee Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 31
overview: 'Recruitee exposes 31 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Recruitee
provider_slug: recruitee
slug: recruitee-agentic-access
source_filename: recruitee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/recruitee-ats-api-openapi.yml, openapi/recruitee-careers-site-api-openapi.yml,\n  openapi/recruitee-partners-production-secret-openapi.yml, openapi/recruitee-partners-release-candidate-secret-openapi.yml,\n  openapi/recruitee-partners-release-candidate-token-openapi.yml, openapi/recruitee-private-api-staging-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    acting: 18\n    connected: 13\n  by_consequence:\n    write: 18\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /c/{company_id}/attachments\n  method: post\n  operationId: attachments-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /c/{company_id}/candidates\n  method: post\n  operationId: candidates-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /c/{company_id}/candidates\n  method: get\n  operationId: candidates-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /c/{company_id}/candidates/{id}\n  method: get\n  operationId: candidatesid-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /c/{company_id}/candidates/{id}\n  method: patch\n  operationId: candidatesid-patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /c/{company_id}/candidates/{id}\n  method: delete\n  operationId: candidatesid-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /c/{company_id}/candidates/{id}/notes\n  method: get\n  operationId: candidatesidnotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /c/{company_id}/candidates/{id}/update_cv\n  method: patch\n  operationId: candidatesidupdate_cv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /c/{company_id}/custom_fields/candidates/{id}/fields\n  method: post\n  operationId: custom_fieldscandidatesidfields-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /c/{company_id}/departments\n  method: get\n  operationId: departments-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /c/{company_id}/locations\n  method: get\n  operationId: locations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /c/{company_id}/offers\n  method: get\n  operationId: offers-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /c/{company_id}/offers\n  method: post\n  operationId: offersid-post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /c/{company_id}/offers/{id}\n  method: get\n  operationId: offersid-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /c/{company_id}/offers/{id}\n  method: patch\n  operationId: offersid-patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /c/{company_id}/offers/{id}\n  method: delete\n  operationId: offersid-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /c/{company_id}/search/new/candidates\n  method: get\n  operationId: searchnewcandidates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /offers/\n  method: get\n  operationId: offers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offers/{id}\n  method: get\n  operationId: offersid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offers/{offer_slug}/candidates\n  method: post\n  operationId: offersoffer_idcandidates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /p/{codename}/partner/regenerate-secret\n  method: post\n  operationId: post-partner-regenerate-secret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /p/{codename}/c/{company_id}/candidates/{candidate_id}/reports\n  method: get\n  operationId: get-candidate-reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /p/{codename}/c/{company_id}/reports\n  method: post\n  operationId: post-reports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /p/{codename}/reports/{report_id}\n  method: patch\n  operationId: patch-reports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /p/{codename}/reports/{report_id}\n  method: delete\n  operationId: delete-reports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /p/{codename}/c/{company_id}/partner\n  method: post\n  operationId: post-partner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /p/{codename}/c/{company_id}/partner\n  method: patch\n  operationId: patch-partner\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /p/{codename}/c/{company_id}/partner\n  method: get\n  operationId: get-partner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /p/{codename}/c/{company_id}/partner\n  method: delete\n  operationId: delete-partner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /i/p/{partner}/analytics\n  method: post\n  operationId: analytics\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /i/p/{partner}/timeline\n  method: get\n  operationId: timeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recruitee/refs/heads/main/agentic-access/recruitee-agentic-access.yml
summary_line: 31 operations · 18 acting
tags:
- Recruiting
- Applicant Tracking
- Human Resources
- Hiring
- Careers Site
- Tellent
---
