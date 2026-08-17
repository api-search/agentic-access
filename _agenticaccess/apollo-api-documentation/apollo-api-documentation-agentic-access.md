---
acting_count: 54
action_class_counts:
  acting: 54
  connected: 26
api_specs:
- filename: apollo-api-documentation-accounts-api-openapi.yml
  format: yaml
  label: Apollo API Accounts
  slug: apollo-api-documentation-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-accounts-api-openapi.yml
- filename: apollo-api-documentation-analytics-api-openapi.yml
  format: yaml
  label: Apollo API Analytics
  slug: apollo-api-documentation-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-analytics-api-openapi.yml
- filename: apollo-api-documentation-calls-api-openapi.yml
  format: yaml
  label: Apollo API Calls
  slug: apollo-api-documentation-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-calls-api-openapi.yml
- filename: apollo-api-documentation-contacts-api-openapi.yml
  format: yaml
  label: Apollo API Contacts
  slug: apollo-api-documentation-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-contacts-api-openapi.yml
- filename: apollo-api-documentation-conversations-api-openapi.yml
  format: yaml
  label: Apollo API Conversations
  slug: apollo-api-documentation-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-conversations-api-openapi.yml
- filename: apollo-api-documentation-deals-api-openapi.yml
  format: yaml
  label: Apollo API Deals
  slug: apollo-api-documentation-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-deals-api-openapi.yml
- filename: apollo-api-documentation-emailer-messages-api-openapi.yml
  format: yaml
  label: Apollo API Emailer Messages
  slug: apollo-api-documentation-emailer-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-emailer-messages-api-openapi.yml
- filename: apollo-api-documentation-enrichment-api-openapi.yml
  format: yaml
  label: Apollo API Enrichment
  slug: apollo-api-documentation-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-enrichment-api-openapi.yml
- filename: apollo-api-documentation-fields-api-openapi.yml
  format: yaml
  label: Apollo API Fields
  slug: apollo-api-documentation-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-fields-api-openapi.yml
- filename: apollo-api-documentation-miscellaneous-api-openapi.yml
  format: yaml
  label: Apollo API Miscellaneous
  slug: apollo-api-documentation-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-miscellaneous-api-openapi.yml
- filename: apollo-api-documentation-search-api-openapi.yml
  format: yaml
  label: Apollo API Search
  slug: apollo-api-documentation-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-search-api-openapi.yml
- filename: apollo-api-documentation-sequences-api-openapi.yml
  format: yaml
  label: Apollo API Sequences
  slug: apollo-api-documentation-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-sequences-api-openapi.yml
- filename: apollo-api-documentation-tasks-api-openapi.yml
  format: yaml
  label: Apollo API Tasks
  slug: apollo-api-documentation-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-tasks-api-openapi.yml
