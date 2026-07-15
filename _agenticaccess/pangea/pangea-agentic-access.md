---
acting_count: 18
action_class_counts:
  acting: 18
api_specs:
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea AuthN API
  slug: authn
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea Secure Audit Log API
  slug: secure-audit-log
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea Redact API
  slug: redact
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea Vault API
  slug: vault
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea File Scan API
  slug: file-scan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea IP Intel API
  slug: ip-intel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea Domain & URL Intel API
  slug: domain-intel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea AI Guard & Prompt Guard API
  slug: ai-guard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
consequence_counts:
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pangea Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Pangea exposes 18 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pangea
provider_slug: pangea
slug: pangea-agentic-access
source_filename: pangea-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pangea-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 18\n  by_consequence:\n    write: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/user/create\n  method: post\n  operationId: authnUserCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/user/list\n  method: post\n  operationId: authnUserList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/flow/start\n  method: post\n  operationId: authnFlowStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/client/session/refresh\n  method: post\n  operationId: authnClientSessionRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/log\n  method: post\n  operationId: auditLog\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/log\n  method: post\n  operationId: auditLogBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/search\n  method: post\n  operationId: auditSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/root\n  method: post\n  operationId: auditRoot\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/redact\n  method: post\n  operationId: redactText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/redact_structured\n  method: post\n  operationId: redactStructured\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/encrypt\n  method: post\n  operationId:\
  \ vaultEncrypt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/decrypt\n  method: post\n  operationId: vaultDecrypt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/secret/store\n  method: post\n  operationId: vaultSecretStore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scan\n\
  \  method: post\n  operationId: fileScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/reputation\n  method: post\n  operationId: ipReputation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/geolocate\n  method: post\n  operationId: ipGeolocate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/reputation\n  method: post\n  operationId: domainReputation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/text/guard\n  method: post\n  operationId: aiGuardText\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/agentic-access/pangea-agentic-access.yml
summary_line: 18 operations · 18 acting
tags:
- Security
- AI Security
- Authentication
- Audit Log
- Data Protection
---
