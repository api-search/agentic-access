---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 7
api_specs:
- filename: apollo-io-accounts-api-openapi.yml
  format: yaml
  label: Apollo.io Accounts API
  slug: apollo-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-accounts-api-openapi.yml
- filename: apollo-io-contacts-api-openapi.yml
  format: yaml
  label: Apollo.io Contacts API
  slug: apollo-io-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-contacts-api-openapi.yml
- filename: apollo-io-email-accounts-api-openapi.yml
  format: yaml
  label: Apollo.io Email Accounts API
  slug: apollo-io-email-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-email-accounts-api-openapi.yml
- filename: apollo-io-emailer-campaigns-api-openapi.yml
  format: yaml
  label: Apollo.io Emailer Campaigns API
  slug: apollo-io-emailer-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-emailer-campaigns-api-openapi.yml
- filename: apollo-io-mixed-companies-api-openapi.yml
  format: yaml
  label: Apollo.io Mixed Companies API
  slug: apollo-io-mixed-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-mixed-companies-api-openapi.yml
- filename: apollo-io-mixed-people-api-openapi.yml
  format: yaml
  label: Apollo.io Mixed People API
  slug: apollo-io-mixed-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-mixed-people-api-openapi.yml
- filename: apollo-io-opportunities-api-openapi.yml
  format: yaml
  label: Apollo.io Opportunities API
  slug: apollo-io-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-opportunities-api-openapi.yml
- filename: apollo-io-organizations-api-openapi.yml
  format: yaml
  label: Apollo.io Organizations API
  slug: apollo-io-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-organizations-api-openapi.yml
- filename: apollo-io-people-api-openapi.yml
  format: yaml
  label: Apollo.io People API
  slug: apollo-io-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-people-api-openapi.yml
- filename: apollo-io-phone-calls-api-openapi.yml
  format: yaml
  label: Apollo.io Phone Calls API
  slug: apollo-io-phone-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-phone-calls-api-openapi.yml
- filename: apollo-io-sync-report-api-openapi.yml
  format: yaml
  label: Apollo.io Sync Report API
  slug: apollo-io-sync-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-sync-report-api-openapi.yml
- filename: apollo-io-tasks-api-openapi.yml
  format: yaml
  label: Apollo.io Tasks API
  slug: apollo-io-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-tasks-api-openapi.yml
- filename: apollo-io-usage-stats-api-openapi.yml
  format: yaml
  label: Apollo.io Usage Stats API
  slug: apollo-io-usage-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-usage-stats-api-openapi.yml
- filename: apollo-io-users-api-openapi.yml
  format: yaml
  label: Apollo.io Users API
  slug: apollo-io-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-users-api-openapi.yml
consequence_counts:
  read: 7
  write: 21
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apollo Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 28
overview: 'Apollo.io exposes 28 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 21 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apollo.io
provider_slug: apollo-io
slug: apollo-io-agentic-access
source_filename: apollo-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/apollo-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 21\n    connected: 7\n  by_consequence:\n    write: 21\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /people/match\n  method: post\n  operationId: peopleEnrichment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/bulk_match\n  method: post\n  operationId: bulkPeopleEnrichment\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/enrich\n  method: get\n  operationId: organizationEnrichment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mixed_people/search\n  method: post\n  operationId: peopleSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mixed_companies/search\n  method: post\n  operationId: organizationSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/job_postings\n  method: get\n  operationId: organizationJobPostings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}\n  method: patch\n  operationId: updateAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/bulk_create\n  method: post\n  operationId: bulkCreateAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{id}\n  method: patch\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/bulk_create\n  method: post\n  operationId: bulkCreateContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities\n  method: post\n  operationId: createDeal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities/search\n  method: get\n  operationId: listDeals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{id}\n  method: get\n  operationId: viewDeal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emailer_campaigns/search\n  method: post\n  operationId: searchSequences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emailer_campaigns/{id}/add_contact_ids\n  method: post\n  operationId: addContactsToSequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /emailer_campaigns/{id}/update_contact_status\n  method: post\n  operationId: updateContactStatusInSequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks\n  method: post\n  operationId: createTask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/bulk_create\n  method: post\n  operationId: bulkCreateTasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/search\n  method: post\n  operationId: searchTasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usage_stats/api_usage_stats\n  method: post\n  operationId: viewApiUsageStats\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phone_calls\n  method: post\n  operationId: createCallRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phone_calls/search\n  method: get\n  operationId: searchCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phone_calls/{id}\n  method: put\n  operationId: updateCallRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/search\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email_accounts\n  method: get\n  operationId: listEmailAccounts\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sync_report\n  method: post\n  operationId: syncReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/agentic-access/apollo-io-agentic-access.yml
summary_line: 28 operations · 21 acting
tags:
- Sales Intelligence
- Prospecting
- Engagement
- B2B Data
- Enrichment
- SaaS
---
