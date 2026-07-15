---
acting_count: 42
action_class_counts:
  acting: 42
api_specs:
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Keys API
  slug: unkey-dev-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey APIs (Namespaces) API
  slug: unkey-dev-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Ratelimit API
  slug: unkey-dev-ratelimit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Identities API
  slug: unkey-dev-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Permissions and Roles API
  slug: unkey-dev-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Analytics API
  slug: unkey-dev-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Key Migrations API
  slug: unkey-dev-migrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Deploy API
  slug: unkey-dev-deploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
- filename: unkey-dev-openapi.yml
  format: yaml
  label: Unkey Liveness API
  slug: unkey-dev-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/openapi/unkey-dev-openapi.yml
consequence_counts:
  physical: 2
  safety-critical: 4
  write: 36
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Unkey Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/ratelimit.deleteOverride
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/ratelimit.getOverride
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/ratelimit.listOverrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/ratelimit.setOverride
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/deploy.createDeployment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/deploy.getDeployment
operation_count: 42
overview: 'Unkey exposes 42 API operations that an AI agent could call, of which 42 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 write, 2 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Unkey
provider_slug: unkey-dev
slug: unkey-dev-agentic-access
source_filename: unkey-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/unkey-dev-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    acting: 42\n  by_consequence:\n    write: 36\n    safety-critical: 4\n    physical: 2\n  human_in_the_loop_required: 4\noperations:\n- path: /v2/keys.createKey\n  method: post\n  operationId: keys.createKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/keys.verifyKey\n  method: post\n  operationId: keys.verifyKey\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/keys.getKey\n  method: post\n  operationId: keys.getKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/keys.updateKey\n  method: post\n  operationId: keys.updateKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/keys.deleteKey\n  method: post\n  operationId: keys.deleteKey\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/keys.rerollKey\n  method: post\n  operationId: keys.rerollKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/keys.updateCredits\n  method: post\n  operationId: keys.updateCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/keys.whoami\n\
  \  method: post\n  operationId: keys.whoami\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/keys.migrateKeys\n  method: post\n  operationId: keys.migrateKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/keys.addPermissions\n  method: post\n  operationId: keys.addPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/keys.removePermissions\n  method: post\n  operationId: keys.removePermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/keys.setPermissions\n  method: post\n  operationId: keys.setPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/keys.addRoles\n  method: post\n  operationId: keys.addRoles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/keys.removeRoles\n  method: post\n  operationId: keys.removeRoles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/keys.setRoles\n  method: post\n  operationId: keys.setRoles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/apis.createApi\n  method: post\n  operationId: apis.createApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/apis.getApi\n  method: post\n  operationId: apis.getApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/apis.deleteApi\n  method: post\n  operationId: apis.deleteApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/apis.listKeys\n  method: post\n  operationId: apis.listKeys\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ratelimit.limit\n  method: post\n  operationId: ratelimit.limit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ratelimit.multiLimit\n  method: post\n  operationId: ratelimit.multiLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ratelimit.setOverride\n  method: post\n  operationId: ratelimit.setOverride\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/ratelimit.getOverride\n  method: post\n  operationId: ratelimit.getOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/ratelimit.listOverrides\n  method: post\n  operationId: ratelimit.listOverrides\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/ratelimit.deleteOverride\n  method: post\n  operationId: ratelimit.deleteOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/identities.createIdentity\n  method: post\n  operationId: identities.createIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/identities.getIdentity\n  method: post\n  operationId: identities.getIdentity\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/identities.listIdentities\n  method: post\n  operationId: identities.listIdentities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/identities.updateIdentity\n  method: post\n  operationId: identities.updateIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/identities.deleteIdentity\n  method: post\n  operationId: identities.deleteIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/permissions.createPermission\n  method: post\n  operationId: permissions.createPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/permissions.getPermission\n  method: post\n  operationId: permissions.getPermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/permissions.listPermissions\n  method: post\n  operationId: permissions.listPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/permissions.deletePermission\n  method: post\n  operationId: permissions.deletePermission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/permissions.createRole\n  method: post\n  operationId: permissions.createRole\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/permissions.getRole\n  method: post\n  operationId: permissions.getRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/permissions.listRoles\n  method: post\n  operationId: permissions.listRoles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/permissions.deleteRole\n\
  \  method: post\n  operationId: permissions.deleteRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/analytics.getVerifications\n  method: post\n  operationId: analytics.getVerifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/deploy.createDeployment\n  method: post\n  operationId: deploy.createDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/deploy.getDeployment\n  method: post\n  operationId: deploy.getDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/liveness\n  method: post\n  operationId: liveness\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unkey-dev/refs/heads/main/agentic-access/unkey-dev-agentic-access.yml
summary_line: 42 operations · 42 acting · 4 human-in-the-loop
tags:
- API Keys
- Rate Limiting
- Authentication
- Access Control
- Identity
- RBAC
- Analytics
- Open Source
---