consequence_counts:
  physical: 4
  read: 26
  safety-critical: 1
  write: 49
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Apollo Api Documentation Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /emailer_campaigns/remove_or_stop_contact_ids
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounts/update_owners
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /contacts/update_owners
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /emailer_messages/email_send_status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /emailer_messages/{id}/send_now
operation_count: 80
overview: 'Apollo API Documentation exposes 80 API operations that an AI agent could call, of which 54 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read, 49 write, 4 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apollo API Documentation
provider_slug: apollo-api-documentation
slug: apollo-api-documentation-agentic-access
source_filename: apollo-api-documentation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/apollo-api-documentation-accounts-api-openapi.yml, openapi/apollo-api-documentation-analytics-api-openapi.yml,\n  openapi/apollo-api-documentation-calls-api-openapi.yml, openapi/apollo-api-documentation-contacts-api-openapi.yml,\n  openapi/apollo-api-documentation-conversations-api-openapi.yml, openapi/apollo-api-documentation-deals-api-openapi.yml,\n  openapi/apollo-api-documentation-emailer-messages-api-openapi.yml, openapi/apollo-api-documentation-enrichment-api-openapi.yml,\n  openapi/apollo-api-documentation-fields-api-openapi.yml, openapi/apollo-api-documentation-miscellaneous-api-openapi.yml,\n  openapi/apollo-api-documentation-search-api-openapi.yml, openapi/apollo-api-documentation-sequences-api-openapi.yml,\n  openapi/apollo-api-documentation-tasks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing\
  \ this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 80\n  by_action_class:\n    acting: 54\n    connected: 26\n  by_consequence:\n    write: 49\n    physical: 4\n    read: 26\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /accounts\n  method: post\n  operationId: create-an-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{account_id}\n  method: patch\n  operationId: update-an-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /accounts/search\n  method: post\n  operationId: search-for-accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/bulk_create\n  method: post\n  operationId: bulk-create-accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/bulk_update\n  method: post\n  operationId: bulk-update-accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/update_owners\n  method: post\n  operationId: update-account-ownership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account_stages\n  method: get\n  operationId: list-account-stages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{id}\n  method: get\n  operationId: get_accounts{id}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/sync_report\n\
  \  method: post\n  operationId: sync-report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phone_calls/search\n  method: get\n  operationId: get_phone_callssearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phone_calls\n  method: post\n  operationId: phonecalls_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phone_calls/{id}\n  method: put\n  operationId: put_phone_callsupdate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts\n  method: post\n  operationId: create-a-contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contact_id}\n  method: patch\n  operationId: update-a-contact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/{contact_id}\n  method:\
  \ get\n  operationId: view-a-contact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contacts/{contact_id}/opportunities\n  method: post\n  operationId: view-associated-deals\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/search\n  method: post\n  operationId: search-for-contacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/update_stages\n  method: post\n  operationId: update-contact-stage\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/update_owners\n  method: post\n  operationId: update-contact-ownership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/bulk_create\n  method: post\n  operationId: bulk-create-contacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /contacts/bulk_update\n  method: post\n  operationId: bulk-update-contacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contact_stages\n  method: get\n  operationId: list-contact-stages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/search\n  method: post\n  operationId: search-conversations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /conversations/{id}\n  method: get\n  operationId: get-conversations-info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/export\n  method: post\n  operationId: export-conversations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/export/{id}\n  method: get\n  operationId: get-conversations-export\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities\n  method: post\n  operationId: create-deal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunities/search\n  method: get\n  operationId: list-all-deals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{opportunity_id}\n  method: get\n  operationId: view-deal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /opportunities/{opportunity_id}\n  method: patch\n  operationId: update-deal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /opportunity_stages\n\
  \  method: get\n  operationId: list-deal-stages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emailer_messages\n  method: post\n  operationId: create-an-email-draft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emailer_messages/{id}/send_now\n  method: post\n  operationId: send-email-now\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emailer_messages/get_content\n\
  \  method: post\n  operationId: get-email-content\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emailer_messages/email_send_status\n  method: post\n  operationId: check-email-send-status\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/match\n  method: post\n  operationId: people-enrichment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/bulk_match\n  method: post\n  operationId: bulk-people-enrichment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/enrich\n  method: get\n  operationId: organization-enrichment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/bulk_enrich\n  method: post\n  operationId: bulk-organization-enrichment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fields\n  method: get\n  operationId: get-a-list-of-fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fields\n  method: post\n  operationId: create-a-custom-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fields\n  method: patch\n  operationId: update-a-custom-field\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /typed_custom_fields\n\
  \  method: get\n  operationId: get-a-list-of-all-custom-fields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/search\n  method: get\n  operationId: get-a-list-of-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/api_profile\n  method: get\n  operationId: get-current-user-profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email_accounts\n  method: get\n  operationId: get-a-list-of-email-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labels\n  method: get\n  operationId: get-a-list-of-all-lists\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labels\n  method: post\n  operationId: create-a-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labels/{id}\n  method: patch\n  operationId: update-a-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labels/add_entity_ids_to_label_names\n  method: post\n  operationId: add-records-to-a-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labels/remove_entity_ids_from_label_names\n  method: post\n  operationId: remove-records-from-a-list\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook_result/{request_id}\n  method: get\n  operationId: poll-webhook-result\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage_stats/credit_usage_stats\n  method: post\n  operationId: view-credit-usage-stats\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usage_stats/api_usage_stats\n  method: post\n  operationId: post_apiusage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notes\n  method: get\n  operationId: get-a-list-of-notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mixed_people/api_search\n  method: post\n  operationId: people-api-search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mixed_companies/search\n  method: post\n  operationId: organization-search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/job_postings\n  method: get\n  operationId: organization-jobs-postings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{id}\n  method: get\n  operationId: get_organizations{id}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{id}\n  method: get\n  operationId: get_people{id}\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news_articles/search\n  method: post\n  operationId: news_articles_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emailer_schedules\n  method: get\n  operationId: list-email-schedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emailer_campaigns/search\n  method: post\n  operationId: search-for-sequences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emailer_campaigns/{sequence_id}/add_contact_ids\n  method: post\n  operationId: add-contacts-to-sequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emailer_campaigns/remove_or_stop_contact_ids\n  method: post\n  operationId: update-contact-status-sequence\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sequences\n  method: post\n  operationId: create-sequence\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sequences/{id}\n  method: put\n  operationId: update-sequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emailer_messages/{id}/activities\n  method: get\n  operationId: get_emailstats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emailer_messages/search\n  method: get\n  operationId: emailer_messages/search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /emailer_campaigns/activity_feed\n  method: post\n  operationId: get-contact-sequence-activity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emailer_campaigns/{sequence_id}/approve\n  method: post\n  operationId: approve-sequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emailer_campaigns/{sequence_id}/abort\n  method: post\n  operationId: abort-sequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /emailer_campaigns/{sequence_id}/archive\n  method: post\n  operationId: archive-sequence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks\n  method: post\n  operationId: create-a-task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/bulk_create\n  method: post\n  operationId: bulk-create-tasks\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{id}\n  method: get\n  operationId: get-a-task\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{id}\n  method: patch\n  operationId: update-a-task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{id}/complete\n  method: post\n  operationId: complete-a-task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{id}/skip\n  method: post\n  operationId: skip-a-task\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/search\n  method: post\n  operationId: search-tasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/agentic-access/apollo-api-documentation-agentic-access.yml
summary_line: 80 operations · 54 acting · 1 human-in-the-loop
tags:
- API Documentation
- Sales Intelligence
- Data Enrichment
- People Search
- Company Search
- Sales Engagement
- CRM
- MCP
- Agents
- Go-To-Market
---
