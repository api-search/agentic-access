---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 4
api_specs:
- filename: revenuebase-account-api-openapi.yml
  format: yaml
  label: RevenueBase Account API
  slug: revenuebase-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuebase/refs/heads/main/openapi/revenuebase-account-api-openapi.yml
- filename: revenuebase-email-api-openapi.yml
  format: yaml
  label: RevenueBase Email API
  slug: revenuebase-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuebase/refs/heads/main/openapi/revenuebase-email-api-openapi.yml
- filename: revenuebase-jobs-api-openapi.yml
  format: yaml
  label: RevenueBase Jobs API
  slug: revenuebase-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuebase/refs/heads/main/openapi/revenuebase-jobs-api-openapi.yml
- filename: revenuebase-organization-api-openapi.yml
  format: yaml
  label: RevenueBase Organization API
  slug: revenuebase-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuebase/refs/heads/main/openapi/revenuebase-organization-api-openapi.yml
- filename: revenuebase-contact-refresh-openapi.json
  format: json
  label: RevenueBase Contact Refresh API
  slug: revenuebase-contact-refresh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revenuebase/refs/heads/main/openapi/_original/revenuebase-contact-refresh-openapi.json
consequence_counts:
  read: 4
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Revenuebase Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'RevenueBase exposes 10 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RevenueBase
provider_slug: revenuebase
slug: revenuebase-agentic-access
source_filename: revenuebase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/revenuebase-account-api-openapi.yml, openapi/revenuebase-email-api-openapi.yml,\n  openapi/revenuebase-jobs-api-openapi.yml, openapi/revenuebase-organization-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 4\n    acting: 6\n  by_consequence:\n    read: 4\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/account/balance\n  method: get\n  operationId: get_usage_v2_account_balance_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/api-keys/rotate\n  method: post\n  operationId: rotate_api_key_v2_account_api_keys_rotate_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/email/verify\n  method: post\n  operationId: verify_email_v2_email_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/email/verify/batch\n  method: post\n  operationId: verify_email_batch_v2_email_verify_batch_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v2/jobs\n  method: get\n  operationId: list_jobs_v2_jobs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/jobs/{process_id}\n  method: get\n  operationId: get_job_v2_jobs__process_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/jobs/{process_id}/cancel\n  method: post\n  operationId: cancel_job_v2_jobs__process_id__cancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/jobs/{process_id}/download\n  method: get\n  operationId: download_job_v2_jobs__process_id__download_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/organization/resolve\n  method: post\n  operationId: resolve_company_v2_organization_resolve_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/organization/discover\n  method: post\n  operationId: discover_company_v2_organization_discover_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revenuebase/refs/heads/main/agentic-access/revenuebase-agentic-access.yml
summary_line: 10 operations · 6 acting
tags:
- Company
- B2B Data
- Data Enrichment
- Email Verification
- Contact Data
- Company Data
- Lead Intelligence
- Sales Intelligence
---
