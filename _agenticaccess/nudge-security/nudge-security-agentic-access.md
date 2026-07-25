---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 16
api_specs:
- filename: nudge-security-accounts-api-openapi.yml
  format: yaml
  label: Nudge Security Accounts API
  slug: nudge-security-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/openapi/nudge-security-accounts-api-openapi.yml
- filename: nudge-security-app-integrations-api-openapi.yml
  format: yaml
  label: Nudge Security App Integrations API
  slug: nudge-security-app-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/openapi/nudge-security-app-integrations-api-openapi.yml
- filename: nudge-security-apps-api-openapi.yml
  format: yaml
  label: Nudge Security Apps API
  slug: nudge-security-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/openapi/nudge-security-apps-api-openapi.yml
- filename: nudge-security-events-api-openapi.yml
  format: yaml
  label: Nudge Security Events API
  slug: nudge-security-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/openapi/nudge-security-events-api-openapi.yml
- filename: nudge-security-fields-api-openapi.yml
  format: yaml
  label: Nudge Security Fields API
  slug: nudge-security-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/openapi/nudge-security-fields-api-openapi.yml
- filename: nudge-security-findings-api-openapi.yml
  format: yaml
  label: Nudge Security Findings API
  slug: nudge-security-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/openapi/nudge-security-findings-api-openapi.yml
- filename: nudge-security-labels-api-openapi.yml
  format: yaml
  label: Nudge Security Labels API
  slug: nudge-security-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/openapi/nudge-security-labels-api-openapi.yml
- filename: nudge-security-notifications-api-openapi.yml
  format: yaml
  label: Nudge Security Notifications API
  slug: nudge-security-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/openapi/nudge-security-notifications-api-openapi.yml
- filename: nudge-security-oauth-grants-api-openapi.yml
  format: yaml
  label: Nudge Security OAuth Grants API
  slug: nudge-security-oauth-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/openapi/nudge-security-oauth-grants-api-openapi.yml
- filename: nudge-security-user-groups-api-openapi.yml
  format: yaml
  label: Nudge Security User Groups API
  slug: nudge-security-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/openapi/nudge-security-user-groups-api-openapi.yml
- filename: nudge-security-users-api-openapi.yml
  format: yaml
  label: Nudge Security Users API
  slug: nudge-security-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/openapi/nudge-security-users-api-openapi.yml
consequence_counts:
  read: 16
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nudge Security Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Nudge Security exposes 19 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nudge Security
provider_slug: nudge-security
slug: nudge-security-agentic-access
source_filename: nudge-security-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nudge-security-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 16\n    acting: 3\n  by_consequence:\n    read: 16\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /apps\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{app_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/app-category/{app_id}\n  method: post\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{account_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth-grants\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth-grants/{grant_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{event_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-groups\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-groups/{group_id}/members\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fields\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fields\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labels\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labels\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /findings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app-to-app-integrations\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nudge-security/refs/heads/main/agentic-access/nudge-security-agentic-access.yml
summary_line: 19 operations · 3 acting
tags:
- Access Management
- AI Security
- Compliance
- Governance
- OAuth
- SaaS Management
- SaaS Security
- Security
- Shadow IT
- SSPM
---
