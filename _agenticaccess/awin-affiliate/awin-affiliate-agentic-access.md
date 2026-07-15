---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Accounts API
  slug: awin-affiliate-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Transactions API
  slug: awin-affiliate-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Reports API
  slug: awin-affiliate-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Commission Groups API
  slug: awin-affiliate-commission-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Programmes API
  slug: awin-affiliate-programmes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Awin Affiliate Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Awin exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Awin
provider_slug: awin-affiliate
slug: awin-affiliate-agentic-access
source_filename: awin-affiliate-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/awin-affiliate-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publishers/{publisherId}/transactions/\n  method: get\n  operationId: getPublisherTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /advertisers/{advertiserId}/transactions/\n\
  \  method: get\n  operationId: getAdvertiserTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publishers/{publisherId}/reports/advertiser\n  method: get\n  operationId: getPublisherAdvertiserReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publishers/{publisherId}/reports/creative\n  method: get\n  operationId: getPublisherCreativeReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publishers/{publisherId}/reports/campaign\n  method: get\n  operationId: getPublisherCampaignReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /advertisers/{advertiserId}/reports/publisher\n\
  \  method: get\n  operationId: getAdvertiserPublisherReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /advertisers/{advertiserId}/reports/creative\n  method: get\n  operationId: getAdvertiserCreativeReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /advertisers/{advertiserId}/reports/campaign\n  method: get\n  operationId: getAdvertiserCampaignReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publishers/{publisherId}/commissiongroups\n  method: get\n  operationId: getCommissionGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publishers/{publisherId}/programmes\n\
  \  method: get\n  operationId: getProgrammes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publishers/{publisherId}/programmedetails\n  method: get\n  operationId: getProgrammeDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/agentic-access/awin-affiliate-agentic-access.yml
summary_line: 12 operations
tags:
- Affiliate Marketing
- Advertising
- Publishers
- Advertisers
- Transactions
- Reporting
- Commissions
- Performance Marketing
---
