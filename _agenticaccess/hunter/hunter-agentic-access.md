---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 14
api_specs:
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Domain Search API
  slug: domain-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Email Finder API
  slug: email-finder
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Email Verifier API
  slug: email-verifier
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Email Count API
  slug: email-count
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Account API
  slug: account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Discover API
  slug: discover
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Email Enrichment API
  slug: email-enrichment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Company Enrichment API
  slug: company-enrichment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Combined Enrichment API
  slug: combined-enrichment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Leads API
  slug: leads
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Leads Lists API
  slug: leads-lists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Campaigns API
  slug: campaigns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
- filename: hunter-api-openapi.yml
  format: yaml
  label: Hunter Logo API
  slug: logo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/openapi/hunter-api-openapi.yml
consequence_counts:
  read: 14
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hunter Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'Hunter exposes 25 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hunter
provider_slug: hunter
slug: hunter-agentic-access
source_filename: hunter-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hunter-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 14\n    acting: 11\n  by_consequence:\n    read: 14\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /domain-search\n  method: get\n  operationId: domainSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email-finder\n  method: get\n  operationId: emailFinder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email-verifier\n  method: get\n\
  \  operationId: emailVerifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email-count\n  method: get\n  operationId: emailCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads\n  method: get\n  operationId: listLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads\n  method: post\n  operationId: createLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads\n  method: put\n  operationId: upsertLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads/{id}\n  method: get\n  operationId: getLead\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads/{id}\n  method: put\n  operationId: updateLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /leads/{id}\n  method: delete\n  operationId: deleteLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads_lists\n  method: get\n  operationId: listLeadsLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads_lists\n  method: post\n  operationId: createLeadsList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads_lists/{id}\n  method: get\n  operationId: getLeadsList\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads_lists/{id}\n  method: put\n  operationId: updateLeadsList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads_lists/{id}\n  method: delete\n  operationId: deleteLeadsList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}/recipients\n  method: get\n  operationId: listCampaignRecipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns/{id}/recipients\n  method: post\n  operationId: addCampaignRecipients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{id}/recipients\n  method: delete\n  operationId: cancelCampaignRecipients\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /campaigns/{id}/start\n  method: post\n  operationId: startCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /discover\n  method: post\n  operationId: discover\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/find\n  method: get\n  operationId: emailEnrichment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/find\n  method: get\n  operationId: companyEnrichment\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /combined/find\n  method: get\n  operationId: combinedEnrichment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/agentic-access/hunter-agentic-access.yml
summary_line: 25 operations · 11 acting
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
---
