---
acting_count: 302
action_class_counts:
  acting: 302
  connected: 244
api_specs:
- filename: openpath-openapi-original.json
  format: json
  label: Openpath API
  slug: openpath-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpath/refs/heads/main/openapi/openpath-openapi-original.json
consequence_counts:
  physical: 35
  read: 244
  safety-critical: 4
  write: 263
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Openpath Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /auth/resetPassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /orgs/{orgId}/entries/{entryId}/revertTempState
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /orgs/{orgId}/entries/{entryId}/setTempState
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /orgs/{orgId}/zones/apbReset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /auth/setupMobile
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/parcels/sendEmail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/parcels/users/{userId}/sendRecipientParcelReminder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/users/{userId}/credentials/{credentialId}/setupMobile
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/users/{userId}/credentials/{credentialId}/setupWallet
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/users/{userId}/verifyEmail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/wirelessGateways
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/wirelessGateways/updateFirmwareBatch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orgs/{orgId}/wirelessGateways/{wirelessGatewayId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /orgs/{orgId}/wirelessGateways/{wirelessGatewayId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/wirelessGateways/{wirelessGatewayId}/activate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/wirelessGateways/{wirelessGatewayId}/syncDevices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/wirelessGateways/{wirelessGatewayId}/updateFirmware
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/wirelessLockGateways
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/wirelessLockGateways/updateFirmwareBatch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orgs/{orgId}/wirelessLockGateways/{wirelessLockGatewayId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /orgs/{orgId}/wirelessLockGateways/{wirelessLockGatewayId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/wirelessLockGateways/{wirelessLockGatewayId}/syncDevices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/wirelessLockGateways/{wirelessLockGatewayId}/updateFirmware
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orgs/{orgId}/wirelessLockProviders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /orgs/{orgId}/wirelessLockProviders/{wirelessLockProviderId}
operation_count: 546
overview: 'Openpath exposes 546 API operations that an AI agent could call, of which 302 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 244 read, 263 write, 35 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Openpath
provider_slug: openpath
slug: openpath-agentic-access
source_filename: openpath-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/openpath-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 546\n  by_action_class:\n    connected: 244\n    acting: 302\n  by_consequence:\n    read: 244\n    write: 263\n    physical: 35\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /billableFeatures\n  method: get\n  operationId: globalListBillableFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/accessTokens/{token}\n  method: get\n  operationId: describeAccessToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /identities/{identityId}/nicknames\n  method: get\n  operationId: listIdentityNicknames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identities/{identityId}/nicknames\n  method: patch\n  operationId: updateIdentityNicknames\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/wirelessLocks\n  method: get\n  operationId: listWirelessLocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/wirelessLocks\n  method: post\n  operationId: createWirelessLock\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/wirelessGateways\n  method: get\n  operationId: listWirelessGateways\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/wirelessGateways\n  method: post\n  operationId: createWirelessGateway\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/wiegands\n\
  \  method: get\n  operationId: listWiegands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/widgetTypes\n  method: get\n  operationId: listWidgetTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/videoProviderTypes\n  method: get\n  operationId: listVideoProviderTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/users\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/users\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/unusedInputs\n  method: get\n  operationId: listUnusedInputs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/termsAgreements\n  method: get\n  operationId: listTermsAgreements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/termsAgreements\n  method: post\n  operationId: createTermsAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/schedules\n  method: get\n  operationId: listSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/schedules\n  method: post\n  operationId: createSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/readers\n  method: get\n  operationId: listReaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/readers\n  method: post\n  operationId: createReader\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/parcels\n  method: get\n  operationId: listParcels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/parcels\n  method: post\n  operationId: createParcel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/parcels\n  method: delete\n  operationId: deleteParcels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/parcels\n  method: patch\n  operationId: updateParcels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/orgPackagePlans\n  method: get\n  operationId: listOrgPackagePlansSelected\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/mobileAppConfig\n  method: get\n  operationId: describeMobileAppConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/mobileAppConfig\n\
  \  method: delete\n  operationId: deleteMobileAppConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/mobileAppConfig\n  method: patch\n  operationId: updateMobileAppConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/maintenanceWindowMap\n  method: get\n  operationId: listOrgMaintenanceWindowMap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/maintenanceWindowMap\n \
  \ method: post\n  operationId: updateOrgMaintenanceWindowMap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/maintenanceWindowMap\n  method: put\n  operationId: upsertOrgMaintenanceWindowMapForAcus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/maintenanceWindowDefinition\n  method: get\n  operationId: listOrgMaintenanceWindowDefinition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/maintenanceWindowDefinition\n\
  \  method: post\n  operationId: createOrgMaintenanceWindowDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/maintenanceWindowAcuMap\n  method: get\n  operationId: listOrgMaintenanceWindowAcuMap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/maintenanceWindowAcuMap\n  method: put\n  operationId: upsertOrgMaintenanceWindowAcuMap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/mailrooms\n\
  \  method: get\n  operationId: listMailrooms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/mailrooms\n  method: post\n  operationId: createMailroom\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/identityProviders\n  method: get\n  operationId: listIdentityProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/features\n  method: get\n  operationId: listOrgFeatures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /orgs/{orgId}/eolSupervisions\n  method: get\n  operationId: listEolSupervisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/entryStates\n  method: get\n  operationId: listEntryStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/entryStates\n  method: post\n  operationId: createEntryState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/entries\n  method: get\n  operationId: listEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/entries\n  method: post\n  operationId: createEntry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/emailAlertTypes\n  method: get\n  operationId: listEmailAlertTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/badgeConfigs\n  method: get\n  operationId: listBadgeConfigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/badgeConfigs\n  method: post\n  operationId: createBadgeConfig\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/authCerts\n  method: get\n  operationId: listAuthCerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/authCerts\n  method: post\n  operationId: createAuthCert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/alarmStatuses\n  method: get\n  operationId: listAlarmStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/alarmSeverities\n  method: get\n  operationId: listAlarmSeverities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/acuPortTypes\n  method: get\n  operationId: listAcuPortTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/acuPorts\n  method: get\n  operationId: listAllAcuPorts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/acuModels\n  method: get\n  operationId: listAcuModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/acus\n  method:\
  \ get\n  operationId: listAcus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/acus\n  method: post\n  operationId: createAcu\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/alarmActions\n  method: get\n  operationId: listAlarmActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/alarmConfigurations\n  method: get\n  operationId: listAlarmConfigurations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /orgs/{orgId}/alarmConfigurations\n  method: post\n  operationId: createAlarmConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/cardFormats\n  method: get\n  operationId: listCardFormats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/contactSensors\n  method: get\n  operationId: listContactSensors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/credentials\n  method: get\n  operationId: listOrgCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/credentialActionTypes\n  method: get\n  operationId: listCredentialActionTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/credentialTypes\n  method: get\n  operationId: listCredentialTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/customFields\n  method: get\n  operationId: listCustomFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/customFields\n  method: post\n  operationId: createCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/customFields\n  method: patch\n  operationId: updateCustomFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/customFieldTypes\n  method: get\n  operationId: listCustomFieldTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/dashboards\n  method: get\n  operationId: listDashboards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/dashboards\n\
  \  method: post\n  operationId: createDashboard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/emailAlerts\n  method: get\n  operationId: listEmailAlerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/fobAllegions\n  method: get\n  operationId: listOrgFobAllegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/fobAllegions\n  method: post\n  operationId: createOrgFobAllegion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/genericInputs\n  method: get\n  operationId: listGenericInputs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/groups\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/groups\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/hookActions\n  method: get\n\
  \  operationId: listHookActions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/hookActions\n  method: post\n  operationId: createHookAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/hookEvents\n  method: get\n  operationId: listHookEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/orgIdentities\n  method: get\n  operationId: listOrgIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /orgs/{orgId}/identityProviderTypes\n  method: get\n  operationId: listIdentityProviderTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/ios\n  method: get\n  operationId: listIos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/locationMeasurementSourceTypes\n  method: get\n  operationId: listLocationMeasurementSourceTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/lockdownPlans\n  method: get\n  operationId: listLockdownPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/lockdownPlans\n  method:\
  \ post\n  operationId: createLockdownPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/maintenanceWindow\n  method: get\n  operationId: describeOrgMaintenanceWindow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/maintenanceWindow\n  method: delete\n  operationId: deleteOrgMaintenanceWindow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/maintenanceWindow\n  method: patch\n\
  \  operationId: updateOrgMaintenanceWindow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/maintenanceWindow\n  method: put\n  operationId: createOrgMaintenanceWindow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/namespaces\n  method: get\n  operationId: listNamespaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/orgPictures\n  method: get\n  operationId: listOrgPictures\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/orgPictures\n  method: post\n  operationId: createOrgPicture\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/packagePlans\n  method: get\n  operationId: listOrgPackagePlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/palettes\n  method: get\n  operationId: listPalettes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/parcelMessageTypes\n\
  \  method: get\n  operationId: listParcelMessageTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/parcelStatuses\n  method: get\n  operationId: listParcelStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/effectiveScopes\n  method: get\n  operationId: getEffectivePermissionsForOrg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/recentAlarms\n  method: get\n  operationId: listRecentAlarms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/relays\n  method: get\n  operationId: listRelays\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/relayHardwareTypes\n  method: get\n  operationId: listRelayHardwareTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/rexs\n  method: get\n  operationId: listRexs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/roles\n  method: get\n  operationId: listRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/roles\n  method: post\n  operationId: createRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/scheduleTypes\n  method: get\n  operationId: listScheduleTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/scopeResources\n  method: get\n  operationId: listScopeResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/sharedUsers\n  method: get\n  operationId: listSharedUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/sites\n  method: get\n  operationId: listSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/sites\n  method: post\n  operationId: createSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /orgs/{orgId}/thirdPartyReaders\n  method: get\n  operationId: listThirdPartyReaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/thirdPartyWiegands\n  method: get\n  operationId: listThirdPartyWiegands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/triggerMethods\n  method: get\n  operationId: listTriggerMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/wirelessLockGateways\n  method: get\n  operationId: listWirelessLockGateways\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/wirelessLockGateways\n\
  \  method: post\n  operationId: createWirelessLockGateway\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/wirelessLockProviders\n  method: get\n  operationId: listWirelessLockProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/wirelessLockProviders\n  method: post\n  operationId: createWirelessLockProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/wirelessLockReaders\n  method: get\n  operationId: listWirelessLockReaders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{orgId}/wirelessLockReaders\n  method: post\n  operationId: createWirelessLockReader\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{orgId}/wirelessLockTemplates\n  method: get\n  operationId: listWirelessLockTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /orgs/{orgId}/wirelessLockTemplates\n  method: post\n  operationId: createWirelessLockTemplate\n  x-ag\n\n# --- truncated at 32 KB (167 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/openpath/refs/heads/main/agentic-access/openpath-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpath/refs/heads/main/agentic-access/openpath-agentic-access.yml
summary_line: 546 operations · 302 acting · 4 human-in-the-loop
tags:
- Company
- Security
- Access Control
- Physical Security
- Identity
- Credentials
- IoT
- Smart Building
- Avigilon Alta
- Motorola Solutions
---
