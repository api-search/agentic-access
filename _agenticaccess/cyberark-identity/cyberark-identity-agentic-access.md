---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 6
api_specs:
- filename: cyberark-identity-authentication-api-openapi.yml
  format: yaml
  label: CyberArk Identity Authentication API
  slug: cyberark-identity-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark-identity/refs/heads/main/openapi/cyberark-identity-authentication-api-openapi.yml
- filename: cyberark-identity-cdirectoryservice-api-openapi.yml
  format: yaml
  label: CyberArk Identity CDirectoryService API
  slug: cyberark-identity-cdirectoryservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark-identity/refs/heads/main/openapi/cyberark-identity-cdirectoryservice-api-openapi.yml
- filename: cyberark-identity-extdata-api-openapi.yml
  format: yaml
  label: CyberArk Identity ExtData API
  slug: cyberark-identity-extdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark-identity/refs/heads/main/openapi/cyberark-identity-extdata-api-openapi.yml
- filename: cyberark-identity-org-api-openapi.yml
  format: yaml
  label: CyberArk Identity Org API
  slug: cyberark-identity-org-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark-identity/refs/heads/main/openapi/cyberark-identity-org-api-openapi.yml
- filename: cyberark-identity-scim-api-openapi.yml
  format: yaml
  label: CyberArk Identity SCIM API
  slug: cyberark-identity-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark-identity/refs/heads/main/openapi/cyberark-identity-scim-api-openapi.yml
- filename: cyberark-identity-usermgmt-api-openapi.yml
  format: yaml
  label: CyberArk Identity UserMgmt API
  slug: cyberark-identity-usermgmt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark-identity/refs/heads/main/openapi/cyberark-identity-usermgmt-api-openapi.yml
- filename: cyberark-identity-oauth-api-openapi.yml
  format: yaml
  label: CyberArk Identity O Auth API
  slug: cyberark-identity-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cyberark-identity/refs/heads/main/openapi/cyberark-identity-oauth-api-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cyberark Identity Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /UserMgmt/InviteUsers
operation_count: 22
overview: 'CyberArk Identity exposes 22 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 15 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CyberArk Identity
provider_slug: cyberark-identity
slug: cyberark-identity-agentic-access
source_filename: cyberark-identity-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/cyberark-identity-authentication-api-openapi.yml, openapi/cyberark-identity-cdirectoryservice-api-openapi.yml,\n  openapi/cyberark-identity-extdata-api-openapi.yml, openapi/cyberark-identity-oauth-api-openapi.yml,\n  openapi/cyberark-identity-org-api-openapi.yml, openapi/cyberark-identity-scim-api-openapi.yml,\n  openapi/cyberark-identity-usermgmt-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 16\n    connected: 6\n  by_consequence:\n    write: 15\n    read: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /Security/StartAuthentication\n  method: post\n  operationId: postSecurityStartAuthentication\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Security/AdvanceAuthentication\n  method: post\n  operationId: postSecurityAdvanceAuthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Security/Logout\n  method: post\n  operationId: postSecurityLogout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /CDirectoryService/CreateUser\n  method: post\n  operationId: postCDirectoryServiceCreateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /CDirectoryService/GetUser\n  method: post\n  operationId: postCDirectoryServiceGetUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /CDirectoryService/ChangeUser\n  method: post\n  operationId: postCDirectoryServiceChangeUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /ExtData/GetColumns\n  method: post\n  operationId: postExtDataGetColumns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /OAuth2/Token/{appId}\n  method: post\n  operationId: postOAuth2TokenByAppId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Org/Create\n  method: post\n  operationId: postOrgCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /Org/ListAll\n  method: post\n  operationId: postOrgListAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Users\n  method: get\n  operationId: getScimV2Users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Users\n  method: post\n  operationId: postScimV2Users\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Users/{id}\n  method: get\n  operationId: getScimV2UsersById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scim/v2/Users/{id}\n  method: put\n  operationId: putScimV2UsersById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Users/{id}\n  method: delete\n  operationId: deleteScimV2UsersById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scim/v2/Groups\n  method: get\n  operationId: getScimV2Groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /scim/v2/Groups/{id}\n  method: delete\n  operationId: deleteScimV2GroupsById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /UserMgmt/GetUserInfo\n  method: post\n  operationId: postUserMgmtGetUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /UserMgmt/ChangeUserAttributes\n  method: post\n  operationId: postUserMgmtChangeUserAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /UserMgmt/InviteUsers\n\
  \  method: post\n  operationId: postUserMgmtInviteUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /UserMgmt/SetCloudLock\n  method: post\n  operationId: postUserMgmtSetCloudLock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /UserMgmt/RemoveUsers\n  method: post\n  operationId: postUserMgmtRemoveUsers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyberark-identity/refs/heads/main/agentic-access/cyberark-identity-agentic-access.yml
summary_line: 22 operations · 16 acting
tags:
- Identity
- Access Management
- Identity and Access Management
- SSO
- Multi-Factor Authentication
- Authentication
- Zero Trust
---
