---
acting_count: 284
action_class_counts:
  acting: 284
  connected: 354
api_specs:
- filename: acquia-cloud-openapi.yml
  format: yaml
  label: Acquia Cloud API
  slug: acquia-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/openapi/acquia-cloud-openapi.yml
consequence_counts:
  physical: 8
  read: 354
  safety-critical: 24
  write: 252
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 24
kind: agentic-access
layout: agentic-access
method: generated
name: Acquia Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /account/tokens/{tokenUuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /account/tokens/{tokenUuid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /environments/{environmentId}/cdn
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /environments/{environmentId}/cdn
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/cloud-actions/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/cloud-actions/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/cloud-actions/actions/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/cloud-actions/actions/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/crons/{cronId}/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/crons/{cronId}/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/livedev/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/livedev/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/log-forwarding-destinations/{logForwardingDestinationUuid}/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/log-forwarding-destinations/{logForwardingDestinationUuid}/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/mod-proxy/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/mod-proxy/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/production-mode/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/production-mode/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/servers/{serverId}/actions/reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /environments/{environmentId}/servers/{serverId}/actions/reboot
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /identity-providers/{identityProviderUuid}/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /identity-providers/{identityProviderUuid}/actions/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /subscriptions/{subscriptionUuid}/shield-acl/actions/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /subscriptions/{subscriptionUuid}/shield-acl/actions/reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /environments/{environmentId}/artifacts/actions/switch
operation_count: 638
overview: 'Acquia exposes 638 API operations that an AI agent could call, of which 284 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 354 read, 252 write, 8 physical, and 24 safety-critical.


  24 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Acquia
provider_slug: acquia
slug: acquia-agentic-access
source_filename: acquia-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/acquia-cloud-account.yml, openapi/acquia-cloud-agreements.yml, openapi/acquia-cloud-application-performance-monitoring-services.yml,\n  openapi/acquia-cloud-applications.yml, openapi/acquia-cloud-cloud-ide.yml, openapi/acquia-cloud-codebases.yml,\n  openapi/acquia-cloud-current-system-health.yml, openapi/acquia-cloud-distributions.yml, openapi/acquia-cloud-email.yml,\n  openapi/acquia-cloud-environments.yml, openapi/acquia-cloud-identity-providers.yml, openapi/acquia-cloud-invite.yml,\n  openapi/acquia-cloud-messages.yml, openapi/acquia-cloud-notifications.yml, openapi/acquia-cloud-openapi-full.yml,\n  openapi/acquia-cloud-options.yml, openapi/acquia-cloud-organizations.yml, openapi/acquia-cloud-private-networks.yml,\n  openapi/acquia-cloud-subscriptions.yml, openapi/acquia-cloud-teams-and-permissions.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A\
  \ governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 638\n  by_action_class:\n    connected: 354\n    acting: 284\n  by_consequence:\n    read: 354\n    write: 252\n    safety-critical: 24\n    physical: 8\n  human_in_the_loop_required: 24\noperations:\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/applications/{applicationUuid}/actions/mark-recent\n  method: post\n  operationId: postAccountApplicationMarkRecent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /account/applications/{applicationUuid}/actions/star\n  method: post\n  operationId: postAccountApplicationStar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/applications/{applicationUuid}/actions/unstar\n  method: post\n  operationId: postAccountApplicationUnstar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/applications/{applicationUuid}/has-permission\n  method: get\n  operationId: getAccountApplicationHasPermission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/applications/{applicationUuid}/is-admin\n  method: get\n  operationId: getAccountApplicationIsAdministrator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/applications/{applicationUuid}/is-owner\n  method: get\n  operationId: getAccountApplicationIsOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/drush-aliases/download\n  method: get\n  operationId: getAccountDrushAliasesDownload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/ides\n  method: get\n  operationId: getAccountIdes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/invites\n  method: get\n  operationId: getAccountInvites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/messages\n  method: get\n  operationId: getAccountMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/organizations/{organizationUuid}/is-admin\n  method: get\n  operationId: getAccountOrganizationIsAdministrator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/organizations/{organizationUuid}/is-owner\n  method: get\n  operationId: getAccountOrganizationIsOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/password\n  method: post\n  operationId: postAccountPassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/ssh-keys\n  method: get\n  operationId: getAccountSshKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/ssh-keys\n  method: post\n  operationId: postAccountSshKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /account/ssh-keys/{sshKeyUuid}\n  method: delete\n  operationId: deleteAccountSshKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/ssh-keys/{sshKeyUuid}\n  method: get\n  operationId: getAccountSshKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/subscriptions/{subscriptionUuid}/is-admin\n  method: get\n  operationId: getAccountSubscriptionIsAdministrator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/subscriptions/{subscriptionUuid}/is-owner\n  method: get\n  operationId: getAccountSubscriptionIsOwner\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/teams/{teamUuid}/has-permission\n  method: get\n  operationId: getAccountTeamHasPermission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/teams/{teamUuid}/is-admin\n  method: get\n  operationId: getAccountTeamIsAdministrator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/teams/{teamUuid}/is-owner\n  method: get\n  operationId: getAccountTeamIsOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/tokens\n  method: get\n  operationId: getAccountTokens\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/tokens\n  method: post\n  operationId: postAccountTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/tokens/{tokenUuid}\n  method: delete\n  operationId: deleteAccountToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account/tokens/{tokenUuid}\n  method: get\n  operationId: getAccountToken\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agreements\n  method: get\n  operationId: getAgreements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agreements/{agreementUuid}\n  method: get\n  operationId: getAgreement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agreements/{agreementUuid}/actions/accept\n  method: post\n  operationId: postAcceptAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agreements/{agreementUuid}/actions/decline\n  method: post\n  operationId: postDeclineAgreement\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agreements/{agreementUuid}/invitees\n  method: get\n  operationId: getInvitees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/settings/apm\n  method: get\n  operationId: getEnvironmentsApmSetting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/settings/apm\n  method: put\n  operationId: putEnvironmentsApmSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{subscriptionUuid}/apm\n  method: get\n  operationId: getSubscriptionApmTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscriptionUuid}/apm/{apmType}\n  method: get\n  operationId: getSubscriptionApmType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscriptionUuid}/apm/{apmType}/actions/opt-in\n  method: post\n  operationId: postSubscriptionApmOptIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /applications\n  method: get\n  operationId: getApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}\n  method: get\n  operationId: getApplicationByUuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}\n  method: put\n  operationId: putApplicationByUuid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/artifacts\n  method: get\n  operationId: getArtifactsByApplicationUuid\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/artifacts/{artifactId}\n  method: get\n  operationId: getArtifactByApplicationUuidAndId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/code\n  method: get\n  operationId: getCodeByApplicationUuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/code-studio\n  method: delete\n  operationId: deleteCodeStudioProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /applications/{applicationUuid}/code-studio\n  method: get\n  operationId: getCodeStudioProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/code-studio\n  method: post\n  operationId: postCodeStudioProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/databases\n  method: get\n  operationId: getApplicationDatabases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/databases\n  method: post\n  operationId:\
  \ postApplicationDatabaseCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/databases/{name}\n  method: delete\n  operationId: postApplicationDatabaseDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/databases/{name}/actions/erase\n  method: post\n  operationId: postApplicationDatabaseErase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/email/domains\n  method: get\n  operationId: getApplicationEmailDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/email/domains/{domainRegistrationUuid}/actions/associate\n  method: post\n  operationId: postApplicationAssociateEmailDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/email/domains/{domainRegistrationUuid}/actions/disassociate\n  method: post\n  operationId: postApplicationDisassociateEmailDomain\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/environments\n  method: get\n  operationId: getApplicationEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/environments\n  method: post\n  operationId: postApplicationEnvironments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/features\n  method: get\n  operationId: getApplicationFeatures\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/ides\n  method: get\n  operationId: getApplicationIdes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/ides\n  method: post\n  operationId: postApplicationsIde\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/messages\n  method: get\n  operationId: getApplicationMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /applications/{applicationUuid}/metrics/usage\n  method: get\n  operationId: getApplicationsUsageLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/metrics/usage/data\n  method: get\n  operationId: getApplicationsUsageData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/metrics/usage/data-by-environment\n  method: get\n  operationId: getApplicationsUsageDataByEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/metrics/usage/views-by-environment\n  method: get\n  operationId: getApplicationsUsageViewsDataByEnvironment\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/metrics/usage/visits-by-environment\n  method: get\n  operationId: getApplicationsUsageVisitsDataByEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/metrics/usage/{usageMetric}\n  method: get\n  operationId: getApplicationsUsageMetricData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/notifications\n  method: get\n  operationId: getApplicationNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/permissions\n\
  \  method: get\n  operationId: getApplicationPermissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/search\n  method: get\n  operationId: getApplicationSearchList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/search/config-sets\n  method: get\n  operationId: getApplicationSearchConfigurationSets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/search/config-sets\n  method: post\n  operationId: postApplicationSearchConfigurationSets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/search/config-sets/{configurationSetId}\n  method: delete\n  operationId: deleteApplicationSearchConfigurationSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/search/config-sets/{configurationSetId}\n  method: get\n  operationId: getApplicationSearchConfigurationSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/settings\n  method: get\n  operationId: getApplicationSettings\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/settings/hosting\n  method: get\n  operationId: getApplicationHostingSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/settings/keys\n  method: get\n  operationId: getApplicationLegacyProductKeysSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/settings/ra\n  method: get\n  operationId: getApplicationRemoteAdministrationSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/settings/ra\n  method: put\n  operationId:\
  \ putApplicationRemoteAdministrationSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/settings/security\n  method: get\n  operationId: getApplicationSecuritySettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/settings/security\n  method: put\n  operationId: putApplicationSecuritySettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/tags\n\
  \  method: get\n  operationId: getApplicationTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/tags\n  method: post\n  operationId: postApplicationsTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/tags/{tagName}\n  method: delete\n  operationId: deleteApplicationTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationUuid}/tasks\n\
  \  method: get\n  operationId: getApplicationTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationUuid}/teams\n  method: get\n  operationId: getApplicationTeams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ides/{ideUuid}\n  method: delete\n  operationId: deleteIde\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ides/{ideUuid}\n  method: get\n  operationId: getIde\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}/codebase\n  method: get\n  operationId: api_applications_applicationIdcodebase_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /codebases\n  method: get\n  operationId: api_codebases_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /codebases/{codebaseId}\n  method: delete\n  operationId: api_codebases_codebaseId_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /codebases/{codebaseId}\n  method: get\n  operationId: get_codebase_by_id\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /codebases/{codebaseId}\n  method: put\n  operationId: api_codebases_codebaseId_put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /codebases/{codebaseId}/bulk-code-switch\n  method: get\n  operationId: api_codebases_codebaseIdbulk-code-switch_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /codebases/{codebaseId}/bulk-code-switch\n  method: post\n  operationId: create_bulk_code_switch_resource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /codebases/{codebaseId}/bulk-code-switch/{bulkCodeSwitchId}\n  method: get\n  operationId: get_bulk_code_switch_resource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /codebases/{codebaseId}/references\n  method: get\n  operationId: get_references_by_codebase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /codebases/{codebaseId}/references/{referenceName}\n  method: get\n  operationId: get_single_reference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscriptionId}/codebases\n\
  \  method: get\n  operationId: subscription_codebases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscriptionId}/codebases\n  method: options\n  operationId: api_subscriptions_subscriptionIdcodebases_options\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getSystemHealthStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /distributions\n  method: get\n  operationId: getDistributions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /distributions/{name}\n  method: get\n  operationId: getDistributionByName\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}/email\n  method: get\n  operationId: getEmailStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}\n  method: delete\n  operationId: deleteEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}\n  method: get\n  operationId: getEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}\n\
  \  method: options\n  operationId: optionsEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /environments/{environmentId}\n  method: put\n  operationId: putEnvironment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/actions/change-label\n  method: post\n  operationId: postChangeEnvironmentLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/actions/clear-caches\n\
  \  method: post\n  operationId: postEnvironmentsClearCaches\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/artifacts/actions/switch\n  method: post\n  operationId: postDeployArtifact\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /environments/{environmentId}/available-runtimes\n  method: get\n  operationId: getAvailableRuntimes\n  x-agentic-access:\n    action-class: connected\n   \n\n# --- truncated at 32 KB (191 KB total) ---\n# Full\
  \ source: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/agentic-access/acquia-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/agentic-access/acquia-agentic-access.yml
summary_line: 638 operations · 284 acting · 24 human-in-the-loop
tags:
- Content
- Experience
---
