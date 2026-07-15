---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Vault Tokenization API
  slug: vgs-vault-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Accounts Management API
  slug: vgs-accounts-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Routes & Proxy API
  slug: vgs-routes-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Functions API
  slug: vgs-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
- filename: vgs-openapi.yml
  format: yaml
  label: VGS Organizations API
  slug: vgs-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/openapi/vgs-openapi.yml
consequence_counts:
  read: 8
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vgs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Very Good Security exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Very Good Security
provider_slug: vgs
slug: vgs-agentic-access
source_filename: vgs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vgs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 7\n    connected: 8\n  by_consequence:\n    write: 7\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /aliases\n  method: post\n  operationId: createAliases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /aliases\n  method: get\n  operationId: revealMultipleAliases\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aliases/{alias}\n  method: get\n  operationId: revealAlias\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aliases/{alias}\n  method: put\n  operationId: updateAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /aliases/{alias}\n  method: delete\n  operationId: deleteAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations\n\
  \  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations/{organizationId}\n  method: get\n  operationId: getOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vaults\n  method: get\n  operationId: listVaults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vaults\n  method: post\n  operationId: createVault\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vaults/{vaultId}\n\
  \  method: get\n  operationId: getVault\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vaults/{vaultId}/routes\n  method: get\n  operationId: listRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vaults/{vaultId}/routes\n  method: post\n  operationId: createRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vaults/{vaultId}/routes/{routeId}\n  method: get\n  operationId: getRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /vaults/{vaultId}/routes/{routeId}\n  method: put\n  operationId: updateRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vaults/{vaultId}/routes/{routeId}\n  method: delete\n  operationId: deleteRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vgs/refs/heads/main/agentic-access/vgs-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Security
- Tokenization
- Data Privacy
- PCI Compliance
- Vault
---
