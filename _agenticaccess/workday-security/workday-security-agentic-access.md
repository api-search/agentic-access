---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 16
api_specs:
- filename: Authentication_OpenAPI.json
  format: json
  label: Workday Authentication API
  slug: workday-authentication-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Authentication_OpenAPI.json
- filename: Identity_Management_OpenAPI.json
  format: json
  label: Workday Identity Management API
  slug: workday-identity-management-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Identity_Management_OpenAPI.json
- filename: Security_Groups_OpenAPI.json
  format: json
  label: Workday Security Groups API
  slug: workday-security-groups-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Security_Groups_OpenAPI.json
- filename: Audit_OpenAPI.json
  format: json
  label: Workday Audit and Compliance API
  slug: workday-audit-and-compliance-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Audit_OpenAPI.json
- filename: Privacy_OpenAPI.json
  format: json
  label: Workday Privacy API
  slug: workday-privacy-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Security/v44.0/Privacy_OpenAPI.json
consequence_counts:
  read: 16
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Workday Security Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Workday Security exposes 17 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Workday Security
provider_slug: workday-security
slug: workday-security-agentic-access
source_filename: workday-security-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/workday-security-audit-openapi.yml, openapi/workday-security-authentication-openapi.yml,\n  openapi/workday-security-identity-management-openapi.yml, openapi/workday-security-security-groups-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 16\n    acting: 1\n  by_consequence:\n    read: 16\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /auditLogs\n  method: get\n  operationId: listAuditLogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auditLogs/{auditLogId}\n  method: get\n  operationId: getAuditLogEntry\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /securityAudit/permissionChanges\n  method: get\n  operationId: listPermissionChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /complianceReports\n  method: get\n  operationId: listComplianceReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth2/{tenant}/token\n  method: post\n  operationId: requestAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/{tenant}/sessions\n\
  \  method: get\n  operationId: listActiveSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{tenant}/authenticationPolicies\n  method: get\n  operationId: listAuthenticationPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accountSignons\n  method: get\n  operationId: listAccountSignons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accountSignons/{signonId}\n  method: get\n  operationId: getAccountSignon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /unidentifiedSignons\n  method: get\n  operationId: listUnidentifiedSignons\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userAccounts\n  method: get\n  operationId: listUserAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /userAccounts/{accountId}\n  method: get\n  operationId: getUserAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /securityGroups\n  method: get\n  operationId: listSecurityGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /securityGroups/{securityGroupId}\n  method: get\n  operationId: getSecurityGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /securityGroups/{securityGroupId}/members\n  method: get\n  operationId: listSecurityGroupMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainSecurityPolicies\n  method: get\n  operationId: listDomainSecurityPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainSecurityPolicies/{policyId}\n  method: get\n  operationId: getDomainSecurityPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-security/refs/heads/main/agentic-access/workday-security-agentic-access.yml
summary_line: 17 operations · 1 acting
tags:
- Access Control
- Audit
- Authentication
- Compliance
- Enterprise
- Identity Management
- Privacy
- SAML
- Security
- SSO
---
