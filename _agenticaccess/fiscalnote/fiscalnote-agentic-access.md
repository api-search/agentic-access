---
acting_count: 0
action_class_counts:
  connected: 26
api_specs:
- filename: fiscalnote-policynote-openapi.yml
  format: yaml
  label: FiscalNote PolicyNote API
  slug: policynote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-policynote-openapi.yml
- filename: fiscalnote-appdata-openapi.yml
  format: yaml
  label: FiscalNote AppData API
  slug: appdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-appdata-openapi.yml
- filename: fiscalnote-people-openapi.yml
  format: yaml
  label: FiscalNote People API
  slug: people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-people-openapi.yml
- filename: fiscalnote-organization-openapi.yml
  format: yaml
  label: FiscalNote Organization API
  slug: organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-organization-openapi.yml
consequence_counts:
  read: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fiscalnote Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'FiscalNote exposes 26 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FiscalNote
provider_slug: fiscalnote
slug: fiscalnote-agentic-access
source_filename: fiscalnote-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fiscalnote-appdata-openapi.yml, openapi/fiscalnote-organization-openapi.yml,\n  openapi/fiscalnote-people-openapi.yml, openapi/fiscalnote-policynote-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    connected: 26\n  by_consequence:\n    read: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /appdata/v1/bills\n  method: get\n  operationId: listBills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appdata/v1/bills/{billId}\n  method: get\n  operationId: getBill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appdata/v1/issues\n  method: get\n  operationId: listIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appdata/v1/issues/{issueId}\n  method: get\n  operationId: getIssue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appdata/v1/labels\n  method: get\n  operationId: listLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appdata/v1/labels/{labelId}\n  method: get\n  operationId: getLabel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appdata/v1/regulatory-documents\n  method:\
  \ get\n  operationId: listRegulatoryDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appdata/v1/regulatory-documents/{documentId}\n  method: get\n  operationId: getRegulatoryDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/v1/organizations\n  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/v1/organizations/{organizationId}\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/v1/committees\n  method: get\n  operationId: listCommittees\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/v1/committees/{committeeId}\n  method: get\n  operationId: getCommittee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/v1/committees/{committeeId}/members\n  method: get\n  operationId: listCommitteeMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/v2/officials\n  method: get\n  operationId: listOfficials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/v2/officials/{officialId}\n  method: get\n  operationId: getOfficial\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/v2/legislators\n  method: get\n  operationId: listLegislators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/v2/legislators/{legislatorId}\n  method: get\n  operationId: getLegislator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/v2/legislators/{legislatorId}/votes\n  method: get\n  operationId: listLegislatorVotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policynote/v1/legislation\n  method: get\n  operationId: listLegislation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /policynote/v1/legislation/{legislationId}\n  method: get\n  operationId: getLegislation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policynote/v1/regulations\n  method: get\n  operationId: listRegulations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policynote/v1/regulations/{regulationId}\n  method: get\n  operationId: getRegulation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policynote/v1/stakeholders\n  method: get\n  operationId: listStakeholders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policynote/v1/transcripts\n\
  \  method: get\n  operationId: listPresidentialTranscripts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policynote/v1/transcripts/{transcriptId}\n  method: get\n  operationId: getPresidentialTranscript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policynote/v1/intelligence/impact\n  method: get\n  operationId: listPolicyImpactSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/agentic-access/fiscalnote-agentic-access.yml
summary_line: 26 operations
tags:
- Government
- Legislation
- Policy
- Political Intelligence
- Regulation
---
