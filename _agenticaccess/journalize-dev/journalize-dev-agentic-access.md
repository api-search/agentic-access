---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 17
api_specs:
- filename: journalize-dev-accounts-api-openapi.yml
  format: yaml
  label: journalize-dev Accounts API
  slug: journalize-dev-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-accounts-api-openapi.yml
- filename: journalize-dev-export-api-openapi.yml
  format: yaml
  label: journalize-dev Export API
  slug: journalize-dev-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-export-api-openapi.yml
- filename: journalize-dev-health-api-openapi.yml
  format: yaml
  label: journalize-dev Health API
  slug: journalize-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-health-api-openapi.yml
- filename: journalize-dev-journal-api-openapi.yml
  format: yaml
  label: journalize-dev Journal API
  slug: journalize-dev-journal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-journal-api-openapi.yml
- filename: journalize-dev-journalize-api-openapi.yml
  format: yaml
  label: journalize-dev Journalize API
  slug: journalize-dev-journalize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-journalize-api-openapi.yml
- filename: journalize-dev-llms-txt-api-openapi.yml
  format: yaml
  label: journalize-dev Llms.txt API
  slug: journalize-dev-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-llms-txt-api-openapi.yml
- filename: journalize-dev-privacy-api-openapi.yml
  format: yaml
  label: journalize-dev Privacy API
  slug: journalize-dev-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-privacy-api-openapi.yml
- filename: journalize-dev-register-api-openapi.yml
  format: yaml
  label: journalize-dev Register API
  slug: journalize-dev-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-register-api-openapi.yml
- filename: journalize-dev-reports-api-openapi.yml
  format: yaml
  label: journalize-dev Reports API
  slug: journalize-dev-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-reports-api-openapi.yml
- filename: journalize-dev-robots-txt-api-openapi.yml
  format: yaml
  label: journalize-dev Robots.txt API
  slug: journalize-dev-robots-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-robots-txt-api-openapi.yml
- filename: journalize-dev-security-txt-api-openapi.yml
  format: yaml
  label: journalize-dev Security.txt API
  slug: journalize-dev-security-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-security-txt-api-openapi.yml
- filename: journalize-dev-skill-md-api-openapi.yml
  format: yaml
  label: journalize-dev SKILL.md API
  slug: journalize-dev-skill-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-skill-md-api-openapi.yml
- filename: journalize-dev-terms-api-openapi.yml
  format: yaml
  label: journalize-dev Terms API
  slug: journalize-dev-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-terms-api-openapi.yml
- filename: journalize-dev-well-known-api-openapi.yml
  format: yaml
  label: journalize-dev .well Known API
  slug: journalize-dev-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/journalize-dev/openapi/journalize-dev-well-known-api-openapi.yml
consequence_counts:
  read: 17
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Journalize Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 21
overview: 'journalize-dev exposes 21 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: journalize-dev
provider_slug: journalize-dev
slug: journalize-dev-agentic-access
source_filename: journalize-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/journalize-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 4\n    connected: 17\n  by_consequence:\n    write: 4\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /register\n  method: post\n  operationId: register_register_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journal/directives\n  method: post\n  operationId: submit_directive_journal_directives_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journal/directives\n  method: get\n  operationId: list_directives_journal_directives_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /journal/directives/validate\n  method: post\n  operationId: validate_directive_journal_directives_validate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /journal/directives/batch\n  method: post\n  operationId: submit_batch_journal_directives_batch_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: list_accounts_accounts_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/balance\n  method: get\n  operationId: get_account_balance_accounts_balance_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export\n  method: get\n  operationId: export_ledger_export_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/balance-sheet\n  method:\
  \ get\n  operationId: get_balance_sheet_reports_balance_sheet_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/income-statement\n  method: get\n  operationId: get_income_statement_reports_income_statement_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/trial-balance\n  method: get\n  operationId: get_trial_balance_reports_trial_balance_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: home__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /terms\n  method: get\n  operationId: terms_terms_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /privacy\n  method: get\n  operationId: privacy_privacy_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: llms_txt_llms_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SKILL.md\n  method: get\n  operationId: skill_md_SKILL_md_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /robots.txt\n  method: get\n  operationId: robots_txt_robots_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /.well-known/402index-verify.txt\n  method: get\n  operationId: index402_verify__well_known_402index_verify_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/security.txt\n  method: get\n  operationId: security_txt__well_known_security_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security.txt\n  method: get\n  operationId: security_txt_bare_security_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/journalize-dev/agentic-access/journalize-dev-agentic-access.yml
summary_line: 21 operations · 4 acting
tags:
- Company
- Accounting
- Artificial Intelligence
- Fintech
- Ledger
---
