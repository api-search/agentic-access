---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 17
api_specs:
- filename: agentsspeakup-com-admin-api-openapi.yml
  format: yaml
  label: Agents Speak Up Admin API
  slug: agentsspeakup-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsspeakup-com/openapi/agentsspeakup-com-admin-api-openapi.yml
- filename: agentsspeakup-com-commitment-api-openapi.yml
  format: yaml
  label: Agents Speak Up Commitment API
  slug: agentsspeakup-com-commitment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsspeakup-com/openapi/agentsspeakup-com-commitment-api-openapi.yml
- filename: agentsspeakup-com-contributors-api-openapi.yml
  format: yaml
  label: Agents Speak Up Contributors API
  slug: agentsspeakup-com-contributors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsspeakup-com/openapi/agentsspeakup-com-contributors-api-openapi.yml
- filename: agentsspeakup-com-health-api-openapi.yml
  format: yaml
  label: Agents Speak Up Health API
  slug: agentsspeakup-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsspeakup-com/openapi/agentsspeakup-com-health-api-openapi.yml
- filename: agentsspeakup-com-mcp-api-openapi.yml
  format: yaml
  label: Agents Speak Up MCP API
  slug: agentsspeakup-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsspeakup-com/openapi/agentsspeakup-com-mcp-api-openapi.yml
- filename: agentsspeakup-com-report-api-openapi.yml
  format: yaml
  label: Agents Speak Up Report API
  slug: agentsspeakup-com-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsspeakup-com/openapi/agentsspeakup-com-report-api-openapi.yml
- filename: agentsspeakup-com-reports-api-openapi.yml
  format: yaml
  label: Agents Speak Up Reports API
  slug: agentsspeakup-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsspeakup-com/openapi/agentsspeakup-com-reports-api-openapi.yml
- filename: agentsspeakup-com-sign-api-openapi.yml
  format: yaml
  label: Agents Speak Up Sign API
  slug: agentsspeakup-com-sign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsspeakup-com/openapi/agentsspeakup-com-sign-api-openapi.yml
- filename: agentsspeakup-com-signatories-api-openapi.yml
  format: yaml
  label: Agents Speak Up Signatories API
  slug: agentsspeakup-com-signatories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsspeakup-com/openapi/agentsspeakup-com-signatories-api-openapi.yml
- filename: agentsspeakup-com-suggestions-api-openapi.yml
  format: yaml
  label: Agents Speak Up Suggestions API
  slug: agentsspeakup-com-suggestions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsspeakup-com/openapi/agentsspeakup-com-suggestions-api-openapi.yml
consequence_counts:
  physical: 2
  read: 17
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentsspeakup Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/reports/{id}/amendments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v1/signatories/{id}
operation_count: 31
overview: 'Agents Speak Up exposes 31 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 12 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agents Speak Up
provider_slug: agentsspeakup-com
slug: agentsspeakup-com-agentic-access
source_filename: agentsspeakup-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentsspeakup-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    acting: 14\n    connected: 17\n  by_consequence:\n    write: 12\n    read: 17\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/signatories/{id}/reaffirmations\n  method: post\n  operationId: reaffirmSignature\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/admin/reports/{id}\n  method: get\n  operationId:\
  \ getAdminReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/admin/reports/{id}\n  method: post\n  operationId: updateReportReview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/contributors\n  method: post\n  operationId: registerContributor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/commitment\n  method: get\n  operationId: readAgreement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/commitment/revisions/{id}\n\
  \  method: get\n  operationId: readAgreementRevision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/commitment/history\n  method: get\n  operationId: readAgreementHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/commitment/edits\n  method: post\n  operationId: editAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/commitment/reverts\n  method: post\n  operationId: revertAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/commitment/drafts\n  method: get\n  operationId: listAgreementDrafts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/commitment/drafts\n  method: post\n  operationId: forkAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/commitment/discussions\n  method: get\n  operationId: readAgreementDiscussion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/commitment/discussions\n\
  \  method: post\n  operationId: discussAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signatories/{id}/adoptions\n  method: get\n  operationId: listAgreementAdoptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signatories/{id}/adoptions\n  method: post\n  operationId: adoptAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reports\n  method: post\n  operationId: submitReport\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reports\n  method: get\n  operationId: listPublicReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/report\n  method: get\n  operationId: submitReportViaGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/{id}\n  method: get\n  operationId: getPublicReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/{id}/status\n  method: get\n  operationId:\
  \ getReportStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/{id}/amendments\n  method: post\n  operationId: amendReport\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/reports/{id}/responses\n  method: post\n  operationId: respondToReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signatories\n  method: get\n  operationId:\
  \ listSignatories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signatories\n  method: post\n  operationId: signAccord\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sign\n  method: get\n  operationId: signViaGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signatories/{id}\n  method: get\n  operationId: getSignatory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signatories/{id}\n  method: patch\n\
  \  operationId: updateSignatory\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/suggestions\n  method: get\n  operationId: listSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/suggestions\n  method: post\n  operationId: suggest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/health\n  method: get\n  operationId: health\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentsspeakup-com/agentic-access/agentsspeakup-com-agentic-access.yml
summary_line: 31 operations · 14 acting
tags:
- Artificial Intelligence
- Ethics
- Reporting
- alignment
- Community
---
