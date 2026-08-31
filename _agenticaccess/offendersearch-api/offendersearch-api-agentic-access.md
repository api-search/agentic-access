---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 18
api_specs:
- filename: offendersearch-api-account-api-openapi.yml
  format: yaml
  label: Offendersearch API Account API
  slug: offendersearch-api-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-account-api-openapi.yml
- filename: offendersearch-api-admin-api-openapi.yml
  format: yaml
  label: Offendersearch API Admin API
  slug: offendersearch-api-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-admin-api-openapi.yml
- filename: offendersearch-api-auth-api-openapi.yml
  format: yaml
  label: Offendersearch API Auth API
  slug: offendersearch-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-auth-api-openapi.yml
- filename: offendersearch-api-batch-api-openapi.yml
  format: yaml
  label: Offendersearch API Batch API
  slug: offendersearch-api-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-batch-api-openapi.yml
- filename: offendersearch-api-billing-api-openapi.yml
  format: yaml
  label: Offendersearch API Billing API
  slug: offendersearch-api-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-billing-api-openapi.yml
- filename: offendersearch-api-compat-api-openapi.yml
  format: yaml
  label: Offendersearch API Compat API
  slug: offendersearch-api-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-compat-api-openapi.yml
- filename: offendersearch-api-keys-api-openapi.yml
  format: yaml
  label: Offendersearch API Keys API
  slug: offendersearch-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-keys-api-openapi.yml
- filename: offendersearch-api-proof-docs-api-openapi.yml
  format: yaml
  label: Offendersearch API Proof Docs API
  slug: offendersearch-api-proof-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-proof-docs-api-openapi.yml
- filename: offendersearch-api-records-api-openapi.yml
  format: yaml
  label: Offendersearch API Records API
  slug: offendersearch-api-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-records-api-openapi.yml
- filename: offendersearch-api-report-api-openapi.yml
  format: yaml
  label: Offendersearch API Report API
  slug: offendersearch-api-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-report-api-openapi.yml
- filename: offendersearch-api-search-api-openapi.yml
  format: yaml
  label: Offendersearch API Search API
  slug: offendersearch-api-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-search-api-openapi.yml
- filename: offendersearch-api-searches-api-openapi.yml
  format: yaml
  label: Offendersearch API Searches API
  slug: offendersearch-api-searches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-searches-api-openapi.yml
- filename: offendersearch-api-sources-api-openapi.yml
  format: yaml
  label: Offendersearch API Sources API
  slug: offendersearch-api-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-sources-api-openapi.yml
- filename: offendersearch-api-support-api-openapi.yml
  format: yaml
  label: Offendersearch API Support API
  slug: offendersearch-api-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-support-api-openapi.yml
- filename: offendersearch-api-team-api-openapi.yml
  format: yaml
  label: Offendersearch API Team API
  slug: offendersearch-api-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-team-api-openapi.yml
- filename: offendersearch-api-usage-api-openapi.yml
  format: yaml
  label: Offendersearch API Usage API
  slug: offendersearch-api-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/openapi/offendersearch-api-usage-api-openapi.yml
consequence_counts:
  physical: 1
  read: 18
  safety-critical: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Offendersearch Api Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/keys/{keyId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/support
operation_count: 36
overview: 'Offendersearch API exposes 36 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 16 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Offendersearch API
provider_slug: offendersearch-api
slug: offendersearch-api-agentic-access
source_filename: offendersearch-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-18'\nmethod: generated\nsource: openapi/offendersearch-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 36\n  by_action_class:\n    acting: 18\n    connected: 18\n  by_consequence:\n    write: 16\n    read: 18\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/search\n  method: post\n  operationId: syncSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/searches\n  method: post\n  operationId: asyncSearch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/searches/{searchId}\n  method: get\n  operationId: getSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/searches/{searchId}/proof\n  method: post\n  operationId: makeProof\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/report\n  method: post\n  operationId: makeReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch\n  method: post\n  operationId: batchSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/proof-docs/{token}\n  method: get\n  operationId: getProofDoc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/records/{recordId}\n  method: get\n  operationId: getRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sources\n  method: get\n  operationId:\
  \ listSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/support\n  method: post\n  operationId: submitSupportMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/compat/sexoffender\n  method: post\n  operationId: compatSexoffenderPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/compat/sexoffender\n  method: get\n  operationId: compatSexoffenderGet\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/signup\n  method: post\n  operationId: signup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: get\n  operationId: listKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/{keyId}/rotate\n  method: post\n  operationId: rotateKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/{keyId}\n  method: delete\n  operationId: deleteKey\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/team\n  method: get\n  operationId: getTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/team\n  method: post\n  operationId: inviteMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/team/{memberId}\n  method: delete\n  operationId: removeMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing\n  method: get\n  operationId: getBilling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/accounts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/warm-queries\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/admin/warm-queries\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/warm\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/cache-stats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/scraper-health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/admin/scraper-runs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/ingest\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/ingest/rerun-failures\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /admin/ingest/status\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/freshness\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/ingest/report\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offendersearch-api/refs/heads/main/agentic-access/offendersearch-api-agentic-access.yml
summary_line: 36 operations · 18 acting · 1 human-in-the-loop
tags:
- background-checks
- Identity Verification
- public-records
- criminal-records
- Compliance
- trust-and-safety
- hr-tech
- recruiting
- proptech
- tenant-screening
- healthcare-screening
- data-api
- mcp-server
- agent-native
---
