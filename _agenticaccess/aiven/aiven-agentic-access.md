---
acting_count: 255
action_class_counts:
  acting: 255
  connected: 202
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Aiven REST API
  slug: aiven-api
  spec_type: OpenAPI
  url: https://api.aiven.io/doc/
consequence_counts:
  physical: 15
  read: 202
  safety-critical: 14
  write: 226
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 14
kind: agentic-access
layout: agentic-access
method: generated
name: Aiven Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /access_token/{token_prefix}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /me/authentication_methods/{user_authentication_method_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /organization/{organization_id}/user/{member_user_id}/access-token/{token_prefix}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /organization/{organization_id}/user/{member_user_id}/reset_password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /project/{project}/service/{service_name}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /project/{project}/service/{service_name}/clickhouse/user/{user_uuid}/password
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /project/{project}/service/{service_name}/connectors/{connector_name}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /project/{project}/service/{service_name}/flink/application/{application_id}/deployment/{deployment_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /project/{project}/service/{service_name}/flink/jar_application/{application_id}/deployment/{deployment_id}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /project/{project}/service/{service_name}/opensearch/security/admin
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /project/{project}/service/{service_name}/query/stats/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /project/{project}/service/{service_name}/user/{service_username}/credentials/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /user/password_reset/{verification_code}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /user/password_reset_request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /account/{account_id}/payment_method/{card_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/{account_id}/payment_methods
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /card
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /card/{card_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /card/{card_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organization/{organization_id}/custom-cloud-environments/{custom_cloud_environment_id}/provision
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /organization/{organization_id}/payment-method/credit-card/{payment_method_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organization/{organization_id}/payment-method/credit-cards
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /project/{project}/invite
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /project/{project}/service/{service_name}/flink/application/{application_id}/deployment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /project/{project}/service/{service_name}/flink/application/{application_id}/deployment/{deployment_id}
operation_count: 457
overview: 'Aiven exposes 457 API operations that an AI agent could call, of which 255 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 202 read, 226 write, 15 physical, and 14 safety-critical.


  14 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Aiven
provider_slug: aiven
slug: aiven-agentic-access
source_filename: aiven-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/aiven-aiven-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 457\n  by_action_class:\n    acting: 255\n    connected: 202\n  by_consequence:\n    physical: 15\n    read: 202\n    write: 226\n    safety-critical: 14\n  human_in_the_loop_required: 14\noperations:\n- path: /account/{account_id}/payment_methods\n  method: post\n  operationId: AccountAttachPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounts:write\n    - payments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/payment_methods\n  method: get\n  operationId: AccountPaymentMethodsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    - payments:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/authentication\n  method: post\n  operationId: AccountAuthenticationMethodCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    - authentication:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/authentication\n  method: get\n  operationId: AccountAuthenticationMethodsList\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - accounts:read\n    - authentication:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/authentication/{account_authentication_method_id}\n  method: delete\n  operationId: AccountAuthenticationMethodDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    - authentication:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/authentication/{account_authentication_method_id}\n  method: get\n  operationId: AccountAuthenticationMethodGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    - authentication:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/authentication/{account_authentication_method_id}\n\
  \  method: put\n  operationId: AccountAuthenticationMethodUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    - authentication:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/billing-group\n  method: get\n  operationId: AccountBillingGroupList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account\n  method: post\n  operationId: AccountCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account\n  method: get\n  operationId: AccountList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}\n  method: delete\n  operationId: AccountDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}\n  method: get\n  operationId: AccountGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}\n  method:\
  \ put\n  operationId: AccountUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/events\n  method: get\n  operationId: AccountEventList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/parent_account\n  method: put\n  operationId: AccountMove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /account/{account_id}/payment_method/{card_id}\n  method: delete\n  operationId: AccountPaymentMethodDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounts:write\n    - payments:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/projects\n  method: get\n  operationId: AccountProjectsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    - projects:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/project/{project_name}/teams\n  method: get\n  operationId: AccountProjectsTeamsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    scope:\n    - accounts:read\n    - projects:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/teams\n  method: post\n  operationId: AccountTeamCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/teams\n  method: get\n  operationId: AccountTeamList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/team/{team_id}\n  method: delete\n  operationId: AccountTeamDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/team/{team_id}\n  method: get\n  operationId: AccountTeamGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/team/{team_id}\n  method: put\n  operationId: AccountTeamUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/team/{team_id}/invites\n  method: get\n  operationId: AccountTeamInvitesList\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/team/{team_id}/invites/{user_email}\n  method: delete\n  operationId: AccountTeamMemberCancelInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/invite/{invite_verification_code}\n  method: post\n  operationId: AccountTeamMemberVerifyInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/team/{team_id}/member/{user_id}\n\
  \  method: delete\n  operationId: AccountTeamMembersDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/team/{team_id}/members\n  method: post\n  operationId: AccountTeamMembersInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/team/{team_id}/members\n  method: get\n  operationId: AccountTeamMembersList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/team/{team_id}/project/{project}\n  method: post\n  operationId: AccountTeamProjectAssociate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    - projects:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/team/{team_id}/project/{project}\n  method: put\n  operationId: AccountTeamProjectAssociationUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    - projects:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /account/{account_id}/team/{team_id}/project/{project}\n  method: delete\n  operationId: AccountTeamProjectDisassociate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    - projects:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/{account_id}/team/{team_id}/projects\n  method: get\n  operationId: AccountTeamProjectList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    - projects:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/user/{user_id}/projects\n  method: get\n  operationId: AccountUserProjectsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n\
  \    - projects:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/user/{user_id}/teams\n  method: get\n  operationId: AccountUserTeamsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/{account_id}/users/search\n  method: post\n  operationId: AccountUsersSearch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/application-users/{user_id}/access-tokens\n  method: post\n  operationId: ApplicationUserAccessTokenCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - accounts:write\n    - authentication:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/application-users/{user_id}/access-tokens\n  method: get\n  operationId: ApplicationUserAccessTokensList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    - authentication:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organization_id}/application-users/{user_id}/access-tokens/{token_prefix}\n  method: delete\n  operationId: ApplicationUserAccessTokenDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    - authentication:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/application-users\n  method: post\n  operationId: ApplicationUserCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    - authentication:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/application-users\n  method: get\n  operationId: ApplicationUsersList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    - authentication:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organization_id}/application-users/{user_id}\n  method: delete\n  operationId: ApplicationUserDelete\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    - authentication:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/application-users/{user_id}\n  method: get\n  operationId: ApplicationUserGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    - authentication:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organization_id}/application-users/{user_id}\n  method: patch\n  operationId: ApplicationUserUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/authentication-methods/{authentication_method_id}/domains\n  method: put\n  operationId: OrganizationAuthDomainLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/authentication-methods/{authentication_method_id}/domains\n  method: get\n  operationId: OrganizationAuthDomainList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organization_id}/authentication-methods/{authentication_method_id}/domains/{domain_id}\n  method:\
  \ delete\n  operationId: OrganizationAuthDomainUnlink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credit-memos/{credit_memo_id}/{download_cookie}\n  method: get\n  operationId: BillingCreditMemoDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-group\n  method: post\n  operationId: BillingGroupCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /billing-group\n  method: get\n  operationId: BillingGroupList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-group/{billing_group_id}/credits\n  method: post\n  operationId: BillingGroupCreditsClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing-group/{billing_group_id}/credits\n  method: get\n  operationId: BillingGroupCreditsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-group/{billing_group_id}\n\
  \  method: delete\n  operationId: BillingGroupDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing-group/{billing_group_id}\n  method: get\n  operationId: BillingGroupGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-group/{billing_group_id}\n  method: put\n  operationId: BillingGroupUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /billing-group/{billing_group_id}/events\n  method: get\n  operationId: BillingGroupEventList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-group/{billing_group_id}/invoice/{invoice_number}/csv\n  method: get\n  operationId: BillingGroupInvoiceCsvGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-group/{billing_group_id}/invoice/{invoice_number}/{download_cookie}\n  method: get\n  operationId: BillingGroupInvoiceDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-group/{billing_group_id}/invoice/{invoice_number}\n  method: get\n  operationId: BillingGroupInvoiceGet\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-group/{billing_group_id}/invoice/{invoice_number}/lines\n  method: get\n  operationId: BillingGroupInvoiceLinesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-group/{billing_group_id}/invoice\n  method: get\n  operationId: BillingGroupInvoiceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-group/{billing_group_id}/project-assign/{project}\n  method: post\n  operationId: BillingGroupProjectAssign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - billing:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing-group/{billing_group_id}/projects\n  method: get\n  operationId: BillingGroupProjectList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing-group/{billing_group_id}/projects-assign\n  method: post\n  operationId: BillingGroupProjectsAssign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoices/{invoice_number}\n  method: get\n  operationId: InvoiceGet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organization_id}/addresses\n  method: post\n  operationId: OrganizationAddressCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/addresses\n  method: get\n  operationId: OrganizationAddressList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organization_id}/address/{address_id}\n  method: delete\n  operationId: OrganizationAddressDelete\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/address/{address_id}\n  method: get\n  operationId: OrganizationAddressGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    - billing:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organization_id}/address/{address_id}\n  method: patch\n  operationId: OrganizationAddressUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    - billing:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clouds\n  method: get\n  operationId: ListClouds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project/{project}/clouds\n  method: get\n  operationId: ListProjectClouds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - projects:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant}/privatelink-availability\n  method: get\n  operationId: PublicPrivatelinkAvailabilityList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant}/static-ip-availability\n  method: get\n  operationId: PublicStaticIPAvailabilityList\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organization_id}/custom-cloud-environments\n  method: post\n  operationId: CustomCloudEnvironmentCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/custom-cloud-environments/{custom_cloud_environment_id}\n  method: delete\n  operationId: CustomCloudEnvironmentDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/custom-cloud-environments/{custom_cloud_environment_id}\n\
  \  method: get\n  operationId: CustomCloudEnvironmentGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organization_id}/custom-cloud-environments/{custom_cloud_environment_id}\n  method: put\n  operationId: CustomCloudEnvironmentUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/custom-cloud-environments/{custom_cloud_environment_id}/permissions\n  method: get\n  operationId: CustomCloudEnvironmentPermissionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organization_id}/custom-cloud-environments/{custom_cloud_environment_id}/permissions\n  method: put\n  operationId: CustomCloudEnvironmentPermissionsSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/custom-cloud-environments/{custom_cloud_environment_id}/provision\n  method: post\n  operationId: CustomCloudEnvironmentProvision\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/domains\n  method: post\n  operationId: OrganizationDomainAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/domains\n  method: get\n  operationId: OrganizationDomainsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organization_id}/domains/{domain_id}\n  method: patch\n  operationId: OrganizationDomainUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n\
  \    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/domains/{domain_id}\n  method: delete\n  operationId: OrganizationDomainsRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/domains/{domain_id}/verify\n  method: post\n  operationId: OrganizationDomainVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/user-groups\n  method: post\n  operationId: UserGroupCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/user-groups\n  method: get\n  operationId: UserGroupsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organization_id}/user-groups/{user_group_id}\n  method: delete\n  operationId: UserGroupDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization/{organization_id}/user-groups/{user_group_id}\n  method: get\n  operationId: UserGroupGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accounts:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization/{organization_id}/user-groups/{user_group_id}\n  method: patch\n  operationId: UserGroupUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accounts:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\n# --- truncated at 32 KB (163 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/aiven/refs/heads/main/agentic-access/aiven-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiven/refs/heads/main/agentic-access/aiven-agentic-access.yml
summary_line: 457 operations · 255 acting · 14 human-in-the-loop
tags:
- Managed Data Infrastructure
- Apache Kafka
- PostgreSQL
- OpenSearch
- ClickHouse
- Redis
- MySQL
- Open Source
- Cloud Database
- DBaaS
- Data Streaming
- Data Platform
---
