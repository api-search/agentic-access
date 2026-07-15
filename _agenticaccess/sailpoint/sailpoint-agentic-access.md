---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 16
api_specs:
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud V3 API
  slug: identity-security-cloud-v3-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/v3/identity-security-cloud-v-3-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud V2024 API
  slug: identity-security-cloud-v2024-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/v2024/identity-security-cloud-v-2024-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud V2025 API
  slug: identity-security-cloud-v2025-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/v2025/identity-security-cloud-v-2025-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud Beta API
  slug: identity-security-cloud-beta-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/beta/identity-security-cloud-beta-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint IdentityIQ SCIM API
  slug: identityiq-scim-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/iiq/identityiq-scim-rest-api/
- filename: openapi.yaml
  format: yaml
  label: SailPoint Identity Security Cloud V2026 API
  slug: identity-security-cloud-v2026-api
  spec_type: OpenAPI
  url: https://developer.sailpoint.com/docs/api/v2026/identity-security-cloud-v-2026-api/
consequence_counts:
  read: 16
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sailpoint Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 30
overview: 'SailPoint exposes 30 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 14 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SailPoint
provider_slug: sailpoint
slug: sailpoint-agentic-access
source_filename: sailpoint-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/identity-security-cloud-v3.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 16\n    acting: 14\n  by_consequence:\n    read: 16\n    write: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /public-identities\n  method: get\n  operationId: getPublicIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:identity:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public-identities/{id}\n  method: get\n  operationId: getPublicIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:identity:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity-profiles\n  method: get\n  operationId: listIdentityProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:identity-profile:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity-profiles\n  method: post\n  operationId: createIdentityProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:identity-profile:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity-profiles/{identity-profile-id}\n  method: get\n  operationId: getIdentityProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:identity-profile:read\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /identity-profiles/{identity-profile-id}\n  method: patch\n  operationId: updateIdentityProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:identity-profile:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identity-profiles/{identity-profile-id}\n  method: delete\n  operationId: deleteIdentityProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:identity-profile:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access-profiles\n  method: get\n  operationId: listAccessProfiles\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - idn:access-profile:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access-profiles\n  method: post\n  operationId: createAccessProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:access-profile:manage\n    - idn:entitlement:read\n    - idn:identity:read\n    - idn:sources:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access-profiles/{id}\n  method: get\n  operationId: getAccessProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:access-profile:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access-profiles/{id}\n  method: patch\n  operationId: patchAccessProfile\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:access-profile:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access-profiles/{id}\n  method: delete\n  operationId: deleteAccessProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:access-profile:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access-profiles/{id}/entitlements\n  method: get\n  operationId: listAccessProfileEntitlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:access-profile:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /access-profiles/bulk-delete\n\
  \  method: post\n  operationId: bulkDeleteAccessProfiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:access-profile:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles\n  method: get\n  operationId: listRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:role-unchecked:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles\n  method: post\n  operationId: createRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:role-unchecked:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /roles/{id}\n  method: get\n  operationId: getRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:role-unchecked:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles/{id}\n  method: patch\n  operationId: patchRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:role-unchecked:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles/{id}\n  method: delete\n  operationId: deleteRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:role-unchecked:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /roles/{id}/identities\n  method: get\n  operationId: listRoleIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:role-unchecked:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles/bulk-delete\n  method: post\n  operationId: bulkDeleteRoles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:role-unchecked:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /certifications\n  method: get\n  operationId: listIdentityCertifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:certification:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /certifications/{id}\n  method:\
  \ get\n  operationId: getIdentityCertification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:certification:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /certifications/{id}/access-review-items\n  method: get\n  operationId: listCertificationAccessReviewItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:certification:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /certifications/{id}/decide\n  method: post\n  operationId: makeCertificationDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:certification:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /certifications/{id}/reassign\n  method:\
  \ post\n  operationId: reassignIdentityCertification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:certification:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /certifications/{id}/sign-off\n  method: post\n  operationId: signOffIdentityCertification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - idn:certification:manage\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /certifications/{id}/reviewers\n  method: get\n  operationId: listCertificationReviewers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - idn:certification:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /certifications/{id}/tasks\n  method: get\n  operationId: listCertificationTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:certification:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /certifications/{id}/tasks/{taskId}\n  method: get\n  operationId: getCertificationTask\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - idn:certification:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sailpoint/refs/heads/main/agentic-access/sailpoint-agentic-access.yml
summary_line: 30 operations · 14 acting
tags:
- Access Governance
- Compliance
- IAM
- Identity Management
- Identity Security
- Security
---
