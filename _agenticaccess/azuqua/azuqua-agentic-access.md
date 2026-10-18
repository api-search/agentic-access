---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 13
api_specs:
- filename: azuqua-account-api-openapi.yml
  format: yaml
  label: Azuqua Account API
  slug: azuqua-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-account-api-openapi.yml
- filename: azuqua-accounts-api-openapi.yml
  format: yaml
  label: Azuqua Accounts API
  slug: azuqua-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-accounts-api-openapi.yml
- filename: azuqua-connectors-api-openapi.yml
  format: yaml
  label: Azuqua Connectors API
  slug: azuqua-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-connectors-api-openapi.yml
- filename: azuqua-flo-api-openapi.yml
  format: yaml
  label: Azuqua Flo API
  slug: azuqua-flo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-flo-api-openapi.yml
- filename: azuqua-folder-api-openapi.yml
  format: yaml
  label: Azuqua Folder API
  slug: azuqua-folder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-folder-api-openapi.yml
- filename: azuqua-folders-api-openapi.yml
  format: yaml
  label: Azuqua Folders API
  slug: azuqua-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-folders-api-openapi.yml
- filename: azuqua-org-api-openapi.yml
  format: yaml
  label: Azuqua Org API
  slug: azuqua-org-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-org-api-openapi.yml
- filename: azuqua-user-api-openapi.yml
  format: yaml
  label: Azuqua User API
  slug: azuqua-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/openapi/azuqua-user-api-openapi.yml
consequence_counts:
  read: 13
  safety-critical: 1
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Azuqua Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/flo/{flo_id}/disable
operation_count: 28
overview: 'Azuqua exposes 28 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 14 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Azuqua
provider_slug: azuqua
slug: azuqua-agentic-access
source_filename: azuqua-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/azuqua-page-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 15\n    connected: 13\n  by_consequence:\n    write: 14\n    read: 13\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v2/account/{account_id}\n  method: delete\n  operationId: delete-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account/{account_id}\n  method: get\n  operationId: read-account\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account/{account_id}/user/{user_id}/permissions\n  method: put\n  operationId: share-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts\n  method: get\n  operationId: get-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/connectors/{connector_name}/{connector_version}\n  method: get\n  operationId: get-connector-metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/flo/{flo_id}\n\
  \  method: delete\n  operationId: delete-flo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/flo/{flo_id}\n  method: get\n  operationId: read-flo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/flo/{flo_id}\n  method: put\n  operationId: update-flo-metadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/flo/{flo_id}/accounts\n  method: get\n  operationId: get-accounts-for-flo\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/flo/{flo_id}/copy\n  method: post\n  operationId: duplicate-flo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/flo/{flo_id}/copy/org/{org_id}\n  method: post\n  operationId: copy-flo-into-organization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/flo/{flo_id}/disable\n  method: put\n  operationId: disable-flo\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/flo/{flo_id}/enable\n  method: put\n  operationId: enable-flo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/flo/{flo_id}/inputs\n  method: get\n  operationId: get-flo-inputs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/flo/{flo_id}/move/folder/{folder_id}\n  method: put\n  operationId: move-flo-to-folder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/folder\n  method: post\n  operationId: create-folder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/folder/{folder_id}\n  method: delete\n  operationId: delete-tab\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/folder/{folder_id}\n  method: get\n  operationId: read-folder\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/folder/{folder_id}\n  method: put\n  operationId: update-folder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/folder/{folder_id}/flos\n  method: get\n  operationId: read-flos-in-folder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/folder/{folder_id}/user/{user_id}/permissions\n  method: put\n  operationId: add-user-to-tab-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/folder/{folder_id}/users\n  method: get\n  operationId: read-folder-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/folders\n  method: get\n  operationId: get-folders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/org\n  method: get\n  operationId: read-organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/org\n  method: put\n  operationId: update-org\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/org/flos\n  method: get\n  operationId: get-flos-in-organization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/org/user/{user_id}/permissions\n  method: put\n  operationId: update-user-role\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/user/orgs\n  method: get\n  operationId: read-user-orgs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azuqua/refs/heads/main/agentic-access/azuqua-agentic-access.yml
summary_line: 28 operations · 15 acting · 1 human-in-the-loop
tags:
- Company
- Integration
- iPaaS
- Workflow Automation
- Integration Platform
- Automation
- Connectors
- No-Code
---
