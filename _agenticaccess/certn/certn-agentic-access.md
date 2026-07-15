---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: certn-openapi.yml
  format: yaml
  label: Certn Applications API
  slug: certn-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Checks API
  slug: certn-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Reports API
  slug: certn-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Packages API
  slug: certn-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Webhooks API
  slug: certn-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Teams and Users API
  slug: certn-teams-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
consequence_counts:
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Certn Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Certn exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Certn
provider_slug: certn
slug: certn-agentic-access
source_filename: certn-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/certn-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 6\n    connected: 8\n  by_consequence:\n    write: 6\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/hr/applications/invite/\n  method: post\n  operationId: inviteHrApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/hr/applications/quick/\n  method: post\n  operationId: quickScreenHrApplicant\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/hr/applicants/\n  method: get\n  operationId: listHrApplicants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hr/applicants/{applicant_id}/packages/\n  method: put\n  operationId: upgradeHrApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pm/applications/invite/\n  method: post\n  operationId: invitePmApplicant\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pm/applications/quick/\n  method: post\n  operationId: quickScreenPmApplicant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pm/applicants/\n  method: get\n  operationId: listPmApplicants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/{applicant_id}/\n  method: get\n  operationId: getApplicantReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/checks/\n  method: get\n  operationId: listAvailableChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/packages/\n  method: get\n  operationId: listPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/users/\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/teams/\n  method: get\n  operationId: listTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/teams/{team_id}/address/reference_templates/\n  method: get\n\
  \  operationId: getAddressReferenceTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/receiver\n  method: post\n  operationId: receiveWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/agentic-access/certn-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- Background Checks
- Identity Verification
- Criminal Record Check
- Screening
- HR Tech
- Compliance
- Trust and Safety
---
