---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 9
api_specs:
- filename: credly-openapi.yml
  format: yaml
  label: Credly Badge Templates API
  slug: credly-badge-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
- filename: credly-openapi.yml
  format: yaml
  label: Credly Issued Badges API
  slug: credly-issued-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
- filename: credly-openapi.yml
  format: yaml
  label: Credly Organizations API
  slug: credly-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
- filename: credly-openapi.yml
  format: yaml
  label: Credly Events and Webhooks API
  slug: credly-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
- filename: credly-openapi.yml
  format: yaml
  label: Credly OBI Recipients API
  slug: credly-obi-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
consequence_counts:
  read: 9
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Credly Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /organizations/{organization_id}/badges/{id}/revoke
operation_count: 15
overview: 'Credly exposes 15 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 5 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Credly
provider_slug: credly
slug: credly-agentic-access
source_filename: credly-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/credly-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 9\n    acting: 6\n  by_consequence:\n    read: 9\n    write: 5\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /organizations/{organization_id}/badge_templates\n  method: get\n  operationId: listBadgeTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/badge_templates\n  method: post\n  operationId: createBadgeTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/badge_templates/{id}\n  method: get\n  operationId: getBadgeTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/badge_templates/{id}\n  method: put\n  operationId: updateBadgeTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/badge_templates/{id}\n  method: delete\n  operationId: deleteBadgeTemplate\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/badges\n  method: get\n  operationId: listIssuedBadges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/badges\n  method: post\n  operationId: issueBadge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/badges/{id}\n  method: get\n  operationId: getIssuedBadge\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/badges/{id}/replace\n  method: put\n  operationId: replaceIssuedBadge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{organization_id}/badges/{id}/revoke\n  method: put\n  operationId: revokeIssuedBadge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /organizations/{organization_id}\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/employees\n  method: get\n  operationId: listEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organization_id}/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /obi/v2/issuers/{organization_id}\n  method: get\n  operationId: getObiIssuer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /obi/v2/organizations/{organization_id}/badge_assertions/{id}\n  method: get\n  operationId: getObiBadgeAssertion\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/agentic-access/credly-agentic-access.yml
summary_line: 15 operations · 6 acting · 1 human-in-the-loop
tags:
- Digital Credentials
- Open Badges
- Badging
- Certifications
- Verifiable Credentials
- Pearson
---
