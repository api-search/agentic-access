---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 15
api_specs:
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Authentication API
  slug: snov-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Email Finder API
  slug: snov-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Domain Search API
  slug: snov-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Email Verifier API
  slug: snov-email-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Enrichment API
  slug: snov-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Prospects & Lists API
  slug: snov-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Drip Campaigns API
  slug: snov-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Sender Accounts API
  slug: snov-sender-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Email Warm-up API
  slug: snov-warmup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io User & Balance API
  slug: snov-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
consequence_counts:
  physical: 2
  read: 15
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Snov Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/sender-accounts/emails
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/sender-accounts/emails/{id}
operation_count: 37
overview: 'Snov.io exposes 37 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 20 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Snov.io
provider_slug: snov
slug: snov-agentic-access
source_filename: snov-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/snov-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    acting: 22\n    connected: 15\n  by_consequence:\n    write: 20\n    read: 15\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/oauth/access_token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/emails-by-domain-by-name/start\n  method: post\n  operationId: startEmailsByDomainByName\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/emails-by-domain-by-name/result\n  method: get\n  operationId: getEmailsByDomainByNameResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/company-domain-by-name/start\n  method: post\n  operationId: startCompanyDomainByName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/company-domain-by-name/result\n  method: get\n  operationId: getCompanyDomainByNameResult\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/domain-search/start\n  method: post\n  operationId: startDomainSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/domain-search/result/{task_hash}\n  method: get\n  operationId: getDomainSearchResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/domain-search/prospects/start\n  method: post\n  operationId: startDomainProspects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/domain-search/prospects/result/{task_hash}\n  method: get\n  operationId: getDomainProspectsResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/domain-search/domain-emails/start\n  method: post\n  operationId: startDomainEmails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/domain-search/domain-emails/result/{task_hash}\n  method: get\n  operationId: getDomainEmailsResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v2/domain-search/generic-contacts/start\n  method: post\n  operationId: startGenericContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/domain-search/generic-contacts/result/{task_hash}\n  method: get\n  operationId: getGenericContactsResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get-domain-emails-count\n  method: post\n  operationId: getDomainEmailsCount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/email-verification/start\n  method: post\n  operationId: startEmailVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/email-verification/result\n  method: get\n  operationId: getEmailVerificationResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get-profile-by-email\n  method: post\n  operationId: getProfileByEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v2/li-profiles-by-urls/start\n  method: post\n  operationId: startLiProfilesByUrls\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/li-profiles-by-urls/result\n  method: get\n  operationId: getLiProfilesByUrlsResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get-user-lists\n  method: get\n  operationId: getUserLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lists\n  method: post\n  operationId: createList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/prospect-list\n  method: post\n  operationId: getProspectList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/add-prospect-to-list\n  method: post\n  operationId: addProspectToList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/get-user-campaigns\n  method: get\n  operationId: getUserCampaigns\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/get-emails-sent\n  method: post\n  operationId: getEmailsSent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/get-emails-opened\n  method: post\n  operationId: getEmailsOpened\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/get-emails-clicked\n  method: post\n  operationId: getEmailsClicked\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/get-emails-replies\n  method: post\n  operationId: getEmailsReplies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sender-accounts/emails\n  method: get\n  operationId: listSenderAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/sender-accounts/emails\n  method: post\n  operationId: createSenderAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sender-accounts/emails/{id}\n  method: patch\n  operationId: updateSenderAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sender-accounts/check-sender-status\n  method: get\n  operationId: checkSenderStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warm-up\n  method: get\n  operationId: listWarmUpCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warm-up\n  method: post\n  operationId: createWarmUpCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/warm-up/{id}\n  method: get\n  operationId: getWarmUpCampaign\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/warm-up/{id}\n  method: patch\n  operationId: updateWarmUpCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/get-balance\n\
  \  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/agentic-access/snov-agentic-access.yml
summary_line: 37 operations · 22 acting
tags:
- Sales Engagement
- Email Finder
- Email Verification
- Prospecting
- Drip Campaigns
- CRM
- Lead Generation
---
