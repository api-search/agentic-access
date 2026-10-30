---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: concord-com-webhooks-api-openapi.yml
  format: yaml
  label: Concord Webhooks (Outbound Events)
  slug: concord-com-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-webhooks-api-openapi.yml
- filename: concord-com-agreement-api-openapi.yml
  format: yaml
  label: Concord Agreement API
  slug: concord-com-agreement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-agreement-api-openapi.yml
- filename: concord-com-agreement-versions-api-openapi.yml
  format: yaml
  label: Concord Agreement Versions API
  slug: concord-com-agreement-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-agreement-versions-api-openapi.yml
- filename: concord-com-automated-template-api-openapi.yml
  format: yaml
  label: Concord Automated Template API
  slug: concord-com-automated-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-automated-template-api-openapi.yml
- filename: concord-com-clause-library-api-openapi.yml
  format: yaml
  label: Concord Clause Library API
  slug: concord-com-clause-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-clause-library-api-openapi.yml
- filename: concord-com-custom-branding-api-openapi.yml
  format: yaml
  label: Concord Custom Branding API
  slug: concord-com-custom-branding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-custom-branding-api-openapi.yml
- filename: concord-com-events-api-openapi.yml
  format: yaml
  label: Concord Events API
  slug: concord-com-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-events-api-openapi.yml
- filename: concord-com-folders-api-openapi.yml
  format: yaml
  label: Concord Folders API
  slug: concord-com-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-folders-api-openapi.yml
- filename: concord-com-organization-api-openapi.yml
  format: yaml
  label: Concord Organization API
  slug: concord-com-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-organization-api-openapi.yml
- filename: concord-com-organization-groups-api-openapi.yml
  format: yaml
  label: Concord Organization Groups API
  slug: concord-com-organization-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-organization-groups-api-openapi.yml
- filename: concord-com-organization-invitation-api-openapi.yml
  format: yaml
  label: Concord Organization invitation API
  slug: concord-com-organization-invitation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-organization-invitation-api-openapi.yml
- filename: concord-com-organization-members-api-openapi.yml
  format: yaml
  label: Concord Organization Members API
  slug: concord-com-organization-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-organization-members-api-openapi.yml
- filename: concord-com-report-api-openapi.yml
  format: yaml
  label: Concord Report API
  slug: concord-com-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-report-api-openapi.yml
- filename: concord-com-signature-api-openapi.yml
  format: yaml
  label: Concord Signature API
  slug: concord-com-signature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-signature-api-openapi.yml
- filename: concord-com-tags-api-openapi.yml
  format: yaml
  label: Concord Tags API
  slug: concord-com-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-tags-api-openapi.yml
- filename: concord-com-user-api-openapi.yml
  format: yaml
  label: Concord User API
  slug: concord-com-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-user-api-openapi.yml
- filename: concord-com-user-integrations-api-openapi.yml
  format: yaml
  label: Concord User integrations API
  slug: concord-com-user-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-user-integrations-api-openapi.yml
- filename: concord-com-webhooks-api-openapi.yml
  format: yaml
  label: Concord Webhooks API
  slug: concord-com-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-webhooks-api-openapi.yml
consequence_counts:
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Concord Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Concord exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Concord
provider_slug: concord-com
slug: concord-com-agentic-access
source_filename: concord-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/concord-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 8\n    acting: 1\n  by_consequence:\n    read: 8\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /user/me\n  method: get\n  operationId: getCurrentUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/me/organizations\n  method: get\n  operationId: listUserOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/me/organizations/{organizationId}/agreements\n\
  \  method: get\n  operationId: listAgreements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/agreements/{agreementUid}/attachments\n  method: get\n  operationId: listAgreementAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/agreements/{agreementUid}/members\n  method: get\n  operationId: listAgreementMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/reports\n  method: get\n  operationId: listOrganizationReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /organizations/{organizationId}/groups\n  method: get\n  operationId: listOrganizationGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/tags\n  method: get\n  operationId: listOrganizationTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}/templates/{templateUid}/documents\n  method: post\n  operationId: createDocumentFromTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/agentic-access/concord-com-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- Contract Management
- Contract Lifecycle Management
- Contracts
- Agreements
- E-Signature
- Document Management
- Legal
- Workflows
---
